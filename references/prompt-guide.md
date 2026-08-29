# Prompt 指南

需要生成图片、改写 Prompt 或诊断画面偏差时读取本文件。

## 固定风格前缀

```text
A pastel clay-rendered Xiaohongshu cover, 3:4 vertical layout, soft lavender and pink color palette, cute kawaii 3D clay style, rounded cards, soft shadows, clean background.
```

## Prompt 公式

```text
A pastel clay-rendered Xiaohongshu cover, 3:4 vertical layout, soft [主色] and [辅色] color palette, cute kawaii 3D clay style, rounded UI cards, soft long shadows, clean and airy background.

Main title in a bold rounded cute sans-serif font, exact text: "[主标题]".
Subtitle or keyword tags, exact text: "[副标题或标签]".

Center scene: [主体视觉描述，例如 a cute clay girl reading a book with a coffee cup, surrounded by tiny stars and plants].
Decorative elements: [装饰元素，例如 small rounded charts, cute icons, pastel bubbles, mini potted plant].

Composition: sparse decorative elements in the top quarter; a large high-contrast title in the upper-middle; the main clay scene in the middle; subtitle or tags in the bottom quarter. Keep text and subjects inside generous safe margins and legible at thumbnail size.

Mood: healing, soft, girly, cozy, clean. High quality, smooth matte clay texture, warm diffused lighting.
```

不需要副标题时，删除对应行，不要让模型生成占位符。

## 可选负面约束

```text
Avoid landscape or square composition, photorealism, dark horror mood, metallic surfaces, sharp edges, high-saturation neon colors, cluttered texture, hard serif or calligraphic typography, tiny unreadable text, misspelled text, cropped title, watermarks, logos, and copied app interfaces.
```

## 文案与排版策略

- 主标题通常控制在 4-10 个中文字；较长标题拆成不超过两行。
- 明确写出 `exact text`，并使用引号包住用户原文。
- 标题与背景需要显著明度或色相对比，但避免纯黑造成生硬感；深紫、莓果紫通常更协调。
- 标签建议 2-4 个，使用短词而非长句。
- 对中文生成不稳定的模型，先生成留有干净标题区的视觉底图，再在独立排版步骤中添加准确文字。

## 生成后质检

逐项检查：

1. 是否为 3:4 竖版，目标尺寸是否为 1080 x 1440。
2. 主标题是否与用户原文逐字一致，缩略图下是否仍清晰。
3. 主体是否与主题有关，是否与标题争抢视觉焦点。
4. 是否保留足够留白和安全边距。
5. 是否符合淡紫、粉色、马卡龙、哑光黏土、圆角和软阴影的风格 DNA。
6. 是否误用了音乐 App 界面、品牌 Logo、水印或参考图中的独特构图。
