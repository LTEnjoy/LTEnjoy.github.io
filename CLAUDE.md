# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based academic personal homepage (forked from AcadHomepage) that automatically updates Google Scholar citations via GitHub Actions. The site is deployed to GitHub Pages.

## Development Commands

**Start local development server (Linux/Mac):**
```bash
bundle exec jekyll liveserve
```
Access at http://127.0.0.1:4000. On Windows, install Ruby via [RubyInstaller](https://rubyinstaller.org/downloads/) (Ruby+Devkit), then run the command above in PowerShell.

**Install dependencies:**
```bash
bundle install
```

**Deploy:** Push to `main` — GitHub Pages builds and publishes automatically within ~1 minute.

## Architecture

### Jekyll Structure
- `_pages/about.md` - Main homepage content (markdown + HTML)
- `_layouts/` - Page templates (default.html)
- `_includes/` - Reusable components (header, sidebar, analytics, etc.)
- `_sass/` - Stylesheets
- `_data/navigation.yml` - Navigation configuration
- `_config.yml` - Site configuration (author info, SEO, plugins)

### Google Scholar Citation System

**Automated crawler workflow:**
- GitHub Action (`.github/workflows/google_scholar_crawler.yaml`) runs daily at 08:00 UTC and on page builds
- Python script (`google_scholar_crawler/main.py`) fetches citation data using the `scholarly` library
- Requires `GOOGLE_SCHOLAR_ID` secret set in repository settings
- Outputs `gs_data.json` and `gs_data_shieldsio.json` to the `google-scholar-stats` branch (separate from main)

**Displaying paper citations:**
Use a `<span>` tag with class `show_paper_citations` and the Google Scholar paper ID:
```html
<span class='show_paper_citations' data='DhtAFkwAAAAJ:ALROH1vI_8AC'></span>
```
The paper ID comes from the `citation_for_view=XXXX` parameter in the Google Scholar paper URL.

**Citation data loading:**
The `_includes/fetch_google_scholar_stats.html` include fetches citation data from either:
- CDN: `https://cdn.jsdelivr.net/gh/{repo}@google-scholar-stats/gs_data_shieldsio.json` (if `google_scholar_stats_use_cdn: true`)
- Raw GitHub: `https://raw.githubusercontent.com/{repo}/google-scholar-stats/gs_data_shieldsio.json`

### Custom Styles

All custom CSS lives in `assets/css/main.scss` (not in `_sass/`). Key custom classes defined there:

- `.paper-box` / `.paper-box-text` — publication card layout; text takes full width (no image column)
- `.publications-list` — scrollable container wrapping all paper-box cards (fixed `max-height: 600px`, `overflow-y: auto`)
- `.pub-year` — small gray year label rendered before each paper title
- `.badge` — absolute-positioned overlay label on paper images (dark blue)
- `paper-box-text em:last-of-type` — venue label styled as a subtle gray pill tag (e.g. _ICLR 2024 spotlight_)

Font: Inter (loaded via Google Fonts in `_includes/head/custom.html`), falling back to system UI fonts. The font variable is overridden in `_sass/_variables.scss`.

### Publication Entry Format

Each entry in `_pages/about.md` follows this structure — **do not deviate**:

```html
<div class='paper-box'>
<div class='paper-box-text' markdown="1">
<span class="pub-year">YEAR</span> **[Paper Title](https://link-to-paper)**

Author list (**bold** for this author, \* for equal contribution)

<a href="..."><img src="https://img.shields.io/badge/..."></a>  <!-- optional extra badges: HuggingFace, GitHub, Colab, etc. -->

_Venue Name_
</div>
</div>
```

Rules:
- Paper link goes on the **title**, not as a separate badge
- Other resource badges (HuggingFace, GitHub Stars, Colab, Blog) are kept below the author line
- All entries are wrapped in `<div class="publications-list">...</div>`

### Configuration

Primary site configuration is in `_config.yml`:
- Author information (name, bio, social links, email)
- SEO settings (Google Analytics, site verification)
- Jekyll plugins and build settings
- Excluded directories (docs, google_scholar_crawler)

## Important Notes

- The `google-scholar-stats` branch is auto-generated and should not be manually edited
- Changes to `_config.yml` require restarting the Jekyll server
- The site uses kramdown for markdown processing with GFM input
- Timezone is set to Asia/Shanghai
