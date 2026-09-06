---
title: "DySL-VLA: Efficient Vision-Language-Action Model Inference via Dynamic-Static Layer-Skipping for Robot Manipulation"
collection: publications
category: conferences
permalink: /publication/2026-dysl-vla-dac
excerpt: 'Dynamic-static layer-skipping for vision-language-action models: adaptive layer bypass based on task requirements and motion significance, with 85.7× fewer trainable parameters than full fine-tuning.'
date: 2026-06-02
venue: 'DAC 2026'
paperurl: ''
citation: 'Z. Yang, Y. Qi, T. Xie, B. Yu, S. Liu, and M. Li. &quot;DySL-VLA: Efficient Vision-Language-Action Model Inference via Dynamic-Static Layer-Skipping for Robot Manipulation.&quot; <i>Design Automation Conference (DAC)</i>, 2026.'
---
Vision-language-action (VLA) models enable generalizable robotic manipulation but are too heavy for real-time control on robots. DySL-VLA exploits the high activation similarity between adjacent VLA layers (mean ~80%) to adaptively skip layers according to task requirements and motion significance — where trajectory continuity reflects the importance of the current action. Adapters and skip controllers trained in two stages reduce trainable parameters by 85.7× versus full-parameter fine-tuning.
