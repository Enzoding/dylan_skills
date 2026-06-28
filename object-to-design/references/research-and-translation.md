# Research and Translation

## Research Inputs

Use the strongest available evidence first:

1. User-provided images, links, PDFs, notes, or product names.
2. Official product pages, manuals, press releases, store pages, support pages, and brand archives.
3. Museum/archive entries, designer interviews, credible reviews, teardown articles, product photography, and historical catalogs.
4. Image search for visual details when text sources do not reveal form, materials, labels, controls, or construction.

For current products, verify details online. For old or niche products, prefer multiple independent sources and document uncertainty.

## Source Scope

### Specific Object

Analyze the named object directly. If the object has multiple variants, use the variant the user named. If the variant is unclear but does not materially affect the design language, proceed and note the assumption.

### Product Family

Analyze 2-4 representative products in the family. Identify shared traits and meaningful variation.

### Brand-Level Source

Select 3-5 representative physical objects. Choose by:

- Design-language representativeness.
- Availability of reliable visual/source material.
- Variety across time, category, or use case.
- Transferability to digital interfaces.
- Balance between classic and contemporary objects.

Do not collapse a broad brand into generic adjectives. Use the objects as evidence.

## Evidence Discipline

Separate:

- Observed facts: visible form, layout, material, controls, labels, colors, construction, context of use.
- Inferences: design intent, interaction analogy, UI translation, emotional tone.
- Unknowns: missing, conflicting, or unverified details.

If sources conflict, mention the conflict briefly in the `Known Gaps` section of `DESIGN.md` and choose the interpretation that is best supported or most useful for UI generation.

## Translation Heuristics

Use these as effect-oriented heuristics, not rigid rules.

### Physical Controls to Digital Components

Translate knobs, switches, sliders, buttons, dials, bezels, ports, and latches into controls such as segmented controls, sliders, toggles, mode selectors, steppers, command bars, status dials, and focused input groups.

Avoid turning every physical control into decorative skeuomorphic UI. Ask what job the control performs: mode switching, precision adjustment, confirmation, safety, hierarchy, feedback, or affordance.

### Materials to Surface Systems

Translate plastic, aluminum, glass, rubber, fabric, leather, transparent shells, brushed metal, and matte coatings into surface color, contrast, border behavior, translucency, shadow restraint, texture restraint, and durability cues.

Do not paste fake material textures unless the user explicitly wants skeuomorphism.

### Construction to Layout

Translate seams, panels, grids, screws, perforations, modular parts, hinges, rails, and joinery into page structure, panel grouping, grid rhythm, card boundaries, toolbars, separators, density, and information architecture.

### Markings to Typography and Microcopy

Translate engraved labels, printed legends, scales, badges, care labels, warning labels, embroidery, and serial markings into caption systems, technical labels, metadata rows, numeric formatting, small caps, and concise status copy.

### Use Posture to Interaction Model

Translate how the object is used: handheld, workbench, outdoor, precision, performance, repair, wearable, domestic, public, or professional. Let this shape touch target size, information density, feedback strength, shortcuts, and error states.

### Aging, Repair, and Lifecycle to State Design

For objects where wear, repair, maintenance, patina, modular replacement, or sustainability matter, translate those qualities into lifecycle metadata, repair states, reversible actions, durable copy, and honest status indicators.

## Anti-Cosplay Rule

Reject shallow readings such as:

- Brand equals one color plus logo.
- Industrial design equals fake screws and texture.
- Premium equals giant whitespace and rounded cards.
- Retro equals sepia, noise, and nostalgia props.
- Outdoor equals mountains and green.
- Audio equals leather texture and knobs everywhere.
- Transparent product equals random glassmorphism.

Instead, ask: what does the physical trait do, and how can that function improve UI clarity, control, durability, feedback, or comprehension?

## Brand/IP Safety

Do not copy or embed:

- Logos, wordmarks, monograms, proprietary icons, official product photography, or official packaging art.
- Exact product silhouettes or distinctive trade dress as interface assets.
- Proprietary fonts unless the user provides a licensed font.
- Official slogans, campaign copy, app screens, advertisements, or protected artwork.

Use inspired tokens and rules instead of copied assets. The generated interface should not imply official affiliation, endorsement, or counterfeit identity.
