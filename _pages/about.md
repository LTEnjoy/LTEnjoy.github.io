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

Hi there! My name is Jin Su. I am now a third-year PhD student at [Westlake University](https://www.westlake.edu.cn/), supervised by Prof. 
[Fajie Yuan](https://fajieyuan.github.io/). 
I received my B.S. degree from [Huazhong University of Science and Technology](https://www.hust.edu.cn/) in 2022, 
where I worked with Prof. [Wei Wei](https://www.eric-weiwei.com/) on the adversarial attack and defense for NLP models.

Currently my research interests lie in the AI for protein, primarily focusing on the protein representation learning. I
am also interested in the newest AI technologies and want to apply them to the protein field.

I also like to write interesting and useful code projects, such as [easyChat](https://github.com/LTEnjoy/easyChat)
<a href="https://github.com/LTEnjoy/easyChat"><img src="https://img.shields.io/github/stars/LTEnjoy/easyChat?style=social&label=Code+Stars" style="max-width: 100%;"></a>
, an easy way to send WeChat messages to your friends automatically. If you have any interesting idea, feel free to
email me!

# 🔥 News

- *2024.09.06*: I will be a reviewer for **ICLR 2025** 🎉🎉🎉!

- *2024.06.03*: We are thrilled to release [ProTrek](https://github.com/westlake-repl/ProTrek), a tri-modal PLM modeling protein sequence, structure and function!

- *2024.05.28*: Our preprint [SaprotHub](https://huggingface.co/SaProtHub) is released! Everyone now can effortlessly process data, train protein model and 
collaborate with an open community🤩!
 
- *2024.01.17*: Our SaProt paper has been accepted as **ICLR 2024 spotlight** 🎉🎉🎉!

- *2023.10.02*: We release [SaProt](https://github.com/westlake-repl/SaProt) <a href="https://github.com/westlake-repl/SaProt"><img src="https://img.shields.io/github/stars/westlake-repl/SaProt?style=social&label=Code+Stars" style="max-width: 100%;"></a>, a 650M structure-aware protein language model. 

# 📝 Publications
\* denotes equal contribution

<div class='paper-box'><div class='paper-box-image'><div><div class="badge"></div><img src='images/papers/ProTrek.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**ProTrek: Navigating the Protein Universe through Tri-Modal Contrastive Learning**

**Jin Su**, Xibin Zhou, Xuting Zhang, Fajie Yuan

<a href="https://www.biorxiv.org/content/10.1101/2024.05.30.596740v1"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>
<a href="https://huggingface.co/spaces/westlake-repl/Demo_ProTrek_650M_UniRef50"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-red?label=Demo" style="max-width: 100%;"></a>
<a href="https://github.com/westlake-repl/ProTrek"><img src="https://img.shields.io/github/stars/westlake-repl/ProTrek?style=social&label=Code+Stars" style="max-width: 100%;"></a>

_bioRxiv preprint_
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge"></div><img src='images/papers/SaprotHub.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**SaprotHub: Making Protein Modeling Accessible to All Biologists**

**Jin Su**, Zhikai Li, Chenchen Han, Yuyang Zhou, Junjie Shan, Xibin Zhou, Dacheng Ma, The OPMC, Sergey Ovchinnikov,
Fajie Yuan

<a href="https://www.biorxiv.org/content/10.1101/2024.05.24.595648v1"><img src="https://img.shields.io/badge/Paper-bioRxiv-green" style="max-width: 100%;"></a>
<a href="https://huggingface.co/SaProtHub"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-red?label=SaprotHub" style="max-width: 100%;"></a>
<a href="https://colab.research.google.com/github/westlake-repl/SaprotHub/blob/main/colab/SaprotHub.ipynb"><img src="images/colab-badge.svg" style="max-width: 100%;"></a>
<a href="https://github.com/westlake-repl/SaProtHub"><img src="https://img.shields.io/github/stars/westlake-repl/SaprotHub?style=social&label=Code+Stars" style="max-width: 100%;"></a>

_bioRxiv preprint_
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge"></div><img src='images/papers/SaProt.png' alt="sym" width="100%"></div></div>
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

<div class='paper-box'><div class='paper-box-image'><div><div class="badge"></div><img src='images/papers/humingyang.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Exploring evolution-aware & -free protein language models as protein function predictors**

Mingyang Hu, Fajie Yuan, Kevin K. Yang, Fusong Ju, **Jin Su**, Hui Wang, Fei Yang, Qiuyang Ding

<a href="https://arxiv.org/abs/2206.06583"><img src="https://img.shields.io/badge/Paper-arXiv-red"></a>
<a href='https://github.com/elttaes/Revisiting-PLMs'><img src="https://img.shields.io/github/stars/elttaes/Revisiting-PLMs?style=social&label=Code+Stars"></a>

_NeurIPS 2022_
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge"></div><img src='images/papers/MAYA.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**Multi-granularity textual adversarial attack with behavior cloning**

Yangyi Chen\*, **Jin Su**\*, Wei Wei

<a href="https://arxiv.org/abs/2109.04367"><img src="https://img.shields.io/badge/Paper-arXiv-red"></a>
<a href='https://github.com/Yangyi-Chen/MAYA'><img src="https://img.shields.io/github/stars/Yangyi-Chen/MAYA?style=social&label=Code+Stars"></a>

_EMNLP 2021_
</div>
</div>

# 🎖 Honors and Awards


[//]: # (- *2021.10* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. )
[//]: # (- *2021.09* Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ornare aliquet ipsum, ac tempus justo dapibus sit amet. )

# 📖 Educations
- *2022.09 - now,* PhD in Westlake University.
- *2018.09 - 2022.06*, B.S. in Huazhong University of Science and Technology.

# 💬 Invited Talks
- *2024.08.23*, Debora Marks Lab of Harvard Medical School: "SaProt and SaprotHub".
- *2024.04.26*, AI for Drug Discovery Team, ByteDance Research: "AlphaFold2 evaluation and SaProt".

# 💻 Internships
- *2021.07 - 2022.06*, Represenation Learning Laboratory, [Westlake University](https://www.westlake.edu.cn/)
- *2020.12 - 2021.05*, [Cognitive Computing and Intelligent Information Processing (CCIIP) Laboratory](http://cciip.cs.hust.edu.cn/)
