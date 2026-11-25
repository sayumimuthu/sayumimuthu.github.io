---
layout: page
title: Prompt Sensitivity and Evaluation Artifacts in LLMs
description: Is it the model or the metric? Separating genuine prompt sensitivity from scoring artifacts.
img: assets/img/proj_prompt_sensitivity.jpg
importance: 1
category: language models & responsible AI
permalink: /projects/prompt-sensitivity/
github: https://github.com/sayumimuthu/llm-prompt-sensitivity-evaluation-artifact
related_publications: true
---

**Area:** LLM evaluation, reproducibility &nbsp;·&nbsp; **Period:** 2026 &nbsp;·&nbsp; **Status:** Published at IEEE MERCon 2026 {% cite muthukumarana2026promptsensitivity %}

LLMs are often reported to be highly sensitive to small changes in prompt wording. This project asks how much of that observed sensitivity actually comes from the model, and how much is introduced by the way responses are scored.

#### What I did

- Designed an **eight-template evaluation experiment** spanning ARC-Challenge, BoolQ and SQuAD, studying **nine LLMs** and **43,200 prompt-response-judge triples**.
- Introduced **Evaluation-Attributable Sensitivity (EAS)** and **Signed EAS** to separate genuine generation variation from differences introduced by heuristic scoring and LLM-as-judge evaluation.
- Examined how benchmark format and scoring method affect observed sensitivity, identifying contexts in which automatic metrics under- or over-estimate response instability.

#### Methods

Benchmark design · experimental controls · prompt evaluation · statistical analysis · reproducible research artifacts

#### Links

<i class="fa-brands fa-github"></i> [Code](https://github.com/sayumimuthu/llm-prompt-sensitivity-evaluation-artifact) &nbsp;·&nbsp; <i class="fa-solid fa-file-lines"></i> [Paper (IEEE Xplore)](https://ieeexplore.ieee.org/document/11691277)
