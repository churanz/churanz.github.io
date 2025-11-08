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

# ℹ️ Short Bio

Hi, I’m Churan, a master’s student at the University of California, San Diego.

I have the great honor of being collaborating with Prof. [Junbao Zhuo](https://scholar.google.com/citations?user=iBt9uHUAAAAJ&hl=en), [Julian McAuley](https://cseweb.ucsd.edu/~jmcauley/).

My current research interests lie primarily in Natural Language Processing and Deep Learning.

# 📖 Educations
<table>
  <tr>
    <td style="width: 60px; border: none; padding: 10px 15px 10px 0;">
      <img src="./images/ucsd_badge.png" width="80">
    </td>
    <td style="border: none; vertical-align: middle;">
      <b>University of California, San Diego</b><br>
      M.S. in Computer Science
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2024 - 2026</i>
    </td>
  </tr>
  <tr>
    <td style="width: 60px; border: none; padding: 10px 15px 10px 0;">
      <img src="./images/bjtu_badge.png" width="80">
    </td>
    <td style="border: none; vertical-align: middle;">
      <b>Beijing Jiaotong University</b><br>
      B.S. in Computing Science<br>
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2020 - 2024</i>
    </td>
  </tr>
</table>



# 📝 Publications 

<div class='paper-box'>
  <div class='paper-box-image'>
    <img src='images/paper_main/densemixer.png' alt="sym" width="80%">
  </div>
  <div class='paper-box-text' markdown="1">

**[1] DenseMixer: Improving MoE Post-Training with Precise Router Gradients**

Feng Yao, Junxia Cui, Ruohan Zhang, Liyuan Liu, Shibo Hao, Li Zhang, Chengyu Dong, **Churan Zhi**, Shuohang Wang, Yelong Shen, Jianfeng Gao, Jingbo Shang  

**ICLR 2026**

**Short Summary:** We introduce DenseMixer, a novel MoE post-training technique that trades one extra forward pass on inactive experts for a more precise router gradient estimation. Our method consistently outperforms conventional methods across different MoE scales (7B, 14B, 16B, 30B), architectures (with/without shared experts), pre-training methods (from scratch/up-cycling), and post-training data types (instruction/long CoT data). It is universally applicable to any MoE using Top-K routing and can be used in a plug-and-play manner, compatible with existing training libraries and parameter-efficient methods like LoRA, introducing no changes to inference.

[Paper](https://fengyao.notion.site/moe-posttraining)
  </div>
</div>

---

<div class='paper-box'>
  <div class='paper-box-image'>
    <img src='images/paper_main/overview of H3M-SSMoEs.png' alt="sym" width="80%">
  </div>
  <div class='paper-box-text' markdown="1">

**[2] H3M-SSMoEs: Hypergraph-based Multimodal Learning with LLM Reasoning and Style-Structured Mixture of Experts**

Peilin Tan, Liang Xie, **Churan Zhi**, Dian Tu, Chuanqi Shi  

**WWW 2026**

**Short Summary:** Stock movement prediction remains fundamentally challenging due to complex temporal dependencies, heterogeneous modalities, and dynamically evolving inter-stock relationships. Existing approaches often fail to unify structural, semantic, and regime-adaptive modeling within a scalable framework. This work introduces H3M-SSMoEs, a novel Hypergraph-based MultiModal architecture with LLM reasoning and Style-Structured Mixture of Experts, integrating three key innovations: (1) a Multi-Context Multimodal Hypergraph that hierarchically captures fine-grained spatiotemporal dynamics via a Local Context Hypergraph (LCH) and persistent inter-stock dependencies through a Global Context Hypergraph (GCH), employing shared cross-modal hyperedges and Jensen-Shannon Divergence weighting mechanism for adaptive relational learning and cross-modal alignment; (2) a LLM-enhanced reasoning module, which leverages a frozen large language model with lightweight adapters to semantically fuse and align quantitative and textual modalities, enriching representations with domain-specific financial knowledge; and (3) a Style-Structured Mixture of Experts (SSMoEs) that combines shared market experts and industry-specialized experts, each parameterized by learnable style vectors enabling regime-aware specialization under sparse activation. Extensive experiments on three major stock markets demonstrate that H3M-SSMoEs surpasses state-of-the-art methods in both superior predictive accuracy and investment performance, while exhibiting effective risk control. 

[Paper](https://arxiv.org/abs/2510.25091)
  </div>
</div>

---

<div class='paper-box'>
  <div class='paper-box-image'>
    <img src='images/paper_main/biasfreebench.png' alt="sym" width="80%">
  </div>
  <div class='paper-box-text' markdown="1">

**[3] BiasFreeBench: a Benchmark for Mitigating Bias in Large Language Model Responses**

Xin Xu, Xunzhi He#, **Churan Zhi#**, Ruizhe Chen, Julian McAuley, Zexue He  

**ICLR 2026**

**Short Summary:** Existing studies on bias mitigation methods for large language models (LLMs) use diverse baselines and metrics to evaluate debiasing performance, leading to inconsistent comparisons among them. Moreover, their evaluations are mostly based on the comparison between LLMs’ probabilities of biased and unbiased contexts, which ignores the gap between such evaluations and real-world use cases where users interact with LLMs by reading model responses and expect fair and safe outputs rather than LLMs’ probabilities. To enable consistent evaluation across debiasing methods and bridge this gap, we introduce BIASFREEBENCH, an empirical benchmark that comprehensively compares eight mainstream bias mitigation techniques (covering four prompting-based and four training-based methods) on two test scenarios (multi-choice QA and open-ended multi-turn QA) by reorganizing existing datasets into a unified query-response setting.

[Paper](https://arxiv.org/abs/2510.00232)
  </div>
</div>

---

<div class='paper-box'>
  <div class='paper-box-image'>
    <img src='images/paper_main/cpc.png' alt="sym" width="80%">
  </div>
  <div class='paper-box-text' markdown="1">

**[4] Confusing Pair Correction Based on Category Prototype for Domain Adaptation under Noisy Environments**

**Churan Zhi**, Junbao Zhuo, Shuhui Wang  

**AAAI 2024**

**Short Summary:** In this paper, we address unsupervised domain adaptation under noisy environments, which is more challenging and practical than traditional domain adaptation. In this scenario, the model is prone to overfitting noisy labels, resulting in a more pronounced domain shift and a notable decline in the overall model performance. Previous methods employed prototype methods for domain adaptation on robust feature spaces. However, these approaches struggle to effectively classify classes with similar features under noisy environments. To address this issue, we propose a new method to detect and correct confusing class pair. We first divide classes into easy and hard classes based on the small loss criterion. We then leverage the top-2 predictions for each sample after aligning the source and target domain to find the confusing pair in the hard classes. We apply label correction to the noisy samples within the confusing pair. With the proposed label correction method, we can train our model with more accurate labels.

[Paper](https://arxiv.org/abs/2403.12883)
  </div>
</div>

# 🧭 Experiences

## 💼 Internships
<table>
  <tr>
    <td style="border: none; vertical-align: middle;">
      <b>Amazon</b><br>
      Software Engineer - Store: Tax Engine
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2025.06 - 2025.09</i>
    </td>
  </tr>
  <tr>
    <td style="border: none; vertical-align: middle;">
      <b>Microsoft</b><br>
      Software Engineer (AI/ML) - WebXT: Search & Distribution
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2024.05 - 2024.07</i>
    </td>
  </tr>
  <tr>
    <td style="border: none; vertical-align: middle;">
      <b>Xiaomi</b><br>
      Machine Learning Engineer
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2024.02 - 2024.04</i>
    </td>
  </tr>
</table>

---

## 🔬 Research Experience
<table>
  <tr>
    <td style="border: none; vertical-align: middle;">
      <b>University of California, San Diego</b><br>
      Research Assistant
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2024.09 - Present</i>
    </td>
  </tr>
    <tr>
    <td style="border: none; vertical-align: middle;">
      <b>Chinese Academy of Sciences</b><br>
      Research Assistant
    </td>
    <td style="text-align: right; border: none; vertical-align: middle; white-space: nowrap;">
      <i>2022.02 - 2023.08</i>
    </td>
  </tr>
</table>

# 🔥 News
- *2025.10*: &nbsp;😁 We open-sourced the [H3M-SSMoEs](https://github.com/PeilinTime/H3M-SSMoEs).

Last Update: 11/2025
<script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=CtwH9f0klgyu3hreJLQ63mnhOIdBap86JLjOOEr19qk&cl=ffffff&w=a"></script>

