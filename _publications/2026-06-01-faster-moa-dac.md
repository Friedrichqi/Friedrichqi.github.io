---
title: "Faster-MoA: Low-Latency Tree-Structured MoA Serving with Early Exit and Agent-Aware Prefill-Decode Overlap"
collection: publications
category: conferences
permalink: /publication/2026-faster-moa-dac
excerpt: 'Accelerating Mixture-of-Agents serving with a tree-structured aggregation architecture, semantic-similarity-based early exit, and agent-aware prefill-decode overlap — 10× faster inference with only ±1% accuracy variation.'
date: 2026-06-01
venue: 'DAC 2026'
paperurl: 'https://arxiv.org/abs/2512.18126'
citation: 'Z. Wang*, Y. Qi*, H. Chen, and Z. Wan. &quot;Faster-MoA: Low-Latency Tree-Structured MoA Serving with Early Exit and Agent-Aware Prefill-Decode Overlap.&quot; <i>Design Automation Conference (DAC)</i>, 2026. (*Equal contribution)'
---
Mixture-of-Agents (MoA) improves output quality by letting multiple LLM agents collaborate, but its communication-heavy workflow makes serving slow. Faster-MoA introduces a novel tree architecture for local aggregation, agent-aware overlap of the prefill and decoding stages, KV-cache management for consecutive layers, and PEFT-tuned proposers (via LLaMA-Factory) that diversify exploration directions. A semantic-similarity-based early-exit scheme prunes unnecessary inferences, achieving 10× faster serving with only ±1% accuracy variation.
