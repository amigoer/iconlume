# Review Rubric

Review the work that exists. A prompt describes an intention; it is not evidence that an image was generated, exported, or visually inspected.

## Evidence and scope

- If an actual render is supplied, assess the supplied image at full size, at 32 px, and in grayscale.
- If no image is supplied, label the response **"Concept-only review (no image supplied)."** Discuss concept risks, silhouette intent, and prompt clarity, but do not assign visual scores, describe imagined details, or claim a render passed anything.
- Do not infer image quality from a prompt, a description, or an image the user only mentioned.
- Do not claim validation, export, vector conversion, trademark clearance, or production readiness without evidence.

## Six quality gates

Use these before scoring. Every answer must be **YES** for a pass.

1. **Product fit:** Does this symbol belong to this product, not merely to any AI, software, or technology product?
2. **Small-size recognition:** Is the icon recognizable at 32 px?
3. **Geometry carries the design:** Is the strongest visual feature the designed shape, not a glow, reflection, or particle effect?
4. **Intentional execution:** Are the colors, shadows, material boundaries, and crop clearly deliberate?
5. **Reference discipline:** Has the design avoided copying the exact subject of any supplied reference image?
6. **Explainable elements:** Can each major element's role be explained in one sentence?

If any gate fails, the icon is not ready. A high score in one area cannot override a failed gate.

## Six scored dimensions

Score only an actual image. Use **1, 3, or 5**; do not invent decimals, weighted averages, or a percentage. A score of **3 is the minimum acceptable level**. A complete pass requires all six gates to be YES and every dimension to be at least 3.

| Dimension           | 1                                                                          | 3                                                                                                 | 5                                                                                             |
| ------------------- | -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Product fit         | Interchangeable with an unrelated product; relies on a category cliché     | The connection to the product's job is legible at a glance                                        | The metaphor is specific and ownable; substituting another product would break the meaning    |
| Silhouette          | Depends on shading or interior detail to read; weak or fragmented at 32 px | Clear, distinct outline at 32 px with no fragile details                                          | Memorable and confident in flat black; the outline alone carries identity                     |
| Balance             | Crowded, misaligned, or visually unstable                                  | Optical center is stable; spacing and hierarchy look intentional                                  | The tension and rhythm feel precise and quiet at every size and inside the mask               |
| Color               | Competing hues, muddy values, or hierarchy that collapses in grayscale     | One primary palette plus an accent, with clear value separation                                   | Color reinforces semantics and material; restrained, distinctive, and readable without hue    |
| Material and light  | Material soup, glow used as structure, missing contact shadow              | One primary material and at most one secondary; coherent key light, contact shadow, and occlusion | Finish is plausible, highlights explain form, and the material treatment survives 32 px       |
| Craft and restraint | Visible clutter, text, artifacts, inconsistent edges, or unearned effects  | Clean edges, no obvious artifacts, and every visible element has a role                           | Nothing can be removed without losing meaning; micro-decisions remain consistent at all sizes |

## Review procedure

1. State the evidence reviewed: image present or absent, and the sizes inspected.
2. Check all six gates before discussing taste.
3. Score all six dimensions only when an image exists. If a gate fails, state that the result is not a pass even if some scores are strong.
4. Identify the **two most consequential issues**, not every minor imperfection.
5. Recommend targeted edits that change the cause. Do not prescribe a complete visual redesign when a spacing, value, or crop fix will solve the problem.
6. Do not impose a fixed iteration cap unless the user requests one. Stop when the gates pass, every dimension is at least 3, and the two priority issues are addressed or consciously accepted.

## Prioritize causes

Rank issues by consequence before visual polish.

- A defect that breaks product meaning, silhouette, or 32 px recognition outranks a subtle finish mismatch.
- Prefer a change that resolves several smaller symptoms; weak value structure may explain both muddy materials and a lost silhouette.
- Judge against the brief and the evidence, not personal taste.
- If the two priority issues share a cause, state it once and give one repair.

## Write actionable revisions

Use this structure for each priority issue:

- **Observed:** What is visible in the supplied image, at which size.
- **Target:** The specific property to change, such as silhouette, gap, form count, material boundary, highlight, or crop.
- **Preserve:** What must not drift while making the change.

Example: "Observed: at 32 px the two dividers merge, so the recessed band reads as one dark slot. Target: widen the dividers and increase the band's depth contrast. Preserve: the outer plate outline, graphite material, and amber accent."

Do not answer a structural defect with more adjectives, extra decoration, or a color change. If the concept is generic, simplify or replace the metaphor. If a new direction is required, label it as a new concept rather than a revision.

## Minimal review report

For an image review, this is enough:

```text
Evidence: supplied image; inspected at full size, 32 px, and grayscale
Gates: 6/6 pass
Scores: product fit [1/3/5]; silhouette [1/3/5]; balance [1/3/5]; color [1/3/5]; material/light [1/3/5]; craft/restraint [1/3/5]
Priority 1: Observed ... Target ... Preserve ...
Priority 2: Observed ... Target ... Preserve ...
Verdict: pass / revise
```

For a concept-only review, omit the gate result and scores, and begin with the required label. Do not substitute a prompt description for missing visual evidence.

## Report honestly

- Use **"Concept-only review (no image supplied)"** when appropriate, and omit image-based scores.
- Report only defects visible in the actual image.
- Separate observation from preference: "the lower edge is clipped by the crop" is observable; "it feels more premium in blue" is a preference.
- Do not describe an image as generated, revised, exported, or validated unless that action happened.
- Do not imply trademark safety, uniqueness, or production readiness from a visual review.
