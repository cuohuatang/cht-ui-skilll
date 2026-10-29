---
name: json-render
display_name: "json-render 生成式 UI 框架（参考型嫁接）"
description: "Vercel 出品的 Generative UI 框架（Apache-2.0）。核心方法论：定义 catalog（组件/动作/数据绑定护栏）→ AI 生成受约束的 JSON Spec → renderer 流式渲染。本目录为 cht-ui-skill 的参考型子资产，收录 packages/core（catalog/spec 模型灵魂）、packages/react（主流渲染器）、skills/（30 个 agent 子技能）、examples/chat（最小可运行示例）。"
source: vercel-labs/json-render
source_license: Apache-2.0
source_stars: 18800
graft_type: reference
---

# json-render —— 生成式 UI 框架（嫁接参考）

> 上游来源：[vercel-labs/json-render](https://github.com/vercel-labs/json-render)（**Apache-2.0**，⭐ ~18.8k）。
> 本目录是 **cht-ui-skill 的参考型子资产**——精选收录、保留上游 LICENSE 与归属、不修改上游源码。要落地工程请从上游 `npm install` 安装，本目录是「方法论文档 + 模型参考」。

## 一、它解决什么问题

普通「AI 生成 UI」容易失控：模型随便编组件、样式不可预测、输出无法校验。json-render 的解法是**护栏（guardrails）**：

> 你先声明 **catalog**（允许出现的组件、动作、数据绑定、可见性、校验），AI 只能在这个范围内生成**结构化的 JSON Spec**，再由 **renderer** 把它流式渲染成真实 UI。

结果：AI 输出永远是你 catalog 的子集 → **可预测、可校验、可回放、失败可降级**。覆盖 React、React Native、Vue、Svelte、Solid、React Three Fiber（3D / 高斯溅射）、react-email（邮件）、react-pdf（PDF）、Ink（终端）、Next.js。

## 二、核心心智模型

```
                  ┌─────────────┐
   你定义 ──────▶ │   catalog   │  (组件 / 动作 / 数据绑定 / visibility / validation 护栏)
                  └──────┬──────┘
                         │ AI 只能在此范围内生成
                         ▼
                  ┌─────────────┐
   prompt ──────▶ │ JSON Spec   │  (受约束的结构化 UI 描述)
                  └──────┬──────┘
                         │ renderer 流式渲染
                         ▼
                  ┌─────────────┐
                  │   真实 UI    │  (React/RN/Vue/Svelte/Solid/R3F/email/pdf/ink)
                  └─────────────┘
```

- **catalog**：能力的"白名单"与"护栏"。不声明的能力，AI 生成出来也会被拒绝/忽略。
- **spec / JEV（JSON Evaluation）**：AI 产出的受约束 JSON，描述要渲染什么、绑定什么数据、触发什么动作。
- **renderer**：把 spec 变成真实组件的渲染器（如 `@json-render/react`）。
- **actions / data bindings**：spec 里可声明"点击调用某动作 / 绑定某数据源"，renderer 负责接线。

## 三、本目录收录（精选，非整仓）

| 路径 | 内容 | 用途 |
|---|---|---|
| `README.md` / `AGENTS.md` / `CHANGELOG.md` / `LICENSE` | 上游总览、agent 用法说明、变更、Apache-2.0 许可 | 入门与合规 |
| `packages/core/` | **catalog / spec / visibility / actions / validation / state 模型**（灵魂），含 `src/` 源码与 README | 理解"护栏 + 受约束生成"的核心 |
| `packages/react/` | **React 渲染器**（`@json-render/react`），主流落地 | 把 spec 渲染成 React UI |
| `skills/`（30 个子技能） | `core`、`react`、`mcp`、`next`、`react-native`、`react-three-fiber`、`json-render-shadcn`、`image`、`ink`、`react-email`、`react-pdf`、`shadcn(-svelte)`、`solid`、`svelte`、`vue`、`remotion`、`xstate`、`zustand`、`jotai`、`redux`、`tanstack-start`、`yaml`、`directives`、`devtools*` 等 | agent 子技能：让 agent 用 json-render 设计/生成受控 UI 的方法论 |
| `examples/chat/` | 最小可运行示例：AI 聊天 + json-render 生成式 UI（含 `lib/render`、`lib/tools`、`components/ui`） | 阅读 catalog/spec/renderer 的实战用法 |

> 未收录：`packages/` 其余 36 个包、`apps/`、`examples/` 其余 23 个（整仓约 14M）。示例 `chat` 作为**阅读参考**——它依赖 monorepo 其它包（`typescript-config`/`shadcn` 等），独立 `pnpm install` 后才能运行，本目录重在演示 catalog/spec 写法。

## 四、怎么读（渐进披露路由）

- **先读**：本文件 + `../README.md`（`json-render/` 根README 的上游总览）→ 建立 catalog→spec→renderer 心智。
- **模型灵魂**：`packages/core/README.md` + `packages/core/src/`（catalog、visibility、actions、validation、state 的定义与示例）。
- **渲染落地**：`packages/react/src/`（`@json-render/react` 渲染器实现）。
- **agent 子技能**：按目标框架读 `skills/<framework>/SKILL.md`（如 `skills/react`、`skills/next`、`skills/react-three-fiber`、`skills/mcp`）。
- **实战示例**：`examples/chat/lib/render`（spec→UI）、`examples/chat/lib/tools`（catalog 里的动作）、`examples/chat/components/ui`（被 catalog 声明的组件）。

## 五、何时用 / 不用

**用：**
- 要让 AI 生成界面，但**必须可靠、可校验、不跑偏**（如 AI 聊天助手、AI dashboard、AI 表单/报告生成器）。
- 要在多端（React / RN / Vue / Svelte / Solid / 3D / 邮件 / PDF / 终端）用**同一套生成范式**产出 UI。
- 需要"生成结果可回放、可降级、可被 visibility/validation 约束"。

**不用：**
- 纯静态、人工写死的设计稿（走 oil-ui / draw-ui / m3e-canvas）。
- 不需要 AI 参与的常规组件开发（走 Chakra UI / 第 8 项）。
- 把 json-render 当"无约束的自由 UI 生成器"——这违背它的核心价值（护栏）。

## 六、与 cht-ui-skill 其它能力的关系

- 补上 **"AI 驱动但可靠"** 这一层：把"AI 生成界面"从自由发散收敛为受控输出。
- 与 `oil-ui`（定方向）、`design-to-motion`（出展示片）、`impeccable × jakubkrehel-skills`（交付前评审）串联成 **「设计 → 生成式落地 → 动效展示 → 客观评审」** 闭环。
- 触发总入口见 `../SKILL.md`（第 20 项、`json-render/SKILL.md`）。

## 七、合规与归属

- 全部内容版权归 **Vercel Labs**，以 **Apache-2.0** 许可再分发（见 `LICENSE`）。
- 本目录仅作**方法论文档与模型参考**的精选嫁接；商业/工程落地请从上游仓库安装对应 npm 包并遵循其许可。
