---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* M.S. in Integrated Circuit Engineering, Peking University, 2024 - 2027 (expected)
  * Advisors: Prof. Tianyu Jia, Prof. Dunshan Yu
  * Honor: Merit Student of Peking University
* B.S. in IC Design and Integrated Systems, Hefei University of Technology, 2019 - 2023
  * Honor: University's Science and Technology Activity Awards

Research Interests
======
* 3D integration architecture for emerging AI applications
* Scalable AI computing systems
* Efficient RISC-V AI accelerator chips

Research Experience
======
* **3D-Stacked Chip Architecture and Algorithm Optimization for VLMs**, Sep 2025 - Mar 2026
  * Designed a 3D-stacked chip architecture for VLM-based video understanding, combining a content-aware sparse attention algorithm with a multi-core dynamic parallel strategy.
  * Proposed a content-aware attention map prediction method that classifies each attention head into three types online using lightweight computation.
  * Addressed inter-core load imbalance on the many-core logic layer with a dynamic hybrid parallel strategy integrating head-wise and sequence-wise parallelism.

* **Thermal-Aware PNM-Based Heterogeneous Architecture for Multi-Turn Dialogue LLM Inference**, Nov 2025 - Apr 2026
  * Proposed a thermal-aware GPU-PNM heterogeneous architecture with dynamic request offloading, targeting the fluctuating compute intensity of incremental prefill and memory-bound decode.
  * Implemented a prefix-cache-based Radix-tree strategy for dynamic request scheduling, with co-processing and adaptive mode-switching to mitigate workload imbalance.
  * Optimized PNM thermal behavior through content-aware prefix cache mapping and logic-layer layout refinement.

* **Chiplet Optimization with Optical Interconnects for LLM Training**, Apr 2025 - Sep 2025
  * Developed a cross-layer optimization framework for LLM training clusters using chiplets and optical interconnects, exploiting spatial and temporal unevenness in training traffic.
  * Jointly optimized MCM architecture, optical network topology, and training parallelism under a cost-aware model.
  * Achieved up to 19.58x higher training throughput than conventional GPU clusters and 41% improvement over prior network designs at similar cost.

* **Context-Aware Multi-Speaker ASR Accelerator with Microscaling CIM**, Jan 2025 - Aug 2025
  * Built a CIM-based streaming multi-speaker ASR accelerator featuring context-aware redundancy skipping, a 2D-writable MX-DCIM with static and dynamic pages, and a similarity-aware TCAM for approximate speaker search and N-best caching.
  * Independently implemented an end-to-end real-time KWS demo covering the full silicon lifecycle: RTL design, FPGA prototyping, backend physical implementation, and tape-out.
  * Post-silicon validation integrated MCU-based VAD and MFCC preprocessing on a custom PCB; a lightweight CNN trained on GSCD and quantized via PTQ runs on CIM and a custom VPU under RISC-V CPU control.

Engineering Projects
======
* **Hardware Simulator for Groq-LPU and Ascend Davinci Cube**, Nov 2025 - Apr 2026
  * Developed a behavioral simulator for comparative performance analysis between the Groq-LPU and a Huawei Davinci Cube baseline.
  * Modeled both architectures at the behavioral level under a 12nm process node, including an L1-L0 memory hierarchy and optimized workload partitioning for the baseline.
  * Huawei 2012 Laboratories joint university-industry project (ongoing).

Skills
======
* **Programming**: SystemVerilog, Python, C, LaTeX
* **EDA Tools**: VCS, Verdi, Spyglass, Genus, Innovus, Vivado, Altium Designer, Keil
* **Testing**: SMU, DMM, digital oscilloscope, J-Link debugger

Honors and Awards
======
* Merit Student of Peking University, 2025
* Hefei University of Technology's Science and Technology Activity Awards, 2022
* Honorable Mention, National Finals, 6th IC-Innovation Challenge for Graduate Students, 2022
* Honorable Mention, FPGA Innovation Design Contest, Chinese Institute of Electronics, 2022

Publications
======
  <ol>{% for post in site.publications reversed %}
    <li>{{ post.citation }}</li>
  {% endfor %}</ol>
