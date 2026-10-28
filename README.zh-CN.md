# Iconlume

[English](README.md) | **简体中文**

为 App 图标与产品标识提供高品质的图标艺术指导。

![带有一道琥珀色玻璃切缝的石墨色方板](assets/readme/hero.svg)

_概念习作：一道光切过石墨色方板。矢量几何，不是生成的图标。_

Iconlume 是一个纯文档 skill：它把具体的产品简介转化为不同的视觉隐喻，再写成结构化的英文图像生成提示词；有实际渲染图时，它评审图像本身，而不是凭提示词想象结果。

## 示例

需求：“为一个本地优先的笔记应用设计 App 图标。”

**考虑过的方向：**

- **物件：** 一张被掀起的纸页盖在错位的两张纸页上，一道暖色边缘接住光。
- **抽象系统：** 实心的本地节点连出一小段闭合回路，回路不延伸到外部区域，暗示数据留在本地。
- **表现性形态：** 卷起、带有类似面部折痕的纸页因语气过于俏皮而被放弃。

**选定方向：** 掀起的纸页是主形态，下面两张纸页构成一个辅助纸叠，形成有触感、层级清楚、在小尺寸下仍有明确动作且不依赖文字的笔记隐喻。

**提示词节选：** "One lifted paper leaf over an offset two-leaf stack, matte paper on dark ceramic, one amber accent, soft upper-left light, generous margin, plain field, no text, no UI, no mockup."

本示例未生成图片；若有渲染图，应评审实际图像。完整方法与另一份说明性简报见 [OverBench 示例](examples/overbench-example.md)。

## 工作方式

1. **解读产品。** 推断产品用途、语气、受众、既有识别和图标约束。
2. **选出不同的概念。** 先比较物件、抽象系统与表现性形态三条路线，再确定方向。
3. **约束几何。** 一个主形态，最多两个辅助形态；一种主材质，最多一种辅助材质；一个主色系，最多一个强调色；一个受控的主光源。
4. **按五个区块写提示词。** 主体与语义隐喻、几何与构图、色彩与材质、光照与质感、取景与负面约束。
5. **只评审已有内容。** 有图像时评审实际渲染图并做针对性修改；没有图像时明确标注为概念层面的评审。

## 安装

```sh
git clone https://github.com/amigoer/iconlume.git ~/.claude/skills/iconlume
```

这个路径是 Claude Code 使用的用户级 skill 目录。其他支持 skill 目录的客户端，需要把仓库放进各自的 skill 目录。请克隆整个仓库，并让 `references/` 与 `SKILL.md` 保持同级，以便链接的指导文件随 skill 一起保留。

新建会话让客户端发现该 skill，然后调用：

```text
/iconlume Design an app icon for a local-first notes app.
```

有些客户端也能从“设计一个 App 图标”这样的自然语言请求中选择该 skill；是否生效取决于客户端，并不存在单独的触发词清单。

更新已有安装：

```sh
git -C ~/.claude/skills/iconlume pull --ff-only
```

仓库：[github.com/amigoer/iconlume](https://github.com/amigoer/iconlume)

## 文件

- [SKILL.md](SKILL.md)：工作流、交付规则与质量门槛。
- [references/visual-language.md](references/visual-language.md)：层级、结构关系、材质、光照、检查与修正。
- [references/prompt-system.md](references/prompt-system.md)：五区块提示词模板与改写示例。
- [references/review-rubric.md](references/review-rubric.md)：证据规则、质量门槛与可观察的评分锚点。
- [examples/overbench-example.md](examples/overbench-example.md)：从概念到提示词的完整说明性示例。
- [assets/readme/hero.svg](assets/readme/hero.svg)：上方展示的矢量概念习作。

## 使用边界

- 提示词与评审流程是纯文本，无需图像工具。
- 只有客户端具备可用工具且用户明确提出时，才会生成渲染图或导出文件。
- 图像模型的输出是位图，不是矢量母版。
- 不负责商标检索、唯一性检查或法律确认。
- 上方 hero 是概念习作，不是其他产品的默认主体或配色。
