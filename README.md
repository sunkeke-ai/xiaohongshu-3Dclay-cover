# Xiaohongshu Cover Skill

一个用于生成 **3:4 小红书竖版封面** 的 Codex Skill。输入主题与标题，即可得到粉紫马卡龙配色、圆润 3D 黏土材质和清晰标题层级的封面方案。

![粉紫治愈系 3D 黏土 AI 设计工具配图](assets/pastel-clay-cover-preview.png)

> 实际结果会根据主题、文案和参考图调整；核心视觉语言保持粉紫治愈、软萌角色、卡片式构图与柔和阴影。

## 适合用来做什么

- AI 工具、学习计划、效率方法等知识型小红书首图。
- 需要统一视觉风格的系列内容。
- 把主题、主标题和副标题转成可直接生成图片的英文 Prompt。
- 生成后检查画幅、文字、层级、留白与风格一致性。
- 在环境允许时修复模糊或错误的落图文字。

## 使用方式

安装后可以直接说：

```text
Use $xiaohongshu-pastel-clay-cover to make a 3:4 Xiaohongshu cover.
主题是“早起学习计划”，主标题是“5:30 早起自律”，副标题是“我的高效晨间 routine”。
```

也可以用自然语言触发：

- 帮我做一张粉紫治愈系的小红书封面。
- 生成 3:4 的 3D 黏土风首图，标题是“周末松弛感”。
- 参考 pastel dashboard 的材质和配色，但不要复制界面。

## 工作流程

```text
主题与文案 → 画面结构 → 英文 Prompt → 图像生成 → 文字与版式质检
```

本 Skill 不绑定特定图像服务。运行环境需提供图像生成能力；如果希望中文标题更稳定，建议同时使用图像编辑或排版工具。缺少主题或主标题时，Skill 会先确认，不会自行编造具体文案。

## 安装

```bash
git clone https://github.com/sunkeke-ai/xiaohongshu-cover-skill.git
cp -R xiaohongshu-cover-skill ~/.codex/skills/xiaohongshu-pastel-clay-cover
```

重新加载 Codex Skills 后，显式调用 `$xiaohongshu-pastel-clay-cover` 即可。

## 项目结构

```text
.
├── SKILL.md
├── agents/openai.yaml
├── assets/
│   └── pastel-clay-cover-preview.png
└── references/
    ├── examples.md
    ├── prompt-guide.md
    └── resources.md
```

- `SKILL.md`：执行入口与核心规则。
- `references/prompt-guide.md`：Prompt 公式、负面约束和质检清单。
- `references/examples.md`：完整示例与主题适配。
- `references/resources.md`：外部参考及使用边界。

## 自定义与使用边界

- 修改 `SKILL.md` 中的配色、构图或文字约束，可以创建个人变体。
- 只将拥有分发权的图标、字体或模板放入 `assets/`。
- 第三方参考图仅作为风格锚点，本仓库不重新分发其图片文件。
- 发布或再分发前，请根据用途补充适用的 `LICENSE`。
