# Iconlume

**English** | [简体中文](README.zh-CN.md)

Premium icon art direction for app icons and product marks.

Iconlume turns a product brief into distinct visual metaphors, then into a structured English image-generation prompt. When a render exists, it critiques that actual image rather than the prompt that produced it.

## Generated examples

![Six generated app icons: Pleatnote, Stillpoint, and Dovetail on the top row; Cairn, Timbre, and Coat on the bottom row](assets/demos/gallery.webp)

_Six fictional product briefs, each rendered as an actual raster image from its accompanying prompt. Top row: Pleatnote (notes), Stillpoint (focus), Dovetail (developer tools). Bottom row: Cairn (personal finance), Timbre (audio), Coat (color grading). [Briefs and full prompts](examples/demo-icons.md)._

## Worked example

Brief: "Design an app icon for a local-first notes app."

**Directions considered:**

- **Object:** A single lifted paper leaf rests over an offset two-leaf stack, with one warm edge catching the light.
- **Abstract system:** A solid local node holds a short closed loop that never reaches the outer field, suggesting private data that stays nearby.
- **Expressive form:** A curled page with a face-like fold was rejected because its playful character does not suit a calm, durable tool.

**Chosen direction:** The lifted leaf is the hero and the two leaves beneath it form one supporting stack, creating a tactile note metaphor with a countable hierarchy, a clear action at 32 px, and no reliance on text.

**Prompt excerpt:** "One lifted paper leaf over an offset two-leaf stack, matte paper on dark ceramic, one amber accent, soft upper-left light, generous margin, plain field, no text, no UI, no mockup."

No image was generated for this worked example; it is a separate notes brief, not the Pleatnote icon in the gallery above. The [full OverBench example](examples/overbench-example.md) applies the complete method to another illustrative brief, and the [demo icons](examples/demo-icons.md) carry six different briefs through to actual renders.

## How it works

1. **Decode the product.** Infer the job, tone, audience, existing identity, and icon constraints.
2. **Choose a distinct idea.** Compare object, abstract-system, and expressive routes before selecting a direction.
3. **Constrain the geometry.** One hero form, at most two supports, one primary material plus at most one secondary, a primary palette plus one accent, and one controlled key light.
4. **Write the prompt in five blocks.** Subject and metaphor, geometry and composition, palette and materials, lighting and finish, framing and negative constraints.
5. **Review what exists.** If an image is available, judge the render and make targeted revisions. If not, keep the review at concept level and say so.

## Install

```sh
git clone https://github.com/amigoer/iconlume.git ~/.claude/skills/iconlume
```

This path is the user-level skill directory used by Claude Code. Other clients that support skill directories need the repository placed in their own skill directory. Clone the whole repository and keep `references/` beside `SKILL.md` so the linked guidance stays with the skill.

Start a new session so the client can discover the skill, then call:

```text
/iconlume Design an app icon for a local-first notes app.
```

Some clients also select skills from a natural-language request such as "design an app icon." Whether that works depends on the client, not on a separate trigger list.

Update an existing install with:

```sh
git -C ~/.claude/skills/iconlume pull --ff-only
```

Repository: [github.com/amigoer/iconlume](https://github.com/amigoer/iconlume)

## Files

- [SKILL.md](SKILL.md): workflow, handoff rules, and quality gates.
- [references/visual-language.md](references/visual-language.md): hierarchy, topology, materials, light, checks, and repairs.
- [references/prompt-system.md](references/prompt-system.md): the five-block prompt template and rewrite examples.
- [references/review-rubric.md](references/review-rubric.md): evidence rules, quality gates, and observable scoring anchors.
- [examples/overbench-example.md](examples/overbench-example.md): a full illustrative concept-to-prompt walkthrough.
- [examples/demo-icons.md](examples/demo-icons.md): briefs, individual images, and full prompts for the six generated demos.
- [assets/demos/](assets/demos/): the gallery contact sheet and the six individual demo icon images.

## Limits

- The prompt and review workflow works without image tools; rendering is an optional step.
- Renders and exports are produced only when a capable image tool is available and the user requests them.
- Generated output is raster, not a vector master.
- Trademark clearance, uniqueness checks, and legal approval are outside its scope.
- The demo product names and briefs are fictional and illustrative, not cleared brands or customer work.
