# Worked Example: OverBench Agent Workspace

> **Illustrative brief.** The product description, user needs, and cell count in this example are inferred design premises for demonstrating the method. They are not claims about OverBench's actual platform features or coverage. Do not reuse this subject, composition, or palette as a default for another product.

## Brief

- **Product:** OverBench, described here as an agent workspace for parallel technical work.
- **Assumed job:** let a developer start, monitor, and compare several coding agents on one project.
- **Personality:** calm, exacting, technical, and humane.
- **Audience:** developers and technical teams who value quiet control.
- **Existing identity:** none supplied for this exercise.
- **Icon constraints:** one square icon, readable at 32 px, clear on a dark field.
- **Design intent:** make parallel agent work feel like one calm work surface with clearly ordered activity.

This brief assumes three parallel work streams only because three cells make the composition legible. It is a design premise, not a feature claim.

## Three distinct concepts

### 1. Object metaphor: graphite bench plate

A thick rounded-square graphite plate with a shallow overhang along its lower edge. One continuous recessed band sits above the lip, divided into three cells by two slim ribs.

- **Rationale:** one sturdy surface holds separate active areas. Parallel work stays ordered because everything belongs to the same bench.
- **Silhouette:** a weighted rounded square with a clear lower lip and one strong horizontal recess.
- **Read at 32 px:** the plate outline and horizontal band survive; the cell dividers can be tuned for legibility.

### 2. Abstract system: continuous beam with parallel strips

One continuous beam crosses a dark opening. Three parallel light strips are set into its face at equal spacing, each at a slightly different depth.

- **Rationale:** several independent streams are carried by one structure.
- **Silhouette:** a long horizontal bar with a deliberate void beneath it.
- **Read at 32 px:** strong as a silhouette, but the open void may make the icon feel like a bridge or media control rather than a workspace.

### 3. Expressive form: operators under a canopy

Three rounded figures lean together beneath one soft canopy, suggesting a team sharing a working space.

- **Rationale:** expresses companionship and shared effort.
- **Silhouette:** a domed cluster with three rounded feet.
- **Why rejected:** it is too toy-like for the intended tone, implies social collaboration rather than parallel independent work, and asks the viewer to parse too many separate forms at small size.

These are three conceptual families, not recolors of one shape.

## Chosen direction

The graphite bench plate wins on semantic fit, scale, and restraint.

- **Hierarchy:** the plate is the single hero form. There are exactly two supporting forms: the shallow overhang lip and the continuous recessed band. The two divider ribs are details inside that band, not additional supports. The repeated cells read as one system.
- **Geometry:** the plate is centered in a square crop. The lip and band align to one horizontal axis; the band spans most of the width with generous side margins. The cell dividers are wide enough to remain visible at 32 px.
- **Materials:** one primary material, satin graphite anodized aluminum, and one secondary material, warm amber frosted glass. No third material.
- **Color:** a near-black graphite palette with one amber accent. Metal, glass, and divider ribs separate by value, not by extra hues.
- **Light:** a soft key from the upper left, restrained edge highlights on the top-left radius and lip, a quiet contact shadow, and ambient occlusion inside the band. No bloom or spectacle.

## Final prompt

```text
A desktop app icon for OverBench, an agent workspace for parallel technical work. Show one calm graphite bench plate holding a single continuous band of active work cells: parallel activity contained within one surface.

Center a thick rounded-square plate in a 1:1 frame as the only hero form. Add two supports: a shallow overhang lip across the lower edge and one recessed horizontal band above it. Two slim divider ribs split the band into three equal cells; these ribs are details within the band, not separate shapes. Keep wide margins inside a rounded-square mask and readable spacing at 32 px.

Use only two materials: satin graphite anodized aluminum for the plate and lip, and warm amber frosted glass for the band. Palette: near-black graphite with one amber accent. Keep a clear value step between dark metal, amber glass, and graphite dividers.

Light from the soft upper left. A restrained highlight follows the top-left radius and overhang lip. Give the band gentle ambient occlusion, a narrow amber inner edge and no bloom; seat the plate with a quiet contact shadow. Finish satin-matte with a low broad sheen, never glossy.

Present one centered icon on a plain dark neutral field in a clean square crop, with no device mockup. No text, numerals, people, arrows, screens, UI, extra symbols, particles, lens flare or watermark.
```

## Concept-level risk review

**No image was rendered or inspected for this example.** This is a concept-level review of the described geometry and prompt, not an assessment of a generated result. No image-based gates or scores apply.

1. **The overhang may overpower the plate.** A heavy lip could read as a separate shelf or pull too much weight toward the lower edge.
   - **Targeted instruction:** reduce the lip's visual depth relative to the plate, merge it into the plate outline, and describe its shadow as a narrow occlusion line rather than a large cast shadow. Preserve the band layout, materials, and light direction.
2. **The cells may collapse at 32 px.** Narrow dividers or a shallow band can merge into a single dark slot.
   - **Targeted instruction:** increase the band height and divider width, keep the outer margins generous, and maintain three equal cells. Do not add extra symbols or change the palette to compensate.

These are predicted risks, not observed defects. If a render exists, inspect the actual image before applying either instruction.

## What transfers

This example is a method, not a template. What carries to another product is:

- decoding the product's job and tone into one design intent;
- exploring object, abstract, and expressive families before choosing;
- keeping one hero form with at most two supports, and treating a repeated row as one system;
- limiting materials, palette, and light so geometry remains the lead;
- writing a five-block English prompt with countable forms and plain negative constraints;
- reviewing concept-level risks honestly when no image exists, and reviewing the actual image when one does.

Do not transfer the bench plate, the three-cell band, the graphite-and-amber palette, or the OverBench name to unrelated work.
