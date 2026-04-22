---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hi there! My name is Jin Su. I am now a fourth-year PhD student at [Zhejiang University](https://www.zju.edu.cn/) and [Westlake University](https://www.westlake.edu.cn/), supervised by Prof. 
[Fajie Yuan](https://fajieyuan.github.io/). 
I received my B.S. degree from [Huazhong University of Science and Technology](https://www.hust.edu.cn/) in 2022, 
where I worked with Prof. [Wei Wei](https://www.eric-weiwei.com/) on the adversarial attack and defense for NLP models.

In the early stages of my PhD, my research centered on AI for protein science, with a primary focus on protein 
representation learning. Recently, I have transitioned my research focus toward the development of advanced AI agents.

I also like to write interesting and useful code projects, such as [easyChat](https://github.com/LTEnjoy/easyChat) <a href="https://github.com/LTEnjoy/easyChat"><img src="https://img.shields.io/github/stars/LTEnjoy/easyChat?style=social&label=Code+Stars" style="max-width: 100%; vertical-align: middle;"></a> — an easy way to send WeChat messages to your friends automatically. If you have any interesting idea, feel free to email me!

# 🔥 News

- *2025.08.07*: Our SaprotHub paper has also been accepted by Nature Biotechnology🎉🎉🎉!

- *2025.07.08*: Our ProTrek paper has been accepted by Nature Biotechnology🎉🎉🎉!

- *2024.09.06*: I will be a reviewer for **ICLR 2025**.

- *2024.06.03*: We are thrilled to release [ProTrek](https://github.com/westlake-repl/ProTrek), a tri-modal PLM modeling protein sequence, structure and function!

- *2024.05.28*: Our preprint [SaprotHub](https://huggingface.co/SaProtHub) is released! Everyone now can effortlessly process data, train protein model and 
collaborate with an open community🤩!
 
- *2024.01.17*: Our SaProt paper has been accepted as **ICLR 2024 spotlight** 🎉🎉🎉!

- *2023.10.02*: We release [SaProt](https://github.com/westlake-repl/SaProt) <a href="https://github.com/westlake-repl/SaProt"><img src="https://img.shields.io/github/stars/westlake-repl/SaProt?style=social&label=Code+Stars" style="max-width: 100%;"></a>, a 650M structure-aware protein language model. 

# 📝 Publications
\* denotes equal contribution

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**U-Fold: Dynamic Intent-Aware Context Folding for User-Centric Agents**

**Jin Su**, Runnan Fang, Yeqiu Li, ..., Ningyu Zhang, Fajie Yuan

<a href="https://arxiv.org/abs/2601.18285"><img src="https://img.shields.io/badge/Paper-arXiv-red" style="max-width: 100%;"></a>

_ACL 2026 Findings_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**Prime: A multi-agent environment for orchestrating dynamic computational workflows in protein engineerings**

Yuyang Zhou, **Jin Su**\*, Jiawei Zhang, ..., Li Fan, Fajie Yuan

<a href="https://doi.org/10.1101/2025.09.22.677756"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>

_preprint_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**A trimodal protein language model enables advanced protein searches**

**Jin Su**, Yan He, Shiyang You, ..., Hongyuan Lu, Fajie Yuan

<a href="https://www.biorxiv.org/content/10.1101/2024.05.30.596740v1"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>
<a href="https://huggingface.co/spaces/westlake-repl/Demo_ProTrek_650M_UniRef50"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-red?label=Demo" style="max-width: 100%;"></a>
<a href="https://github.com/westlake-repl/ProTrek"><img src="https://img.shields.io/github/stars/westlake-repl/ProTrek?style=social&label=Code+Stars" style="max-width: 100%;"></a>

_Nature Biotechnology 2025_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**Democratizing protein language model training, sharing and collaboration**

**Jin Su**, Zhikai Li, Tianli Tao, ..., Sergey Ovchinnikov, Fajie Yuan

<a href="https://www.biorxiv.org/content/10.1101/2024.05.24.595648v1"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>
<a href="https://huggingface.co/SaProtHub"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-red?label=SaprotHub" style="max-width: 100%;"></a>
<a href="https://colab.research.google.com/github/westlake-repl/SaprotHub/blob/main/colab/SaprotHub.ipynb"><img src="images/colab-badge.svg" style="max-width: 100%;"></a>
<a href="https://github.com/westlake-repl/SaProtHub"><img src="https://img.shields.io/github/stars/westlake-repl/SaprotHub?style=social&label=Code+Stars" style="max-width: 100%;"></a>

_Nature Biotechnology 2025_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**SaProt: Protein Language Modeling with Structure-aware Vocabulary**

**Jin Su**, Chenchen Han, Yuyang Zhou, Junjie Shan, Xibin Zhou, Fajie Yuan

<a href="https://www.biorxiv.org/content/10.1101/2023.10.01.560349v3"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>
<a href="https://huggingface.co/westlake-repl/SaProt_650M_AF2"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-red?label=Model" style="max-width: 100%;"></a>
<a href="https://portal.valencelabs.com/blogs/post/saprot-protein-language-modeling-with-structure-aware-vocabulary-uyLPrUZqyDF60Yr" alt="blog"><img src="https://img.shields.io/badge/Blog-Portal-violet" /></a> 
<a href="https://zhuanlan.zhihu.com/p/664754366" alt="zhihu"><img src="https://img.shields.io/badge/Zhihu-知乎-blue" /></a> 
<a href="https://github.com/westlake-repl/SaProt"><img src="https://img.shields.io/github/stars/westlake-repl/SaProt?style=social&label=Code+Stars" style="max-width: 100%;"></a>

_ICLR 2024 spotlight_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**Exploring evolution-aware &amp; -free protein language models as protein function predictors**

Mingyang Hu, Fajie Yuan, Kevin K. Yang, Fusong Ju, **Jin Su**, Hui Wang, Fei Yang, Qiuyang Ding

<a href="https://arxiv.org/abs/2206.06583"><img src="https://img.shields.io/badge/Paper-arXiv-red"></a>
<a href='https://github.com/elttaes/Revisiting-PLMs'><img src="https://img.shields.io/github/stars/elttaes/Revisiting-PLMs?style=social&label=Code+Stars"></a>

_NeurIPS 2022_
</div>
</div>

<div class='paper-box'>
<div class='paper-box-text' markdown="1">

**Multi-granularity textual adversarial attack with behavior cloning**

Yangyi Chen\*, **Jin Su**\*, Wei Wei

<a href="https://arxiv.org/abs/2109.04367"><img src="https://img.shields.io/badge/Paper-arXiv-red"></a>
<a href='https://github.com/Yangyi-Chen/MAYA'><img src="https://img.shields.io/github/stars/Yangyi-Chen/MAYA?style=social&label=Code+Stars"></a>

_EMNLP 2021_
</div>
</div>

[//]: # (# 🎖 Honors and Awards)


[//]: # (- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. )
[//]: # (- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. )


# 💬 Invited Talks
- *2025.12.05*, [The Shanghai Institute for Advanced Immunochemical Studies, SIAIS](https://siais.shanghaitech.edu.cn/main.htm): "ProTrek and SaprotHub: Enhancing Protein Research through Deep Learning Technology".
- *2024.11.26*, [Machine learning for protein engineering seminar](https://x.com/ml4proteins): "ProTrek: Navigating the Protein Universe through Tri-Modal Contrastive Learning".
- *2024.08.23*, [Debora Marks Lab of Harvard Medical School](https://www.deboramarkslab.com/): "SaProt and SaprotHub".
- *2024.04.26*, AI for Drug Discovery Team, ByteDance Research: "AlphaFold2 evaluation and SaProt".

# 💻 Internships
- *2025.09 - 2026.02*, [Tongyi Lab, Alibaba Group](https://careers-tongyi.alibaba.com/?lang=zh)
- *2021.07 - 2022.06*, Represenation Learning Laboratory, [Westlake University](https://www.westlake.edu.cn/)
- *2020.12 - 2021.05*, [Cognitive Computing and Intelligent Information Processing (CCIIP) Laboratory](http://cciip.cs.hust.edu.cn/)

# 📖 Educations
- *2022.09 - now,* PhD in Westlake University.
- *2018.09 - 2022.06*, B.S. in Huazhong University of Science and Technology.
