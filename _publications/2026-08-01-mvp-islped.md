---
title: "MVP: A Mobile 3D-Stacked VLM Accelerator for Efficient Video Understanding by Leveraging Dynamic Sparse Attention Patterns"
collection: publications
category: conferences
permalink: /publication/2026-08-01-mvp-islped
excerpt: 'A 3D-stacked VLM accelerator combining content-aware sparse attention with a multi-core dynamic parallel strategy for video understanding.'
date: 2026-08-01
venue: 'International Symposium on Low Power Electronics and Design (ISLPED)'
citation: '<b>Y. Ding</b>, Q. Wang, D. Yu, T. Jia*. (2026). &quot;MVP: A Mobile 3D-Stacked VLM Accelerator for Efficient Video Understanding by Leveraging Dynamic Sparse Attention Patterns.&quot; <i>International Symposium on Low Power Electronics and Design (ISLPED)</i>.'
---

For VLM-based video understanding tasks, MVP designs a 3D-stacked chip architecture that combines a content-aware sparse attention algorithm with a multi-core dynamic parallel strategy.

The work proposes a content-aware attention map feature prediction method in which each attention head is classified into one of three types, with classification performed online using lightweight computation. To tackle the inter-core load imbalance that arises when deploying sparse-attention VLM models on the many-core logic layer of a 3D-stacked architecture, the design employs a dynamic hybrid parallel strategy integrating head-wise and sequence-wise parallelism based on inter-core grouping.
