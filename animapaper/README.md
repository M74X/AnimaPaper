# AnimaPaper Annotation System

## Purpose

Structured annotation system for capturing observations, hypotheses, evidence, notes, and references. Feeds automated paper generation pipelines for the AnimaLab and AnimaCore research tracks.

## ID Convention

```
{type_prefix}-{topic}-{NNN}
```

Examples: `obs-animalab-001`, `hyp-animacore-003`, `evi-animalab-012`

## Type Prefixes

| Prefix | Type        | Description                                      |
|--------|-------------|--------------------------------------------------|
| obs    | observation | Direct observations from sessions or experiments |
| hyp    | hypothesis  | Derived or testable hypotheses                   |
| evi    | evidence    | Supporting or contradicting evidence             |
| note   | note        | Working notes and action items                   |
| ref    | reference   | Papers, sources, and external references         |

## Status Flow

```
raw → reviewed → integrated
```

- **raw**: Initial capture, unverified
- **reviewed**: Checked for accuracy and completeness
- **integrated**: Incorporated into a paper draft

## Topics

- `animalab` — AnimaLab research track
- `animacore` — AnimaCore research track

Extend as needed by adding new topic directories under `animalab/` and `animacore/`.

## Directory Layout

```
animalab/animapaper/
├── README.md
├── animalab/
│   ├── observations/
│   ├── hypotheses/
│   ├── evidence/
│   ├── notes/
│   └── references/
├── animacore/
│   ├── observations/
│   ├── hypotheses/
│   ├── evidence/
│   ├── notes/
│   └── references/
└── _templates/
    ├── observation.md
    ├── hypothesis.md
    ├── evidence.md
    ├── note.md
    └── reference.md
```

## Usage

1. Copy the appropriate template from `_templates/`.
2. Assign an ID following the convention above.
3. Fill in all frontmatter fields and Markdown sections.
4. Set `status: raw` on creation; update as the entry progresses.
