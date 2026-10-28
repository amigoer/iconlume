# Visual Language

This is a working grammar for original app icons. It is not a style preset, a fixed palette, or a library of approved subjects.

## Product semantics come first

- Begin with what the product lets a person do, not with a shape that looks premium.
- Write the design intent in one sentence: "This icon should make [product job] feel [brand quality] through [visual idea]."
- Every major form must have a job. If its job is only decoration, remove it.
- Distinguish inferred positioning from supplied facts. Never invent market claims, awards, or proprietary features.

## Silhouette carries the identity

The silhouette is the icon's memory. It must still say something when color, material, and lighting are removed.

- Test the shape as one flat black form on white. If it becomes an unreadable blob, the concept is not finished.
- Prefer one compact, confident outline over several weak fragments.
- Keep the outline distinct from category defaults. A generic shield, cloud, speech bubble, or gear needs a product-specific structural reason.
- Preserve a recognizable mark's essential geometry when modernizing it. A new material treatment is not permission to erase brand recognition.
- Judge the silhouette at 32 px before adding interior detail.

## Build a clear hierarchy

Use **one hero form** and **at most one or two supporting forms**.

- The hero establishes the silhouette and the main meaning.
- Supports may act as a base, frame, lip, inset, counterform, or single repeated system. They must clarify the hero, not compete with it.
- A repeated row or band counts as one supporting form when it reads as one continuous system. Dividers inside that system are details.
- If three or more independent shapes demand attention, reduce them or combine them into a single system.
- Be able to explain each major element's role in one sentence.

## Use topology deliberately

The relationship between forms is part of the idea. Choose one dominant structural move and make it unambiguous.

| Move    | What it does                                                    | Common failure                                                       |
| ------- | --------------------------------------------------------------- | -------------------------------------------------------------------- |
| Inlay   | Places one material inside another; signals precision and craft | The inlay floats, has no seating depth, or reads as a painted stripe |
| Cutout  | Uses negative space to reveal the field or an inner layer       | The hole becomes a second unrelated symbol                           |
| Overlap | Creates depth through a clear front/back order                  | Layers merge because their values are too close                      |
| Recess  | Sets a support below the primary surface                        | The recess reads as a flat decal without occlusion or edge behavior  |
| Relief  | Raises a form above the hero                                    | The relief adds clutter without explaining the product               |

One topology should dominate. A hero with an inlay, a cutout, and a floating overlap usually needs simplification.

## Limit materials

Choose **one primary material** and **at most one contrasting secondary material**.

- The primary material defines the icon's character: for example ceramic, satin polymer, anodized metal, or dark glass.
- The secondary material should mark one meaningful distinction, such as an active cell, a cutting edge, or a transparent layer.
- State how the materials differ in value, roughness, and edge treatment. Do not rely on texture noise alone.
- Keep material boundaries crisp and physically plausible. If the viewer cannot tell where one material ends, the separation has failed.
- Soft 3D is allowed. Material soup, random bevels, and glossy noise are not.

## Control color

Use **one primary palette plus one accent** when an accent is needed.

- Derive the palette from the product's identity and category, not from a fashionable default.
- Establish strong value separation before choosing hue. The icon must work as a grayscale composition.
- Give the accent a specific role: active state, energy, a sealed edge, or a focal detail.
- Keep the number of competing hues small. A restrained range with precise transitions reads richer than many unrelated colors.
- Do not use a purple gradient as a substitute for a concept.

## Balance optically

Geometric centering is only the starting point. Balance the perceived weight of forms.

- Give dense or dark masses more space than light ones.
- Keep margins generous inside the square crop; a bold mark can still feel crowded.
- Align repeated elements to a shared axis or a deliberate rhythm. Uneven spacing should look intentional.
- Adjust oversized circles and diagonals for optical overshoot where needed.
- Ensure the visual center of mass is stable. A top-heavy silhouette needs a counterweight, not a larger shadow.
- Check that the icon still makes sense under a rounded-square mask.

## Light and shadow explain form

Use a large, soft key light, restrained edge highlights, real contact shadows, and soft ambient occlusion.

- Pick one key direction, usually readable from the upper left. Keep secondary light weak and secondary.
- Use edge highlights only where a surface turns toward the light. Do not outline every edge.
- Add contact shadow where a form meets another surface, and ambient occlusion in recesses. This is what makes the topology believable.
- Keep reflections broad and controlled. A single small specular event can be enough.
- The strongest visual feature must be designed geometry, not bloom, flare, or glow. Lighting should reveal the shape, not become the concept.
- Avoid spectacle that disappears at 32 px or distracts from the product meaning.

## Test legibility

- **Grayscale check:** remove color. The hierarchy, material separation, and silhouette must survive.
- **32 px check:** inspect at the actual small size, not a zoomed-out large render. Remove details that become specks or disappear.
- **Flat check:** fill the silhouette with black. Confirm the idea remains recognizable.
- **Count check:** count the hero and supports. If the answer exceeds three visible forms, simplify.
- **Crop check:** view through a rounded-square mask. Confirm no essential form or highlight is clipped.
- **Background check:** test against light and dark neutral fields when the brief requires it.

## Keep presentation clean

- Show one icon on a quiet field. No device mockup, desktop scene, poster layout, or explanatory UI.
- Do not include text, lettering, numerals, watermarks, decorative labels, or screenshots in the icon.
- Do not add a logo lockup unless the user explicitly asks for one.
- Distinguish concept studies from generated icon renders and from vector production files.

## Avoid stock motifs by default

Eyeballs, vinyl records, robot heads, sparks, brain shapes, hexagons, generic gradient swirls, and letter monograms are defaults to avoid, not permanent bans. They are allowed only when the product's meaning makes them the clearest original choice and the silhouette is not a category cliché. If you use one, state the semantic reason in one sentence.

Study references for composition, proportion, material, and finish. Do not copy the depicted subject unless the user explicitly asks.

## Repair defects with targeted changes

| Defect                          | Target the cause | Repair                                                                             |
| ------------------------------- | ---------------- | ---------------------------------------------------------------------------------- |
| Shape could belong to any app   | Product fit      | Replace the metaphor or restructure the silhouette around the product's actual job |
| Hero is unclear                 | Hierarchy        | Remove or merge supports; increase the hero's relative scale                       |
| Too many supports               | Restraint        | Combine repeated elements into one band, recess, or frame; delete the rest         |
| Shape is unreadable at 32 px    | Legibility       | Enlarge the dominant feature, cut thin lines, remove tiny details                  |
| Silhouette disappears in black  | Silhouette       | Rework the outline before changing materials or lighting                           |
| Colors are muddy                | Separation       | Simplify the palette and widen value contrast                                      |
| Materials look pasted on        | Topology         | Add seating depth, edge behavior, contact shadow, and occlusion                    |
| Glow dominates the design       | Restraint        | Reduce bloom and speculars; let the geometry carry the image                       |
| Overlap is ambiguous            | Depth order      | Introduce a clear seam, counterform, or value break                                |
| Composition feels top-heavy     | Optical balance  | Shift mass, adjust crop, or add a quiet counterweight                              |
| Form feels generic              | Semantics        | Change the conceptual family, not just the color scheme                            |
| Reference is copied too closely | Originality      | Change the subject and topology, not only the angle or palette                     |

Before delivery, confirm the design answers the product brief, survives grayscale and 32 px, and has no element that cannot be explained.
