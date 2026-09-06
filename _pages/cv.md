---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

<a href="{{ base_path }}/files/cv.pdf" class="btn btn--primary">Download CV as PDF</a>

Education
======
* B.S. in Applied Physics, Peking University, 2022 — 2026
  * EECS Department; GPA: 3.75/4.0 (Top 18%)
  * Advised by [Prof. Meng Li](https://mengli.me/)
* Undergraduate Research Intern, Georgia Institute of Technology, 2025 — 2026
  * [SHARC Lab](https://sharclab.ece.gatech.edu/), ECE Department
  * Advised by [Prof. Cong (Callie) Hao](https://sharclab.ece.gatech.edu/)

Core courses: Hardware Foundations of Artificial Intelligence (A+), Machine Learning for Electronics Information Engineering (A), Undergraduate Research Practice (A), Chip Design using High-level Programming Language (A)

Research experience
======

* **CREATE: Cross-Layer Resilience Characterization and Optimization for Efficient yet Reliable Embodied AI Systems** (accepted by ASPLOS 2026)
  * Jul 2024 — Mar 2025, Peking University, advised by [Prof. Meng Li](https://mengli.me/)
  * Assessed the reliability of modern LLM-based embodied AI systems and proposed error detection and correction methodologies at the application, system, and circuit levels.
  * Applied SmoothQuant's fault-injection methodology, identifying o_proj and down_proj as the most sensitive layers.
  * Designed a lightweight AD circuit that protects the planner, improving robustness from 10<sup>-7</sup> to 10<sup>-3</sup> BER.
  * Used QuaRot to remap sensitive weight matrices to a more uniform domain, boosting robustness from 10<sup>-7</sup> to 10<sup>-5</sup> BER.
  * Integrated an entropy-aware LDO for dynamic voltage scaling, cutting compute energy by 40.6%.

* **Faster-MoA: Low-Latency Tree-Structured MoA Serving with Early Exit and Agent-Aware Prefill-Decode Overlap** (accepted by DAC 2026)
  * Mar 2025 — Nov 2025, Georgia Tech SHARC Lab, advised by [Prof. Cong (Callie) Hao](https://sharclab.ece.gatech.edu/)
  * Goal: rival server-level large models with small but powerful models through cross-agent communication.
  * Systematically profiled the influence of different configurations on the overall performance of the MoA system.
  * Introduced a novel tree architecture for local aggregation and pipelined the prefilling and decoding stages.
  * Applied PEFT via LLaMA-Factory to diversify proposer exploration directions and decrease mutual semantic overlap.
  * Managed KV-cache for consecutive layers in the MoA system.
  * Applied semantic-similarity-based early exit to prune unnecessary inferences (10× faster) with only ±1% accuracy variation.

* **DySL-VLA: Efficient Vision-Language-Action Model Inference via Dynamic-Static Layer-Skipping for Robot Manipulation** (accepted by DAC 2026)
  * Feb 2025 — May 2025, Peking University, advised by [Prof. Meng Li](https://mengli.me/)
  * Assessed the inter-layer similarity of VLA models and proposed an adaptive layer-skip scheme that bypasses layers based on task requirements and motion significance.
  * Profiled VLA models' robustness under dynamic layer skipping and quantified activation similarity between adjacent layers (mean ~80%).
  * Trained adapters and skip controllers in two stages, reducing trainable parameters by 85.7× versus full-parameter fine-tuning.
  * Identified that trajectory continuity reflects the importance of the current action.

Course projects
======

* **CircuitNet — Congestion Prediction for VLSI Layouts** (final project for Machine Learning for Electronics Information Engineering)
  * Forecast cell-level routing congestion from post-placement layout images.
  * Implemented and benchmarked baseline UNet, deeper UNet, UNet+SE, and Double-UNet on the CircuitNet dataset with NRMSE, SSIM, and EMD; ablated depth, attention, normalization, and activation choices.
  * Ran PTQ and QAT experiments at different bit-widths on weights and activations, and analyzed decoder- versus encoder-sensitivity to quantization noise.

* **SpMM Accelerator ASIC Design** (final project for Chip Design using High-level Programming Language)
  * Designed an SpMM accelerator to optimize multiplication between an N × N row-compressed sparse matrix and an N × N dense matrix.
  * Implemented the FAN-network within the Reduction Unit to compute partial sums of power-of-2 elements, and a PE core performing SpMV with Halo-Adder cross-boundary sums.
  * Designed a PE array that transforms ordinary matrices into row-compressed format and parallelizes SpMV computations into SpMM operations.
  * Integrated double input/output buffers (Dbbuf) for simultaneous data transfer and computation, and output/weight-stationary (OS/WS) dataflows for finer control with alleviated I/O occupation.

Skills
======
* Programming: C++, Python, PyTorch, Verilog
* Developer tools: Vivado, Vitis, Linux, Git, Docker

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
