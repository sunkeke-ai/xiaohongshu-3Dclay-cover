# 小红书粉紫治愈系 3D 黏土封面 Skill

这是一个可直接放入 GitHub 仓库分发的 Codex Skill，用于生成带标题排版的 3:4 小红书竖版封面。核心风格是粉紫马卡龙配色、圆润 3D 黏土材质、软阴影、卡片式布局和可爱角色。

## 效果展示

![粉紫治愈系 3D 黏土 AI 设计工具配图](assets/pastel-clay-cover-preview.png)

上图展示了本 Skill 所强调的粉紫马卡龙配色、圆润黏土材质、可爱角色、卡片式界面和清晰标题层级。实际生成结果会根据主题、文案和参考图调整。

## 能做什么

- 根据主题和文案设计完整的小红书首图。
- 保持粉紫治愈、软萌可爱、3D 黏土的稳定风格。
- 生成适用于图像模型的英文 Prompt。
- 在生成后检查画幅、文字、层级、留白和风格一致性。
- 在环境允许时修复模糊或错误的落图文字。

## 项目结构

```text
xiaohongshu-pastel-clay-cover/
├── SKILL.md                  # Skill 入口和核心执行规则
├── README.md                 # 面向 GitHub 访客的项目说明
├── agents/
│   └── openai.yaml          # Codex UI 元数据
├── references/
│   ├── prompt-guide.md       # Prompt 公式、负面约束和质检清单
│   ├── examples.md           # 完整示例和主题适配表
│   └── resources.md          # 外部风格参考及使用边界
└── assets/
    ├── pastel-clay-cover-preview.png # README 效果展示图
    └── README.md                    # 本地素材的放置约定
```

> 标准 Skill 入口文件名为大写 `SKILL.md`。原始需求中提到的 `skill.md` 已按规范修正。

## 安装

将整个目录克隆或复制到 Codex Skills 目录，例如：

```bash
git clone <your-repository-url>
cp -R xiaohongshu-pastel-clay-cover ~/.codex/skills/
```

重新加载 Skills 后，可自动触发，也可以显式调用：

```text
Use $xiaohongshu-pastel-clay-cover to make a 3:4 Xiaohongshu cover.
主题是“早起学习计划”，主标题是“5:30 早起自律”，副标题是“我的高效晨间 routine”。
```

## 典型触发语

- 帮我做一张粉紫治愈系的小红书封面。
- 生成 3:4 的 3D 黏土风首图，标题是“周末松弛感”。
- 参考这种 pastel dashboard 的材质和配色，但不要复制界面。

## 使用说明

本 Skill 不绑定特定图像服务。运行环境应提供可用的图像生成工具；如需稳定的中文标题，最好同时具备图像编辑或排版能力。没有主题或主标题时，Skill 会先向用户确认，不会自行编造具体文案。

第三方参考图仅作为风格锚点，仓库不重新分发其图片文件。详见 [references/resources.md](references/resources.md)。

## 发布到 GitHub

1. 新建空仓库。
2. 将本目录作为仓库根目录提交。
3. 根据你的发布策略补充 `LICENSE`；本项目未替你假定许可证。
4. 可在仓库简介中使用：`A Codex Skill for pastel 3D clay-style Xiaohongshu covers.`

## 自定义

- 修改 `SKILL.md` 中的配色、构图或文字约束可创建个人变体。
- 将你拥有分发权的图标、字体或模板放入 `assets/`，并在 `SKILL.md` 中说明何时使用。
- 不要把无授权的第三方参考图直接提交到仓库。
