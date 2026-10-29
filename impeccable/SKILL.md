---
name: impeccable
description: 编码 Agent 的「设计词汇表」——24 条可执行的设计指令（bolder/quieter/distill/critique/audit…）+ 62 条确定性反-slop 规则。给 cht-ui-skill 补上「改稿动词」与客观评审闭环，克制 AI 默认审美。
source: https://github.com/pbakaus/impeccable （⭐ ~92.8k，作者 pbakaus）
---

# impeccable — 设计词汇表与反-slop 方向盘

来源：[pbakaus/impeccable](https://github.com/pbakaus/impeccable)。原文是「给编码 Agent 的设计词汇」：用**可命名的指令**代替「make it pop」这种模糊诉求，并用 62 条确定性规则在交付前拦下 AI slop。

> 定位：与 cht-ui-skill 现有的「AI 审美三件套」互补——
> - `frontend-design` 给**立场**（避开 5 大默认陷阱）
> - `taste-skill` / `garden-skills` 给**方向**（方向牌 / 风格配方）
> - **impeccable 给可执行的「改稿动词」+ 客观评审**（critique / audit），把审美从形容词变成动词

## 核心：AI 默认陷阱（slop tells）

无引导时，模型反复生成同一套：Inter 包打一切、紫→蓝渐变、卡片套卡片、彩色背景上压灰字、每个标题上方一个圆角方块图标瓦片。impeccable 用 **62 条确定性规则**无 LLM、无 API key 地标记这些 tell，外加 cramped padding、跳级标题等质量问题。规则配置见 `assets/detector-config.json`。

## 24 条指令（分组）

| 组 | 指令 | 语义 |
|----|------|------|
| **Steer 把控** | `bolder` | 放大稳妥的设计 |
| | `quieter` | 压低过响的设计 |
| | `distill` | 删掉页面不需要的东西 |
| | `colorize` | 给灰界面注入色彩 |
| | `typeset` | 修字体、层级、字号 |
| | `layout` | 修间距与节奏 |
| | `animate` | 加过渡与交互反馈 |
| | `delight` | 加个性 |
| | `overdrive` | 上 shader、弹簧物理、滚动驱动特效 |
| **Review 评审** | `critique` | 打分制 UX 评审，排出先修项 |
| | `audit` | 技术质量报告（无障碍 / 性能 / 主题 / 响应式），P0–P3 排序 |
| **Finish 收尾** | `polish` | 上线前最后一遍 |
| | `harden` | 错误 / i18n / 溢出 / 边界情况 |
| | `clarify` | 重写不清的文案 |
| | `adapt` | 屏幕尺寸与设备 |
| | `optimize` | 加载与渲染性能 |
| | `onboard` | 首次流程与空态 |
| **Iterate live 实时迭代** | `live` | 浏览器里选元素、循环变体 |
| | `generate` | 无需手选，生成命名元素的变体 |
| **Plan & setup 规划与初始化** | `shape` | 编码前规划 UX |
| | `init` | 写 `PRODUCT.md`（产品是谁/要做什么/约束） |
| | `document` | 写 `DESIGN.md`（捕获既有视觉系统，保持品牌一致） |
| | `extract` | 把重复模式抽成设计系统 |

第 24 条 `craft` 为普通 build 请求的废弃别名。

## 在 cht-ui-skill 里怎么用

1. **定调阶段**：读 `references/README.md`（24 指令全表）与 `references/DESIGN.md`（设计系统参考），挑一个**窄目标**（单个 section / 组件）比整页泛审效果更好。
2. **改稿阶段**：把指令当动词下达，例如「`bolder` 定价卡片」「`quieter` 落地页」「`polish` 设置页」「`critique` 注册流程」。
3. **评审闭环**：交付前跑一遍 `critique`（UX 排序）+ `audit`（P0–P3 技术质量），按 P0 先修。可对照 `assets/detector-config.json` 的 62 条规则自检 slop。
4. **品牌一致**：若项目已有视觉系统，先 `document` 落在 `DESIGN.md`，改动保持 on-brand。

## 深度参考

- `references/` — README（24 指令）、DESIGN.md、STYLE.md、PRODUCT.md、NOTICE.md
- `assets/design-system.json` — 设计 token（含 kinpaku 暗色系统：金箔金 / 铜绿锈 / 漆黑底）
- `assets/detector-config.json` — slop 检测器规则配置

> 注：上游完整引擎为 Rust CLI（`npx impeccable install`，含实时变体叠加 / 设计钩子自动检查），本目录为**参考型嫁接**，只收录人读词汇与规则文档，不运行时依赖。
