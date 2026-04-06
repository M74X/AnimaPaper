---
id: obs-animalab-001
type: observation
topic: animalab
date: 2026-04-05
tags: [benchmarks, protocol-adherence, multi-model, pedagogy, paper-1.1]
status: raw
target_paper: animalab-paper-1.1
related: []
---

## Observation

Standard benchmarks (MMLU etc.) measure speed to correct answer, not adherence
to pedagogical protocol. A model that gives the direct answer scores perfectly on
benchmarks but commits a protocol violation in AnimaLab. These are orthogonal
objectives.

## Evidence

- Day 07R Gemini: protocol violation — showed code directly, skipped student prediction.
- Day 07R Qwen: zero violations through Gate 4 — guided with questions, respected protocol.
- Pattern: Claude and Qwen show higher adherence to restrictive protocols than Gemini and ChatGPT.

## Derived hypothesis

Models optimized for "fast useful" have worse calibration for "contextually useful."
Protocol adherence under restrictive constraint is a separate evaluative dimension
from general helpfulness.

## Notes for paper

- New evaluation dimension: protocol-adherence under restrictive constraint.
- Proposed section: "Benchmark Limitations for Pedagogical LLM Evaluation."
- Needs: Mistral data point + more Gemini/ChatGPT sessions to strengthen pattern.
