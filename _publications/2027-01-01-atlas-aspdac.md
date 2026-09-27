---
title: "ATLAS: A Thermal-Aware Hybrid-Bonding Based Heterogeneous Architecture Empowering LLM Multi-turn Dialogue System"
collection: publications
category: conferences
permalink: /publication/2027-01-01-atlas-aspdac
excerpt: 'A thermal-aware GPU-PNM heterogeneous architecture with prefix-cache-based Radix-tree scheduling for LLM multi-turn dialogue inference.'
date: 2027-01-01
venue: '32nd Asia and South Pacific Design Automation Conference (ASP-DAC)'
citation: '<b>Y. Ding</b>, Q. Wang, K. Ji, D. Yu, T. Jia*. (2027). &quot;ATLAS: A Thermal-Aware Hybrid-Bonding Based Heterogeneous Architecture Empowering LLM Multi-turn Dialogue System.&quot; <i>32nd Asia and South Pacific Design Automation Conference (ASP-DAC)</i>.'
---

LLM multi-turn dialogue workloads alternate between compute-intensive incremental prefill and memory-bound decode, which strains conventional homogeneous deployments. ATLAS proposes a thermal-aware GPU-PNM heterogeneous architecture with a dynamic request offloading strategy.

Unlike traditional prefill/decode-decoupled systems, this architecture implements a prefix-cache-based Radix-tree strategy for dynamic request scheduling and offloading. By integrating co-processing and adaptive mode-switching, the system mitigates workload imbalance in complex, real-world deployments. The thermal performance of PNM processors is optimized through content-aware prefix cache mapping and logic-layer layout refinement, lowering operational temperatures.
