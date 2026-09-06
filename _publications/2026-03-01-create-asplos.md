---
title: "CREATE: Cross-Layer Resilience Characterization and Optimization for Efficient yet Reliable Embodied AI Systems"
collection: publications
category: conferences
permalink: /publication/2026-create-asplos
excerpt: 'Characterizing the reliability of LLM-based embodied AI systems across the application, system, and circuit layers, with error detection and correction techniques for efficient yet reliable embodied AI.'
date: 2026-03-01
venue: 'ASPLOS 2026'
paperurl: ''
citation: 'T. Xie*, Y. Qi*, J. Wen, Z. Wan, Y. Dong, Z. Wang, S. Cai, Y. Liang, T. Jia, Y. Wang, R. Wang, and M. Li. &quot;CREATE: Cross-Layer Resilience Characterization and Optimization for Efficient yet Reliable Embodied AI Systems.&quot; <i>International Conference on Architectural Support for Programming Languages and Operating Systems (ASPLOS)</i>, 2026. (*Equal contribution)'
---
LLM-based embodied AI systems are increasingly deployed on resource-constrained edge platforms, where hardware faults threaten both reliability and efficiency. CREATE systematically characterizes fault sensitivity across the application, system, and circuit layers of embodied AI pipelines, and introduces complementary detection and correction techniques: fault-injection profiling that identifies the o_proj and down_proj layers as most sensitive, a lightweight anomaly-detection circuit that protects the motion planner (improving robustness from 10<sup>-7</sup> to 10<sup>-3</sup> BER), QuaRot-based weight remapping (10<sup>-7</sup> to 10<sup>-5</sup> BER), and an entropy-aware LDO for dynamic voltage scaling that cuts compute energy by 40.6%.
