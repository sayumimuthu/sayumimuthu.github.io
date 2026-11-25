---
layout: page
title: "ABSORB: Discrete Diffusion for Single-Cell RNA-seq Imputation"
description: Treating dropout as masked missingness for selective imputation of gene expression.
img: assets/img/proj_absorb.jpg
importance: 1
category: computational biology
permalink: /projects/absorb/
related_publications: true
---

**Area:** Computational biology, generative modeling &nbsp;·&nbsp; **Period:** January 2026 – present &nbsp;·&nbsp; **Status:** Under review at ICLR 2027 {% cite adhikari2026absorb %}

In single-cell RNA sequencing, a zero count can mean two very different things: the transcript was present but not captured (dropout), or the gene is genuinely not expressed. ABSORB aims to impute only the former.

#### What I did

- Studied the ambiguity of zero counts in scRNA-seq, distinguishing **missing transcript measurements** from **biologically meaningful zeros** through selective imputation.
- Worked on an **absorbing [MASK]-state** formulation using **per-gene quantile tokenization**, a **role-conditioned Transformer**, fixed observed context and **confidence-ordered parallel reconstruction**.
- Contributed to research on modeling dropout as masked missingness and to the experimental evaluation.

#### Methods

Discrete diffusion · Transformers · self-supervised learning · transcriptomics
