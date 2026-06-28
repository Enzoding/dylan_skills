---
name: object-to-design
description: Create AI-coding-agent-ready DESIGN.md files from physical products, product families, brand artifacts, or material design language. Use when the user asks to turn an object, industrial design reference, physical brand, appliance, device, garment, bag, tool, speaker, vehicle, furniture, packaging, or product brand such as Braun, Dyson, Nothing, Apple, Patagonia, or Marshall into a DESIGN.md/design system for digital UI generation. Also use for brand-level physical design analysis when representative objects must be selected first. This is not Google Material Design and should not trigger for generic CSS material effects alone.
---

# Object to Design

## Purpose

Turn physical product language into `DESIGN.md` files that help AI coding and design agents build better digital interfaces. Extract functional design principles from real objects, then translate them into tokens, layout rules, components, interaction patterns, and agent guardrails.

The main output is not a design essay. It is a practical design system document for downstream UI generation.

## Read Before Working

Read `references/research-and-translation.md` before researching or interpreting the object.

Read `references/design-md-format.md` before writing `DESIGN.md`.

## Default Output

Create one file unless the user requests otherwise:

```text
design-md/<object-slug>/
  DESIGN.md
```

Write to the project root only when the user explicitly says the generated `DESIGN.md` is for the current app/project.

## Workflow

1. Determine source scope: specific object, product family, or brand-level source.
2. For brand-level requests, select 3-5 representative physical objects before analysis. Prefer objects that are iconic, well documented, visually distinct, and transferable to digital UI.
3. Research online by default. User-provided images, links, PDFs, or notes take priority over web results.
4. Do research internally while working. Put only useful source scope, source links, assumptions, and uncertainty into the final `DESIGN.md`.
5. Separate observed product language from digital translation. Do not mix "what was seen" with "what it means for UI."
6. Write `DESIGN.md` using a DESIGN.md-compatible structure: YAML-like tokens first, then markdown guidance.
7. Include `Brand/IP Safety` guardrails in every `DESIGN.md`.
8. Run the quality gate from `references/design-md-format.md` before finishing.

## Core Rules

- Translate function before appearance. Prefer structural, behavioral, and information-design analogues over decorative mimicry.
- Do not create shallow brand cosplay. Avoid reducing a source to obvious colors, logos, slogans, fake textures, or surface-level nostalgia.
- Do not copy protected brand assets. Do not use logos, wordmarks, proprietary icons, exact product silhouettes, official product photography, proprietary fonts, slogans, or confusingly similar trade dress as UI assets.
- Use open/system fonts unless the user has licensed brand fonts.
- Preserve evidence discipline. Mark uncertain claims as uncertain and keep concise sources and gaps inside `DESIGN.md`.
- Optimize for downstream AI coding results: concrete tokens, component recipes, layout rules, responsive behavior, Do/Don't constraints, and an Agent Prompt Guide.

## Example Requests

```text
Use object-to-design to create a DESIGN.md from Braun ET66 for a finance dashboard.
Create a DESIGN.md from Dyson Supersonic that can guide an AI agent building a product configurator.
Generate a DESIGN.md for Patagonia Black Hole Duffel.
Use Apple as a brand-level physical source, select representative objects, then create DESIGN.md for a productivity app UI.
```
