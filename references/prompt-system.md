# Prompt System

A prompt translates a settled design decision into visible instructions. It does not rescue a missing concept. Decode the product and choose the metaphor before writing one.

## Five ordered blocks

### 1. Subject and semantic metaphor

Name the product category, the product, and the one idea the icon expresses. Make the semantics visible by describing a geometric relationship, not a mood.

- State what the shape represents and why that reading is product-specific.
- Prefer one clear metaphor over a list of associated objects.
- Do not add unsupported claims about the product, its users, or its market.

### 2. Geometry and composition

- Name the hero form and its position, scale, and proportions.
- Name at most one or two supporting forms and their roles.
- Define the dominant topology: inlay, cutout, overlap, recess, or relief.
- Specify axis, direction, spacing, and crop. Keep the icon centered unless there is a reason not to.
- State that the silhouette must remain readable at 32 px.

### 3. Palette and materials

- Use one primary material and, at most, one contrasting secondary material.
- Use one primary palette plus one accent when an accent is needed.
- Describe the value relationship between surfaces, not just their colors.
- Avoid mechanically applying a fashionable palette. Tie the choices to the product's identity.

### 4. Lighting and finish

- Choose a key-light direction and keep it consistent.
- Specify restrained edge highlights, contact shadow, and ambient occlusion where forms meet.
- State the finish: matte, satin, soft sheen, or controlled gloss.
- Do not make bloom, flare, or particles the main event.

### 5. Framing and negative constraints

- One centered icon on a quiet field, in a square 1:1 crop with generous margins.
- No text, lettering, mockups, screenshots, UI, watermarks, or extra symbols.
- Add only the negative constraints that address likely failure modes for this concept. Use plain language.

## Length and language

- Aim for **120–240 English words**. Enough to define geometry and materials; short enough to follow.
- Write every generation prompt in English, even when the explanation is in another language.
- Choose specific visible nouns and relationships over superlatives. "A shallow overhang casts a narrow occlusion line" is usable; "premium, stunning, 8K" is not.
- Avoid style-name pileups, parameter flags, camera jargon, artist names, and platform-brand shorthand. They add imitation, not direction.

## Reusable template

```text
A [product category] icon for [product]. Express [product job] as [single visual metaphor], with [visible geometric relationship] carrying the meaning.

Compose one [hero form] at [position and scale] in a square frame. [Proportions and axis.] Add [one or two supporting forms] as [role and topology]. Keep one clear silhouette and generous margins inside a rounded-square mask.

Use only [primary material] and [optional secondary material]. Palette: [primary family] with [one accent]. Maintain [specific value separation] between surfaces.

Light from [direction] with a large soft key, a restrained highlight on [surface], a contact shadow at [junction], and gentle ambient occlusion in [recess]. Finish [matte, satin, or controlled gloss].

Present one centered icon on [plain background] in a clean square crop. No text, lettering, mockup, UI, watermark, extra symbols, or [specific unwanted element].
```

Fill each bracket with a concrete decision. Remove optional clauses rather than adding filler.

## Rewrite examples

### Notes app: replace style words with geometry

**Bad**

> A premium minimal notes app icon, Apple style, glassy 3D, soft gradient, aesthetic, high detail, 8K.

This names a mood and a brand to imitate. It never decides what the icon is, how many forms it has, or how a person reads it. The result is likely a generic gradient tile.

**Better**

> An app icon for a local-first notes app, expressed as one compact graphite writing slab with a single warm paper leaf lifting at its upper-right corner. The lifted leaf is the only supporting form. The slab stays square and centered; the leaf overlaps it by one narrow vertical band, leaving a deep graphite shadow beneath. Materials are matte graphite ceramic and uncoated warm paper. Palette is graphite with bone paper and one amber accent on the lifted edge. Soft upper-left light, a restrained highlight on the paper, contact shadow beneath the leaf, subtle occlusion at the seam. Plain dark neutral background, generous margin, no text, no UI, no extra symbols.

The rewrite gives a single product-specific idea, a countable form hierarchy, a topology, two materials, one accent, and a defined light.

### Password manager: reject the category reflex

**Bad**

> Futuristic cyber security shield logo, neon blue glow, digital particles, 3D, ultra detailed, dramatic lighting.

The shield and glow are category reflexes. The prompt describes spectacle but not a distinctive silhouette, and it would fit any security product.

**Better**

> An app icon for a password manager, expressed as one thick rounded block of brushed titanium with a keyway cut through its center. The keyway is a narrow vertical slot with a small circular opening near the top; its negative space is the only supporting form. The block remains a solid, recognizable square silhouette. Materials are brushed titanium and dark enamel inside the cutout, with one cool blue accent at the deepest inner edge. Palette is silver-grey and near-black. Soft upper-left key light, low satin sheen, contact shadow in the slot, gentle occlusion at the inner rim. Plain warm-neutral background, generous margins, no text, no shield, no glow, no UI.

The second prompt makes a singular object from the product's job, keeps the form count low, and uses plain-language exclusions.

## Explore before recoloring

When asked for alternatives, change the conceptual family, structural logic, metaphor subject, or hierarchy. Do not present three recolors as three concepts. Recolor only after a direction is chosen, or when the user explicitly asks for color studies.

## Revise the actual image

A prompt is an instruction, not evidence of a result. Revise only after inspecting a real render.

- Start with a visible observation, not a taste judgment.
- Name the property to change: silhouette, spacing, crop, form count, material boundary, highlight placement, or value contrast.
- Preserve what already works. Add a constraint such as "keep the band layout and graphite material."
- Fix the two most consequential issues first. Simplify when the render looks generic.
- Use a targeted instruction such as: "The inner dividers disappear at 32 px; make the recessed band deeper and widen the two dividers while keeping the outer plate outline unchanged."
- Do not impose a fixed iteration count unless the user asks for one. Stop when the brief, hierarchy, and legibility are satisfied.

If no image exists, label the work as a concept-level review and do not imply that a render was seen or judged.

## Keep negatives readable

Write exclusions in ordinary visual language: "no text or watermarks," "no device mockup or interface elements," "no extra symbols or lens flare," "no background clutter," "no unrequested color variations." Do not use engine-specific negative-prompt syntax, parameter flags, or invocations of nonexistent tools. State what should stay out of the image plainly.

## Final pass on a prompt

Before delivering, confirm:

- The metaphor is specific to this product.
- The hero and supports are countable and limited.
- The materials and palette are constrained.
- Lighting explains form rather than adding spectacle.
- The prompt is 120–240 English words and contains no imitation shorthand.
- The language distinguishes instructions from observed results.
