---
layout: page
title: ELTLM-Bench
description: Benchmarking temporal perception and reasoning in longitudinal clinical imaging.
img: assets/img/publication_preview/eltlm.svg
importance: 1
---

[Paper](https://aclanthology.org/2026.findings-acl.772/) · [PDF](https://aclanthology.org/2026.findings-acl.772.pdf) · [GitHub](https://github.com/ChengFeng233/ELTLM-Bench) · [Dataset](https://huggingface.co/datasets/Chengfeng233/ELTLM-Bench)

### Research question

Can a large multimodal model compare clinical data from multiple time points and reason about progression, rather than interpreting one exam in isolation?

### What the benchmark evaluates

- **Temporal Perception QA:** identifies changes between clinical time points.
- **Temporal Reasoning QA:** uses changes across exams to answer questions about progression and related clinical context.

The benchmark is derived from longitudinal chest X-rays in MIMIC-CXR. The evaluation found that the tested models struggled to ground their answers in evidence across time points; the paper reports results and error analyses by task.

The [dataset repository](https://huggingface.co/datasets/Chengfeng233/ELTLM-Bench) provides questions and reference answers. Access to the underlying images follows the [PhysioNet MIMIC-CXR access requirements](https://physionet.org/content/mimic-cxr/2.1.0/).
