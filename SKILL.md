---
name: xiaohongshu-pastel-clay-cover
description: Create complete 3:4 Xiaohongshu cover images with readable title layouts in a soft lavender-pink, kawaii 3D clay style. Use for Xiaohongshu covers, first images, or social graphics when the user asks for pastel, healing, cute, clay, macaron, girly, or soft dashboard-like visuals.
metadata:
  short-description: Create pastel 3D clay Xiaohongshu covers
---

# Xiaohongshu Pastel Clay Cover

Create a finished 3:4 vertical cover with the main title, optional subtitle, and optional tags already composed into the image. Preserve the user's topic and wording.

## Required visual DNA

- Use lavender as the primary color, supported by soft pink, cream yellow, mint, or baby blue.
- Render objects as matte 3D clay or soft plasticine with rounded edges and soft, long shadows.
- Favor rounded cards, bubbles, stars, hearts, tiny plants, friendly clay characters, and simple icons.
- Keep the mood healing, relaxed, sweet, clean, warm, and airy.
- Use rounded, cute sans-serif typography with strong thumbnail-scale contrast.
- Avoid dark or horror aesthetics, photorealism, metallic surfaces, neon saturation, sharp geometry, and busy textures.

## Output requirements

- Aspect ratio: 3:4 vertical; target 1080 x 1440 when the tool accepts dimensions.
- Top quarter: sparse decorative elements that establish the mood.
- Upper-middle third: large, clearly readable main title.
- Middle quarter: the clay character, scene, or rounded information card.
- Bottom quarter: subtitle, keyword tags, or a short action phrase.
- Keep all important text and subjects inside safe margins and legible at thumbnail size.

## Workflow

1. Extract the topic, exact main title, optional subtitle or 2-4 tags, and any reference image. If the topic or title is missing, ask for it instead of inventing specific copy. Main titles usually work best at 4-10 Chinese characters or one to two short English lines.
2. Choose a topic-aligned clay scene:
   - Learning: character reading, notebook, coffee, lamp, checklist.
   - Beauty or fashion: mirror, cosmetics, clothes rack, handbag.
   - Lifestyle: tea, room organization, cooking, or a cat.
   - Abstract topic: rounded infographic cards, expressive icons, and decorative shapes.
3. Build the generation prompt with the formula in [references/prompt-guide.md](references/prompt-guide.md). If a reference image is supplied and the available image tool supports references, use it only as a style anchor.
4. Generate with an available image-generation tool that supports a vertical canvas. Do not depend on any platform-specific tool name.
5. Inspect the result for aspect ratio, title accuracy and clarity, visual hierarchy, safe margins, topic relevance, and consistency with the visual DNA.
6. If generated text is incorrect or blurry, use an available image-editing or typography tool to repair the text region. When reliable text rendering is unavailable, generate the artwork with a clean title-safe area, then add the exact text in a separate layout pass if the environment permits.
7. Return the finished cover and briefly note any limitation that could not be corrected.

## References

- Read [references/prompt-guide.md](references/prompt-guide.md) when drafting the image prompt or negative constraints.
- Read [references/examples.md](references/examples.md) for a complete learning-themed example and adaptation patterns.
- Read [references/resources.md](references/resources.md) before using the original external style references.

## Non-negotiable checks

- Do not return a square or landscape image.
- Do not paraphrase user-provided title text without permission.
- Do not copy the reference image's music-app dashboard content; borrow only its palette, material, softness, and rounded component language.
- Treat reference images as inspiration, not as permission to reproduce copyrighted composition, logos, characters, or interface content.
