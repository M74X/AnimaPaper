---
id: obs-animalab-002
type: observation
topic: animalab
date: 2026-04-05
tags: [benchmarks, protocol-adherence, multi-model, mistral, paper-1.1]
status: raw
target_paper: animalab-paper-1.1
related: [obs-animalab-001]
---

## Observation

Mistral Vibe (devstral-small) shows consistent protocol violations in AnimaLab
Day 07R Block 0 Review session. Pattern: model acts as code reviewer, not
inductive tutor. Gives answers and code before student attempts.

## Evidence

- Violation #1: Asked student what day the session was instead of starting
  Recap Quiz directly.
- Violation #2: Asked student to choose the mini-challenge instead of selecting
  one as tutor.
- Violation #3: Showed code snippets in Recap Quiz instead of asking
  conceptually first.
- Violation #4 (critical): Provided complete starter code before student
  attempted implementation.

Session terminated at Gate 1 / mini-challenge start. Gates 3 and 5 not
reached — pattern was already conclusive.

## Derived hypothesis

Mistral ranks below Gemini on protocol adherence. Preliminary ranking:
Qwen > Claude > Gemini > Mistral on restrictive pedagogical protocol adherence.

## Notes for paper

- 4 violations vs Gemini 1 violation vs Qwen 0 violations.
- Mistral pattern: "code reviewer" mode, not "inductive tutor" mode.
- Supports obs-animalab-001 hypothesis: models optimized for immediate
  helpfulness fail restrictive pedagogical protocols systematically.
- Next data point needed: Codex CLI evaluation.
