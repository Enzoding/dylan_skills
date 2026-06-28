# DESIGN.md Format

## Output Files

Default:

```text
design-md/<object-slug>/DESIGN.md
```

Use lowercase slugs with hyphens. Prefer a specific object slug such as `braun-et66` or `dyson-supersonic`. For brand-level sources, use the brand slug unless the user names a target use case.

## DESIGN.md Structure

Use a DESIGN.md-compatible document: structured tokens in frontmatter first, then markdown guidance.

Start with:

```md
---
version: alpha
name: <object-or-brand>-physical-design-analysis
description: <one dense paragraph describing the translated UI language>
source_scope:
  mode: object | product-family | brand
  objects:
    - <representative object>
colors:
typography:
rounded:
spacing:
materials:
components:
interaction_patterns:
---
```

Then include these sections:

```md
## Source Scope
## Observed Product Language
## Physical Design Principles
## Digital Translation
## Colors
## Typography
## Layout
## Materials and Surfaces
## Components
## Motion and Feedback
## Content Voice
## Brand/IP Safety
## Do's and Don'ts
## Responsive Behavior
## Agent Prompt Guide
## Known Gaps
## Sources
```

Optional sections when useful:

```md
## Physical Interaction Model
## Packaging and Labeling
## Repair and Maintenance Language
## Sound, Haptics, and Sensory Cues
## Environmental or Retail Context
```

## Token Guidance

Define tokens that downstream agents can reference directly:

- `colors`: semantic names, hex values, and roles.
- `typography`: font family fallbacks, sizes, weights, line heights, and usage.
- `rounded`: radius scale and where each value is allowed.
- `spacing`: spacing scale and layout rhythm.
- `materials`: translated surfaces such as matte plastic, brushed metal, rubber edge, transparent layer, woven fabric, or stamped label.
- `components`: buttons, cards, panels, nav, filters, inputs, selectors, status displays, data cells, and object-inspired controls.
- `interaction_patterns`: press, active, selected, disabled, focus, loading, and feedback behavior.

Use `{token.refs}` in markdown guidance when referring to tokens.

## Required Content

### Source Scope

State whether the source is an object, product family, or brand. For brand-level work, list representative objects and why they were selected.

### Observed Product Language

Describe visible and sourced product facts: form, proportion, material, color, controls, construction, typography/markings, use context, packaging, and sensory cues.

### Digital Translation

Translate observations into UI rules. Be specific enough that another agent can build components without guessing.

### Brand/IP Safety

Include explicit restrictions:

- Do not use logos, wordmarks, proprietary icons, official photos, exact silhouettes, protected slogans, official packaging art, or proprietary fonts without a license.
- Do not present the UI as official brand output.
- Use abstracted design principles, open/system fonts, and original assets.

### Agent Prompt Guide

End with concise implementation advice:

- 3-5 traits to prioritize.
- Which layout pattern to start from.
- Which components carry the source language.
- Which visual shortcuts to avoid.
- A fallback rule for uncertainty.

## Evidence Handling

Do not create a separate research file by default. Keep working notes internal, then put the useful evidence trail inside `DESIGN.md`:

- `## Source Scope`: what object, family, or representative brand objects were analyzed.
- `## Observed Product Language`: sourced observations, not speculative interpretation.
- `## Known Gaps`: uncertainty, conflicting evidence, or missing states.
- `## Sources`: concise source list with links.

## Quality Gate

Before finishing, verify:

- A downstream coding agent can directly use tokens, components, layout rules, and interaction guidance.
- The document preserves 3-5 distinctive traits from the physical source.
- Observations and inferences are separated.
- Physical traits are translated into UI structure, behavior, or information design before appearance.
- `Do's and Don'ts` block obvious shallow cosplay.
- `Brand/IP Safety` prevents use of protected assets and confusing official affiliation.
- `Known Gaps` honestly names weak evidence or missing states.
- The result would produce a UI that is meaningfully different from a generic minimal template.
