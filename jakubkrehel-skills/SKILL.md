---
name: jakubkrehel-skills
description: 一套面向「界面评审 / 打磨 / 无障碍」的 agent 技能集合（14 个），覆盖 accessibility、layout、typography、colors、writing、UI polish、组件状态机/变体/拆解。适合在出稿或出码之后做证据驱动的精修与评审。
source: https://github.com/jakubkrehel/skills （⭐ ~9k，作者 jakub.kr / Interfaces 杂志）
---

# jakubkrehel-skills — 界面评审与打磨套件

来源：[jakubkrehel/skills](https://github.com/jakubkrehel/skills)。14 个纯 agent 技能，每个都是带 `SKILL.md` 的独立子技能，统一收录在 `skills/` 下。**本目录是路由索引**，真正的方法论在各自的 `skills/<name>/SKILL.md`。

> 定位：cht-ui-skill 在「出稿 / 出码」之后的**评审与精修**环节偏薄（taste-skill 偏方向、garden-skills 偏配方）。这套正好补上 accessibility / typography / colors / layout / writing 的落地打磨，外加组件级工程技能（state-machine / variant / break / teardown）。

## 14 个子技能

| 子技能 | 作用 | 触发场景 |
|--------|------|---------|
| `better-interface` | 跨域总评审（无障碍/布局/文案/字体/色彩/打磨），汇成一份排序报告 | 评审一屏、一条流、整个界面 |
| `better-ui` | 打磨表面、图标与动效（圆角/光学对齐/阴影/图标状态/动画精确值） | 视觉精修 |
| `better-typography` | 字号阶梯、间距、字体特性、换行/截断/标点 | 文本渲染审查 |
| `better-colors` | 生成调色板、命名语义 token、格式互转、对比度测量 | 色彩系统 |
| `better-accessibility` | 键盘/焦点、ARIA、可访问名、表单、屏幕阅读器播报、动效、缩放（对照 WCAG 2.2） | 无障碍 |
| `better-layout` | 分组/对齐/阅读顺序/响应式结构/翻译留白 | 布局 |
| `better-writing` | 界面文案（标签/错误/空态/确认），贴合产品语气并指明下一步 | 文案 |
| `interface-review` | 评审分支 / PR / 未提交改动引入或回归的界面问题 | 变更评审（用户触发） |
| `explain-interface` | 从在线 URL 或截图解释网站/特效/动画的实现方式 | 逆向学习 |
| `break` | 在临时页把所选组件置于每种可达场景做压力测试 | 边界测试 |
| `build-design` | 从 Figma 或设计图构建 UI，贴合设计、复用项目 token 与组件 | 设计转码 |
| `teardown` | 生成技术插画并可配置/上色/导出 SVG·PNG·PDF | 图解 |
| `state-machine` | 在临时页渲染组件每个状态，带 mock 数据与切换器 | 状态覆盖 |
| `variant` | 构建所选组件的多个变体并迭代挑选 | 变体迭代 |

## 使用约定

- **编排归属**：`better-interface` 只做跨域编排，把各领域证据交给对应 `better-*`；变更评审交给 `interface-review`。
- **证据而非品味**：报告门槛是「有证据」；`Approve` 的门槛是「你真检查了你声称检查过的东西」。风格偏好不算 finding，触发式失败（无论风格指南怎么说）才算。
- **先定范围再判断**：先推断屏/流/仓库范围并写明，覆盖空/加载/错误/窄宽状态；范围过大则收窄到一条完整流，绝不暗示未检查的面已被评审。
- **用项目自己的语言写修复**：先 recon 框架、样式系统、组件库、token、视口、预览命令；所有修复用项目自身惯用法，而非要求换栈。

## 路由到主技能

进入 cht-ui-skill 主 `SKILL.md` 后，凡涉及「已出稿/已出码界面的评审、打磨、无障碍、文案、字体、色彩、布局」类任务，路由到本目录对应子技能。
