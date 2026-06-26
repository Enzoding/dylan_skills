# Component Recipes

Use these recipes to build classic Braun-style UI elements. Choose only the recipes that fit the task.

## Product Panel

Use for main app surfaces, landing hero blocks, dashboards, modals, or control areas.

Traits:
- Low-radius rectangle.
- Warm white, light grey, charcoal, or matte black surface.
- Thin border or slightly darker edge.
- Clear content/control zones.
- Small equipment label in one corner.
- Optional narrow metal-like rail or bottom strip.

## Device Label

Use for section captions, metadata, active route labels, or component names.

Traits:
- Small neutral sans-serif.
- All-caps or compact title case.
- Close to the related object.
- Muted but readable.
- May include simple numbering: 01, 02, A/B, L/R, ON/OFF.

## Calculator Keys

Use for command palettes, numeric input, quick actions, mode grids, or dense button groups.

Traits:
- Equal-size buttons in a strict grid.
- Circular or low-radius square keys.
- Neutral key field with one functional accent key.
- Clear hover, pressed, disabled, and selected states.
- Tabular numbers where relevant.

Avoid using calculator keys for long text actions that need sentence labels.

## Dial or Clock Face

Use for time, progress, tuning, volume, weather, health, focus, analytics, or any circular readout.

Traits:
- Circular geometry.
- Fine tick marks.
- One clear indicator line, dot, hand, or active arc.
- Minimal labels.
- Strong center alignment.

Keep it useful: if exact adjustment matters, provide direct input or accessible controls too.

## Segmented Switch

Use for modes, filters, tabs, view changes, and binary or small-option controls.

Traits:
- Rectilinear or pill-with-low-radius track.
- Clear dividers.
- Active segment indicated by fill, lamp, notch, or accent.
- Labels close and concise.

Avoid vague icons without labels when the mode is not obvious.

## Slider with Scale

Use for parameter controls, filters, playback, generation settings, intensity, range selection.

Traits:
- Straight rail.
- Tick marks or numeric endpoints.
- Small knob or rectangular thumb.
- Current value shown as a measured readout.
- Optional accent only on active portion.

## Status Light

Use for live, syncing, recording, connected, alert, success, warning, active, or idle states.

Traits:
- Small circular lamp.
- Functional accent color.
- Label immediately beside it.
- No glow unless extremely subtle.

## Perforation Grid

Use as texture, audio motif, loading surface, decorative counterweight, or empty-state structure.

Traits:
- Even circular holes or dots.
- Strict rows and columns.
- Low contrast.
- Cropped or bounded by a product panel.

Avoid using it everywhere. One well-placed grille is stronger than repeated grilles.

## Display Window

Use for readouts, previews, current state, result panels, charts, or outputs.

Traits:
- Slightly recessed or separated area.
- High legibility.
- Tabular numeric or technical text where relevant.
- Strong contrast with surrounding panel.
- Minimal decoration.

## Module Card

Use for repeated content, dashboard widgets, features, pricing items, or settings groups.

Traits:
- More like a removable product module than a floating SaaS card.
- Aligned to a strict grid.
- Subtle edge, no heavy shadow.
- Compact label and clear value/action.
- Consistent sizing within a row or group.

## Navigation Rail

Use for app navigation or product-page section navigation.

Traits:
- Feels like a control strip.
- Compact labels.
- Active item indicated by lamp, line, fill, or notch.
- Clear separation from content faceplate.

## Implementation Notes

- Use CSS variables for palette ranges and spacing steps, but adapt values to the app.
- Prefer system fonts unless the project already has a suitable neutral sans.
- Use `font-variant-numeric: tabular-nums` for measured data.
- Use consistent border widths and radii.
- Keep shadows minimal; use border, plane changes, and spacing first.
- Make hover, focus, active, disabled, loading, and error states visible.
- Preserve accessibility: contrast, hit targets, focus rings, labels, and semantic controls.
