# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a Jekyll-based academic personal homepage (forked from AcadHomepage) that automatically updates Google Scholar citations via GitHub Actions. The site is deployed to GitHub Pages.

## Development Commands

**Start local development server:**
```bash
bash run_server.sh
```
This runs `bundle exec jekyll liveserve` with live reload. Access at http://127.0.0.1:4000

**Install dependencies:**
```bash
bundle install
```

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

Publication card styles (`.paper-box`, `.paper-box-image`, `.paper-box-text`, `.badge`) are defined in `assets/css/main.scss` (not in `_sass/`). This is where to make layout changes to the publications section.

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
