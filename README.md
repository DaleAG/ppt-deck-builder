# PPT Deck Builder

[English Version](./README.en.md)

一个可复用的 OpenClaw Skill，用于规划、撰写、重构、原型化和打磨中文 PPT / 汇报 deck。

这个 Skill 是从一次真实完整项目中抽象出来的：围绕 OpenClaw 主题，为老板和内部团队制作一套分享型 PPT。现在沉淀下来的是一套可复用的 **做 PPT 能力**。

## 这个 Skill 能解决什么问题

- 把模糊主题整理成清晰的 deck 主线
- 搭建适合老板汇报 / 内部分享的 PPT 结构
- 用案例和证据替代空泛说教
- 当 deck 跑偏时，支持用 v2 / v3 方式重构
- 产出可编辑的 HTML/CSS 幻灯片原型
- 更稳地导出 PDF，减少打印裁切问题
- 复用输入 brief 和输出模板，提高后续生产效率

## 仓库内容

- `ppt-deck-builder.skill` — 打包好的 Skill 文件
- `SKILL.md` — Skill 主入口
- `references/` — 方法论、模板、案例、导出规则

## 如何快速用起来

### 方式 A：直接使用 .skill 文件
如果你的 OpenClaw 环境支持 Skill 导入 / 分发，直接使用：

- `ppt-deck-builder.skill`

### 方式 B：直接使用 Skill 文件夹
把 Skill 目录放到你本地的 skills 目录中，再让 OpenClaw 运行时可读取它。

建议目录结构：

```
ppt-deck-builder/
├── SKILL.md
├── references/
│   ├── ppt-workflow.md
│   ├── story-architecture.md
│   ├── cases-and-evidence.md
│   ├── html-prototyping-and-export.md
│   ├── input-brief-template.md
│   ├── output-templates.md
│   └── openclaw_example.md
```

## 推荐使用路径

1. 先用 `references/input-brief-template.md` 明确任务输入
2. 用 `references/story-architecture.md` 搭建主线
3. 用 `references/cases-and-evidence.md` 整理证据和案例
4. 用 `references/output-templates.md` 搭建页面骨架
5. 如果要做 HTML 原型，再用 `references/html-prototyping-and-export.md`
6. 想看真实示例时，再看 `references/openclaw_example.md`

## 适合哪些任务

- AI / Agent 内部分享 PPT
- 老板汇报型产品 deck
- 策略 / 方案汇报
- 案例型分享 deck
- 新技术认知教育类 PPT

## 说明

- 这是一个 **通用 PPT / 汇报 deck Skill**，不是只适用于 OpenClaw 主题。
- OpenClaw 项目只作为 worked example 保留。
- 如果你的内容迭代频繁，优先用 HTML/CSS 做原型，通常比图片生成路线更稳。

## 英文文档

See [README.en.md](./README.en.md).
