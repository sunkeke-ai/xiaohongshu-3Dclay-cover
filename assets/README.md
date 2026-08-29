# Assets

此目录用于存放拥有合法使用和再分发权的本地资源，例如：

- Skill 图标或仓库预览图；
- 圆润字体文件及其许可证；
- 可复用的背景、装饰图标或排版模板。

当前包含：

- `pastel-clay-cover-preview.png`：README 中的效果展示图，由项目提供者加入仓库。

原始 Skill 提供的第三方风格图未打包进仓库，以避免误分发。相关链接及用途说明见 `references/resources.md`。

加入资源后，请同时：

1. 保存对应许可证或来源说明；
2. 在 `SKILL.md` 中写明何时读取或使用该资源；
3. 若作为 Skill 图标，在 `agents/openai.yaml` 中使用相对路径引用。
