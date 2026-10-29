---
name: cht-ui-skill
display_name: "CHT 前端视觉与动效技能集"
display_name_en: "CHT UI Skills"
description: "一站式前端视觉与动效技能集，融合 19 大能力：p5.js 创意编码、CSS Doodle 图案生成、Theatre.js 时间轴编排、React Spring 物理动画、Inure 精致微交互、UI-UX Craft 设计规范工艺、React PostFX 后期特效、Chakra UI 组件系统、oil-ui 界面设计/改版/评审、draw-ui 设计稿生成与截图还原、m3e-canvas 可拖拽 UI 设计、superpowers 开发方法论（头脑风暴/计划/TDD/调试/验证/评审）、frontend-design 设计哲学（Anthropic 官方，反 AI 默认陷阱）、taste-skill 研究方向引擎（脚本发牌 + 反 slop 实测）、garden-skills 风格配方库（25 种风格 + 6 技能）、ai-design-skills 设计演示与转化引擎（design-to-motion 静态设计稿→像素级 HTML 复刻并导出 MP4/GIF 展示片、landing-page-design 高转化落地页完整系统）、impeccable 设计词汇表与反-slop 方向盘（24 条改稿指令 + 62 条确定性反-slop 规则 + critique/audit 评审）、jakubkrehel-skills 界面评审打磨套件（14 子技能：better-interface/accessibility/typography/colors/layout/writing/ui、interface-review、state-machine、variant、break 等）、json-render 生成式 UI 框架（vercel-labs，⭐~18.8k，Apache-2.0：catalog 护栏约束下 AI 生成受控 JSON Spec → renderer 流式渲染，覆盖 React/RN/Vue/Svelte/Solid/3D/邮件/PDF/终端）。按任务路由到对应分册。"
description_zh: "cht-ui-skill：前端视觉/动效/设计/工程/审美全家桶——创意编码、生成图案、动画编排、物理动画、微交互、设计规范、后期特效、组件系统、界面设计评审、设计稿生成还原、可拖拽 UI 设计、开发方法论（TDD/计划/验证/评审）、设计哲学（反 AI 味）、研究方向引擎、25 种风格配方、设计稿动效展示（MP4/GIF 导出）、高转化落地页系统、设计词汇表（24 改稿指令 + 62 反-slop 规则 + critique/audit 评审）、界面评审打磨（无障碍/字体/色彩/布局/文案/UI 精修 + 组件状态机/变体）、生成式 UI 框架（catalog 护栏约束的 AI 受控 JSON Spec → 流式渲染，覆盖 React/RN/Vue/Svelte/Solid/3D/邮件/PDF/终端）"
description_en: "cht-ui-skill: a frontend visual & motion toolkit covering p5.js, css-doodle, Theatre.js, React Spring, Inure micro-interactions, UI/UX craft, React PostFX, Chakra UI, oil-ui design/review, draw-ui design-to-code, m3e-canvas draggable UI design, superpowers dev methodology, Anthropic frontend-design philosophy, taste-skill direction engine, garden-skills style recipes, ai-design-skills demo/conversion engine (design-to-motion, landing-page-design), impeccable design-vocabulary & anti-slop steerer (24 steer commands + 62 deterministic slop rules + critique/audit), and jakubkrehel-skills interface review/polish suite (14 sub-skills), and json-render generative-UI framework (vercel-labs, Apache-2.0: catalog-guarded AI-generated JSON specs streamed to renderers across React/RN/Vue/Svelte/Solid/3D/email/PDF/terminal)."
category: frontend
version: 1.5.0
author: cuohuatang
tags:
  - frontend
  - visual
  - animation
  - motion
  - generative-art
  - design-system
  - ui
  - creative-coding
  - m3e
  - canvas
  - prototype
  - draggable
  - development
  - tdd
  - methodology
  - anti-slop
  - design-taste
  - taste-skill
  - frontend-design
  - garden-skills
  - style-recipes
  - art-direction
  - ai-design-skills
  - landing-page
  - design-to-motion
  - motion-export
  - conversion
  - impeccable
  - jakubkrehel-skills
  - better-interface
  - design-vocabulary
  - review
  - accessibility
  - ui-polish
  - generative-ui
  - json-render
allowed-tools: Read,Write,Bash
---

# cht-ui-skill —— 前端视觉与动效技能集

> 把 20 个前端视觉/动效/设计/工程能力**嫁接成一个技能包**。每个能力都是对应知名开源项目（或官方/策展来源）的实战工艺指南，
> 本文件是**总入口与路由**，具体 API、模板、配方都在 `references/` 分册里（渐进披露，按需读取）。

## 一、20 大能力一览

| # | 能力 | 开源来源 | 一句话 |
|---|------|----------|--------|
| 1 | **p5.js 创意编码** | `processing/p5.js` | 交互式 Canvas 视觉、粒子背景、生成艺术 |
| 2 | **CSS Doodle 图案** | `css-doodle/css-doodle` | 类 CSS 小 DSL 生成几何纹理 / SVG / GPU shader |
| 3 | **Theatre.js 编排** | `theatre-js/theatre` | 网页里的 AE：时间轴 + 关键帧，编排出场顺序 |
| 4 | **React Spring 物理动画** | `pmndrs/react-spring` | 弹簧物理弹性，手势跟随与列表进出 |
| 5 | **Inure 精致微交互** | `Hamza417/Inure`（参考样本） | 参考拆解 + 复刻「小操作也舒服」的 UI 动效 |
| 6 | **UI-UX Craft 设计工艺** | 设计规范方法论 | token + 组件状态矩阵 + 交付 QA 门禁 |
| 7 | **React PostFX 后期特效** | `pmndrs/react-postprocessing` | R3F 场景的 Bloom/景深/暗角/glitch 等后期 |
| 8 | **Chakra UI 组件系统** | `chakra-ui/chakra-ui` | 开箱即用、支持主题定制的 React 组件库 |
| 9 | **oil-ui 界面设计/改版/评审** | `oil-oil/oil-ui` | 先定设计北极星，多风格同屏对比、按真实截图打磨视觉层级；只做设计判断 |
| 10 | **draw-ui 设计稿生成/还原** | `oil-oil/draw-ui` | 生成 UI 设计稿（图片），并还原为 HTML/CSS/小程序；与 oil-ui 互补 |
| 11 | **m3e-canvas 可拖拽 UI 设计** | `lnkiai/m3e-canvas` | AI 生成 Material 3 设计 JSON → 分享链接 → 侧边栏/浏览器拖改 → 导出 vibe-coding 提示词 |
| 12 | **superpowers 开发方法论** | `obra/superpowers` | 给 AI 编程代理的完整开发方法论：头脑风暴 → 计划 → TDD → 子代理执行 → 调试 → 验证 → 评审 |
| 13 | **frontend-design 设计哲学** | `anthropics/skills`（Anthropic 官方） | 设计宪法：像设计工作室主设那样思考，避开 5 大 AI 默认陷阱，两遍流程（先 token 设计计划 → 审校 → 再写码） |
| 14 | **taste-skill 研究方向引擎** | `Leonxlnx/taste-skill` | 从 247 个策展画廊站提炼：脚本发牌 20 个研究方向、严格 no-slop 房规、真实浏览器 inspect、三宽度截图 look-and-fix 循环 |
| 15 | **garden-skills 风格配方库** | `ConardLi/garden-skills` | web-design-engineer 内置 25 种风格配方（Linear/Aesop/Pentagram/Stripe…）+ 设计工程师全流程；另含视频演示/图像生成/文章排版/知识检索/动效展示共 6 技能 |
| 16 | **design-to-motion 设计稿动效展示** | `elayadesign/ai-design-skills` | 静态设计稿（Figma/截图/UI 卡片/仪表盘/hero）→ 像素级 HTML 复刻 → 每个视觉"演出"其功能（图表被读、列表进项、prompt 被打字）→ 无缝循环 → 导出 MP4（X）/ 网页 GIF / 800×500 GIF |
| 17 | **landing-page-design 高转化落地页** | `elayadesign/ai-design-skills` | 落地页/营销页完整系统：intake 提问、页面结构、布局选择、转化文案、SEO + 严格视觉规则（字体/间距/圆角/背景/hero/图标/动效）；核心理念 one offer → one audience → one primary action |
| 18 | **impeccable 设计词汇表 / 反-slop 方向盘** | `pbakaus/impeccable`（⭐ ~92.8k） | 编码 Agent 的「设计词汇表」：24 条可执行改稿指令（bolder/quieter/distill/critique/audit…）+ 62 条确定性反-slop 规则 + critique/audit 评审；给 AI 审美补「改稿动词」与客观验收闭环（参考型嫁接：收人读词汇/规则，不含 Rust 引擎） |
| 19 | **jakubkrehel-skills 界面评审打磨套件** | `jakubkrehel/skills`（⭐ ~9k） | 14 个纯 agent 子技能：better-interface/accessibility/typography/colors/layout/writing/ui、interface-review、explain-interface、break、build-design、teardown、state-machine、variant；补全出稿/出码后的证据驱动精修与评审 |
| 20 | **json-render 生成式 UI 框架** | `vercel-labs/json-render`（⭐ ~18.8k，Apache-2.0） | 定义 catalog（组件/动作/数据绑定/visibility/validation 护栏）→ AI 生成受约束 JSON Spec → renderer 流式渲染；覆盖 React/RN/Vue/Svelte/Solid/R3F(3D)/react-email/PDF/Ink(终端)；让"AI 生成 UI"可预测、可校验、失败可降级（参考型嫁接：收 packages/core+react、skills/ 全 30 子技能、examples/chat） |

## 二、什么时候用 / 不要用

**用：** 用户在做前端视觉、UI、动效、组件系统相关任务时，无论要「生成图案」「做粒子背景」
「编排转场」「加弹性反馈」「复刻精致动效」「定设计规范」「加 3D 后期」「搭组件库」，都用本技能路由。
若要做**整站/整页的界面设计、改版、风格探索或多方案对比、独立视觉评审**，路由到 `oil-ui/SKILL.md`（第 9 项）。
若要做**UI 设计稿（图片）生成、截图/参考图精准还原成 HTML/CSS/小程序**，路由到 `draw-ui/SKILL.md`（第 10 项）。
若要做**可拖拽/可交互的 UI 原型**（AI 直出设计、边看边改、导出 vibe-coding 提示词），路由到 `m3e-canvas/SKILL.md`（第 11 项）。
若要把设计交付物变成**工程化、已验证的代码**（需求收敛/计划/TDD/调试/验证/评审），路由到 `superpowers/SKILL.md`（第 12 项）。
若要为设计确立**「不像 AI」的审美哲学**（主题优先、避默认字体、避开 5 大 AI 默认陷阱、两遍流程），读 `frontend-design/SKILL.md`（第 13 项）作为审美底座。
若要**脚本化生成并筛选研究方向**（发牌 20 个已研究方向、反 slop 房规、真实浏览器 inspect、三宽度截图 look-and-fix），路由到 `taste-skill/SKILL.md`（第 14 项）。
若要**套用 25 种具体风格配方**（Linear/Aesop/Pentagram/Stripe…）或走设计工程师全流程（含 Step 0 事实核查、Design Direction Advisor 模式），路由到 `garden-skills/skills/web-design-engineer/SKILL.md`（第 15 项）。
若要做**高转化落地页 / 营销页 / 含转化目标的页面与组件**（intake 提问、页面结构、布局选择、转化文案、SEO、严格视觉规则），路由到 `ai-design-skills/skills/landing-page-design/SKILL.md`（第 17 项）。
若要把**静态设计稿变成会动的展示片**（Figma/截图/UI 卡片/仪表盘/hero 动画，导出 MP4/GIF 用于社媒或落地页动效），路由到 `ai-design-skills/skills/design-to-motion/SKILL.md`（第 16 项）。
若要给设计稿/出码界面做**「设计词汇」级的改稿与反-slop 评审**（用 bolder/quieter/distill/critique/audit 等 24 条指令把审美从形容词变动词，按 62 条确定性规则拦下 AI slop），路由到 `impeccable/SKILL.md`（第 18 项）。
若已出稿/出码、需要**证据驱动的界面评审与打磨**（无障碍/字体/色彩/布局/文案/UI 精修，或组件状态机/变体/拆解/逆向解释），路由到 `jakubkrehel-skills/skills/` 下对应子技能（第 19 项），或先走 `jakubkrehel-skills/skills/better-interface/SKILL.md` 做跨域总评审。
若要构建**由 AI 驱动、但受 catalog 护栏约束的生成式 UI**（AI 只生成你声明的组件/动作/数据绑定、输出可预测可校验、覆盖 React/RN/Vue/Svelte/Solid/R3F/邮件/PDF/终端），路由到 `json-render/SKILL.md`（第 20 项）。

**不用：** 纯后端、纯业务逻辑、与视觉/交互无关的任务无需激活。若只是静态样式微调（颜色/间距），
可走 `ui-ux-craft` 分册的 token 规范；若需要选整体设计风格方向，与 `ui-ux-pro-max` 互补（它选方向，本技能落地）。

## 三、能力选择决策树

| 你想做 | 读这个分册 |
|---|---|
| 互动海报 / 粒子背景 / 鼠标交互 / 数据艺术 / 导出 GIF | `references/01-p5js.md` |
| 几何背景纹理 / 装饰图案 / 参数方程图形 / 品牌纹理 | `references/02-css-doodle.md` |
| 多元素精确时序 / 产品演示 / 3D 运镜 / 页面转场 | `references/03-theatrejs.md` |
| 按钮弹性反馈 / 拖拽跟随 / 列表进出 / 连锁编排 | `references/04-react-spring.md` |
| 复刻「高级感」微交互 / 有参考录屏想拆解实现 | `references/05-inure.md` |
| 统一按钮字号间距 / 补齐 loading·empty·error 状态 / 设计规范 | `references/06-ui-ux-craft.md` |
| 3D 产品展示加 Bloom·景深·暗角·glitch | `references/07-react-postfx.md` |
| 用现成组件库搭界面 / 主题定制 / v3 system | `references/08-chakra-ui.md` |
| 整站/整页设计、改版、多风格对比、截图还原、独立视觉评审 | `oil-ui/SKILL.md`（含自带的 references/、scripts/、assets/） |
| UI 设计稿（图片）生成、截图还原成 HTML/CSS/小程序、参考图精准复刻 | `draw-ui/SKILL.md`（含自带的 references/、scripts/、assets/、evals/） |
| 可拖拽/可交互的 UI 原型、AI 直出设计、边看边改、vibe-coding 提示词 | `m3e-canvas/SKILL.md`（含自带的 scripts/、references/） |
| 开发方法论、需求收敛、计划、TDD、调试、完成前验证、代码评审、子代理驱动 | `superpowers/SKILL.md`（含自带的 skills/，15 个组合式技能） |
| 确立「不像 AI」的审美哲学 / 避开默认字体与默认陷阱 / 设计前先定 token 计划并审校 | `frontend-design/SKILL.md` |
| 脚本化生成研究方向 / 反 slop 房规 / 真实浏览器 inspect / 三宽度截图 look-and-fix | `taste-skill/SKILL.md`（含 `library/` 20 方向、`references/`、`scripts/`） |
| 套用 25 种风格配方 / 设计工程师全流程 / Step 0 事实核查 / Design Direction Advisor / 网页视频演示·图像生成·文章排版·知识检索 | `garden-skills/skills/`（web-design-engineer 等 6 技能） |
| 高转化落地页 / 营销页 / 含转化目标的页面 / 落地页文案与视觉规则 | `ai-design-skills/skills/landing-page-design/SKILL.md`（含严格视觉规则表） |
| 静态设计稿动画化 / Figma·截图·UI 卡片·仪表盘"演出"功能 / 导出 MP4·GIF 展示片 | `ai-design-skills/skills/design-to-motion/SKILL.md` |
| 设计词汇改稿 / 反-slop 评审 / bolder·quieter·distill·critique·audit / 62 条确定性 slop 规则 / 交付前拦 AI 味 | `impeccable/SKILL.md`（references/ 含 24 指令与设计系统，assets/ 含 slop 检测器配置与 token） |
| 界面评审打磨 / 无障碍·字体·色彩·布局·文案·UI 精修 / 组件状态机·变体·拆解·逆向解释 / 跨域总评审 | `jakubkrehel-skills/skills/`（better-interface 等 14 子技能） |
| AI 驱动且受 catalog 护栏约束的生成式 UI / JSON Spec → 流式渲染 / React·RN·Vue·Svelte·Solid·3D·邮件·PDF·终端 | `json-render/SKILL.md`（packages/core 模型 + packages/react 渲染器 + skills/ 30 子技能） |

**组合模式（常见）：** Theatre.js 编排转场 + React Spring 做交互反馈 + React PostFX 做画面；
UI-UX Craft 定 token 与状态规范作为其它所有能力的统一底座；
**审美组合（AI 审美三件套，接口④⑤）**：frontend-design 定审美立场 + taste-skill/garden-skills 供方向素材 + taste-skill look-and-fix 实测验收——专治「AI 味 / 模板脸」；
**交付前评审组合（接口⑧）**：impeccable 的 `critique`/`audit` + 62 条 slop 规则做客观评审，jakubkrehel `better-*` 做证据驱动精修（`better-interface` 总评审、`better-accessibility` 无障碍、`better-typography` 字体、`better-colors` 色彩、`better-layout` 布局、`better-writing` 文案、`better-ui` 视觉/动效），把「评审先于交付」落成可执行步骤。
**生成式 UI 组合（接口⑨）**：json-render 的 catalog 护栏让"AI 生成 UI"成为可控输出——配合 oil-ui 定方向、design-to-motion 出展示、impeccable×jakubkrehel 做评审，形成"设计→生成式落地→动效→评审"闭环。

## 四、全局铁律（跨所有子能力）

1. **只动 `transform` 与 `opacity`**（颜色插值在动画库里安全）。动 `width/height/margin/top/left` 触发 layout，掉帧。
2. **`prefers-reduced-motion` 必须处理**：减弱动效偏好下保留 opacity/color 过渡，去掉位移与缩放；交互类直接呈现终态。
3. **装饰性视觉不承载信息**：图案/粒子/特效层不要放正文；其上叠文字必须有遮罩层保对比度（WCAG ≥ 4.5:1）。
4. **触控热区 ≥ 44×44px**（WCAG），可见控件更小要用伪元素扩，且热区不重叠。
5. **性能预算**：移动端动效要实机验证；粒子数按面积自适应，postprocessing 高开销效果按设备降级。
6. **状态全覆盖**：任何交互组件至少具备 default / hover / active / focus-visible / disabled；数据视图必备 loading / empty / error。
7. **代码与文档同步**：设计 token 与规范改动须同步 `references/06-ui-ux-craft.md` 的约定，避免规范失效。
8. **善用官方文档为准**：下方分册给出经过核验的 API 与版本要点，但库会迭代，落地前以官方文档/当前版本为准。
9. **TDD 不可跳过**（superpowers）：写任何实现代码前先写测试，且必须亲眼看过测试失败（红）再写实现到通过（绿）。
10. **计划先行**（superpowers）：需求未收敛不进实现；计划未确认不动手；不 YAGNI/DRY 双标——不做多余的东西，重复代码必须抽象。
11. **完成前验证**（superpowers）：声称"完成"前，必须运行验证（测试/构建/检查）并给出证据，不得口头宣称完成。
12. **反 AI 默认陷阱**（frontend-design）：动笔前先识别并避开 AI 生成界面的 5 大默认特征——① 米白底(#F4F1EA)+高对比衬线+陶土/暖橙强调；② 近黑底+单一荧光绿/朱红强调；③ 报纸式细线密集分栏、零圆角；④ SaaS 卡片套件（同一圆角/同一灰阴影/渐变装饰）；⑤ 模板铬件（全大写 eyebrow、"A · B · C" 中点串、"词—片段"破折号标签、等宽小数据标签、链接文字后加 "→"）。这些对某些 brief 合法，但若是「默认」而非「为这个 brief 做的选择」就不要用。
13. **实测而非空想**（taste-skill）：设计好坏靠**真实浏览器测量与截图**判定，不凭感觉——用 `taste-skill/scripts/inspect.mjs` 量排版，走「三宽度截图 → 评审 rubric → fix → 再看」的 look-and-fix 循环；没在浏览器里亲眼看过自己做的页面，不算做完。
14. **事实先于设计**（garden web-design-engineer Step 0）：设计涉及具体产品/品牌/技术/版本/时间线时，**先核实再设计**，不凭记忆断言；搜不到或存疑就问用户，禁用"我觉得 X 还没发布 / 应该是 N 版 / X 大概不存在"这类无据表述。
15. **一页一意图**（landing-page-design）：落地页不是首页——一次 offer → 一类受众 → 一个主行动。禁止首屏多个互相竞争的 CTA、禁止含糊价值主张（"streamline/optimize"）、禁止背景渐变与单侧卡片描边；字号/间距/圆角必须落到 Tailwind 刻度，正文禁用连字符、禁斜体、禁用 900/black 字重。
16. **评审先于交付**（impeccable × jakubkrehel-skills）：出稿/出码后、声称完成前，先跑一遍**客观评审**：用 impeccable 的 `critique`（打分 UX 评审）+ `audit`（P0–P3 技术质量，含无障碍/性能/主题/响应式）对照 62 条 slop 规则拦 AI 味；再按 jakubkrehel `better-*` 做证据驱动精修（无障碍/字体/色彩/布局/文案/UI），只报有证据的问题、不报纯品味偏好。报告门槛是「有证据」，`Approve` 门槛是「真检查过你声称检查过的东西」。
17. **生成式 UI 必须 catalog 护栏约束**（json-render）：任何"AI 生成 UI"场景，必须先定义 catalog（声明允许的组件/动作/数据绑定/visibility/validation），让 AI 只生成受约束的 JSON Spec、再交给 renderer 流式渲染——禁止无 catalog 自由生成不可预测 UI；输出须可校验、可回放、失败可降级。

## 五、分册索引（触发词 → 文件）

| 分册 | 触发词 |
|---|---|
| `01-p5js.md` | p5.js、Processing、sketch、粒子、流场、柏林噪声、生成艺术、互动背景 |
| `02-css-doodle.md` | css-doodle、CSS 图案、生成背景、几何纹理、@grid、@shape、@pattern |
| `03-theatrejs.md` | Theatre.js、时间轴、关键帧、编排动画、cinematic camera、转场 sequence |
| `04-react-spring.md` | react-spring、弹性动画、物理动画、spring animation、回弹、拖拽跟随 |
| `05-inure.md` | Inure、微交互、精致动效、操作反馈、菜单展开、页面切换、交互质感 |
| `06-ui-ux-craft.md` | 设计规范、按钮统一、字号间距、加载/空/错状态、UI 工艺、DESIGN.md、token |
| `07-react-postfx.md` | postprocessing、后期特效、bloom、景深、暗角、glitch、扫描线、R3F 特效 |
| `08-chakra-ui.md` | Chakra UI、组件系统、主题定制、chakra v3、recipe、design system |
| `oil-ui/SKILL.md` | oil-ui、界面设计、改版、风格探索、多方案对比、截图还原、视觉评审、设计北极星、design direction |
| `draw-ui/SKILL.md` | draw-ui、UI 设计稿、生成设计图、截图还原、HTML 还原、小程序、参考图复刻、design mockup、reconstruction |
| `m3e-canvas/SKILL.md` | m3e、M3E Canvas、可拖拽设计、可交互原型、Material 3 画布、AI 直出设计、边看边改、vibe-coding、分享链接、#docz |
| `superpowers/SKILL.md` | superpowers、开发方法论、需求收敛、计划、TDD、测试驱动、调试、完成前验证、代码评审、子代理驱动、worktree |
| `frontend-design/SKILL.md` | frontend-design、设计哲学、审美宪法、反 AI 味、避开默认陷阱、design lead、token 设计计划、typography |
| `taste-skill/SKILL.md` | taste-skill、design-taste-frontend、研究方向、反 slop、no-slop、draw.mjs 发牌、浏览器实测、look-and-fix、AI tells、premium、award-level |
| `garden-skills/skills/web-design-engineer/SKILL.md` | garden-skills、web-design-engineer、风格配方、style-recipes、Linear/Aesop/Pentagram/Stripe、设计工程师、事实核查、Design Direction Advisor、网页视频演示、图像生成、文章排版、知识检索 |
| `ai-design-skills/skills/landing-page-design/SKILL.md` | landing-page-design、落地页、营销页、转化、landing page、CTA、hero、SEO、AEO、intake、转化文案、页面结构、布局选择、one offer、one audience |
| `ai-design-skills/skills/design-to-motion/SKILL.md` | design-to-motion、设计稿动画、Figma 动画、截图还原动画、UI 卡片动画、仪表盘动画、hero 动画、展示片、MP4 导出、GIF 导出、motion mockup、showcase loop、空状态加载 |
| `impeccable/SKILL.md` | impeccable、设计词汇、design vocabulary、bolder、quieter、distill、critique、audit、slop 检测、62 规则、反 AI 味、改稿动词、kinpaku |
| `jakubkrehel-skills/skills/better-interface/SKILL.md` | jakubkrehel、better-interface、better-accessibility、better-typography、better-colors、better-layout、better-writing、better-ui、interface-review、state-machine、variant、break、组件评审、UI 精修、无障碍评审 |
| `json-render/SKILL.md` | json-render、generative-ui、生成式 UI、catalog、spec、renderer、@json-render/core、@json-render/react、AI 生成界面、受控 UI、流式渲染、React·RN·Vue·Svelte·Solid·R3F·邮件·PDF·终端 |

## 六、与其它技能的关系

- `oil-ui`（第 9 项）：负责**界面设计、改版、风格探索、多方案对比与独立视觉评审**，自带完整的设计方法与截图工具；是 cht-ui-skill 里「设计判断」这一层的主体。它与本集其它 8 项（落地实现）配合：oil-ui 定方向/出评审结论 → 其余分册负责把设计**落地**成可运行代码与组件。
- `draw-ui`（第 10 项）：负责**生成 UI 设计稿（图片）并把截图/参考图精准还原为 HTML/CSS/小程序**，是「设计稿生成 + 还原成代码」这一层。它与 oil-ui 互补——draw-ui 自己也会在探索视觉方向时推荐 oil-ui，二者常串联：draw-ui 出图/还原 → oil-ui 做方向打磨与评审；对已有界面的小幅改造则直接用 draw-ui 的还原路径。
- `m3e-canvas`（第 11 项）：负责**可拖拽/可交互的 UI 原型**——AI 按 M3E 协议生成设计 JSON，压缩进分享链接，用户在豆包侧边栏或浏览器画布里直接拖改，改完导出 vibe-coding 提示词喂给 AI 代码生成。与 draw-ui 互补：draw-ui 出**静态精细稿**，m3e-canvas 出**可拖改原型**；在内置工作流第二步作为分支乙（见第七节）。
- `superpowers`（第 12 项）：负责**开发方法论**——需求收敛（brainstorming）、实现计划（writing-plans）、测试驱动开发（test-driven-development）、子代理驱动执行（subagent-driven-development）、系统化调试（systematic-debugging）、完成前验证（verification-before-completion）、代码评审（requesting/receiving-code-review）。是「工程实现」这一层：cht-ui-skill 的设计/视觉能力负责"做出什么"，superpowers 负责"怎么工程化交付"；在内置工作流第一步（需求模糊时）与第三步（工程模式）对接（见第七节）。
- `frontend-design`（第 13 项，Anthropic 官方）：**审美哲学底座**——像设计工作室主设那样思考：主题优先、避默认字体、列出并避开 5 大 AI 默认陷阱、两遍流程（先 token 设计计划 → 审校 → 再写码）。它回答「怎么思考才不像 AI」，供所有设计/出稿环节做审美校准。
- `taste-skill`（第 14 项）：**研究方向引擎**——`scripts/draw.mjs` 从 247 个策展站提炼的 20 个研究方向里发牌 3 个供选，`library/` 提供 type/palette/hero/section 蓝图，`scripts/inspect.mjs` 在真实浏览器里量排版，走三宽度截图 + rubric + fix 的 look-and-fix 循环。与 oil-ui 互补：oil-ui 做设计**判断**，taste-skill 提供**可执行的方向素材与反 slop 验收**。
- `garden-skills`（第 15 项）：**风格配方库 + 设计工程师全流程**——`web-design-engineer` 内置 25 种锚定风格配方（Linear/Aesop/Pentagram/Bloomberg/Stripe…，各含调色板/字体/手法/反模式）、Step 0 事实核查、需求模糊时切 Design Direction Advisor 模式；另含 `web-video-presentation`（网页视频演示）、`gpt-image-2`（图像生成）、`beautiful-article`（文章排版）、`kb-retriever`（知识检索）、`motion-showreel`（动效展示）。是「具体风格从哪来」的弹药库。
- `ai-design-skills`（第 16/17 项，elayadesign）：**设计演示与转化引擎**——`design-to-motion`（第 16 项）把静态设计稿（Figma/截图/UI 卡片/仪表盘/hero）在空状态加载后逐元素"演出"功能、无缝循环、导出 MP4（X）/ 网页 GIF / 800×500 GIF，是"会动的展示片"专用引擎，与 Theatre.js（编排）、motion-showreel（短视频）互补；`landing-page-design`（第 17 项）是落地页/营销页的转化视角系统（intake 提问 / 页面结构 / 布局选择 / 转化文案 / SEO + 严格视觉规则），与 oil-ui（设计判断）、draw-ui（出稿）互补，补上"营销页/落地页转化率"这块拼图。
- `impeccable`（第 18 项，pbakaus）：**设计词汇表与反-slop 方向盘**——把审美从形容词变成动词：24 条可执行指令（bolder/quieter/distill/critique/audit…），其中 `critique` 打分 UX 评审、`audit` 出 P0–P3 技术质量报告；另用 62 条确定性规则在交付前拦下 AI slop（紫蓝渐变、Inter 包打一切、卡片套卡片…）。与「AI 审美三件套」互补：frontend-design 给立场、taste-skill/garden-skills 给方向、**impeccable 给改稿动词与客观评审**，三者共同把"像不像 AI"从感觉变成可操作的步骤。
- `jakubkrehel-skills`（第 19 项，jakubkrehel）：**界面评审与打磨套件**——14 个纯 agent 子技能，覆盖出稿/出码后的证据驱动精修：better-interface（跨域总评审）、better-accessibility/typography/colors/layout/writing/ui（单域打磨）、interface-review（变更评审）、state-machine/variant/break/teardown（组件级工程）、explain-interface/build-design（逆向与转码）。它把铁律 16「评审先于交付」落到实处：只报有证据的问题，不报纯品味偏好。
- `json-render`（第 20 项，vercel-labs）：**生成式 UI 框架**——把"AI 生成界面"从自由发散收敛为"catalog 护栏约束下的受控 JSON Spec → renderer 流式渲染"：AI 只能使用你 catalog 里声明的组件/动作/数据绑定，输出永远可预测、可校验、失败可降级，覆盖 React/RN/Vue/Svelte/Solid/R3F(3D)/react-email/PDF/Ink(终端)。它补上 cht-ui-skill 在"AI 驱动但可靠"这一层的空白，与 oil-ui（方向）、design-to-motion（展示）、impeccable×jakubkrehel（评审）串联成"设计→生成式落地→动效→评审"闭环。
- `ui-ux-pro-max`：负责选「风格方向」（风格/配色/字体）；本技能负责把方向**落地**成可运行代码与规范。
- `web-design-guidelines`（可访问性审计）：可在交付前做质量复核。
- 本技能是「实践工艺 + 审美哲学 + 工程方法论 + 转化/演示 + 评审打磨」层，与它们构成「审美底座(frontend-design) → 方向选择(风格配方库/研究方向引擎) → 落地页转化视角(landing-page-design) → 设计判断(oil-ui) → 设计稿生成/还原(draw-ui) 或 可拖改原型(m3e-canvas) → 规范制定 → 工程化实现(superpowers) → 动效展示/导出(design-to-motion) → 改稿动词与客观评审(impeccable) → 证据驱动精修(jakubkrehel-skills) → 实测验收(taste-skill) → 可访问性审计」的前端质量闭环。

## 七、内置工作流：出方案矩阵 → 出稿（静态稿 / 可拖改原型）→ 生成可运行代码（快速 / 工程模式）

> 适用：用户说"做个界面 / 设计个页面 / 想看看几种风格"，但**还没定方向**，需要先看方案、再出正式稿、最后还要能跑起来的代码。
> 这条流水线把「方向（oil-ui）× 技术气质（8 大分册）× 交互形态（draw-ui 静态稿 / m3e-canvas 可拖改原型）」组合成**方案矩阵**，
> 第一步后设一道人工确认闸门，第二步按用户偏好走**分支甲（静态精细稿）或分支乙（可拖改原型）**，第三步进入代码生成
> （**快速模式**或接 superpowers 的**工程模式**），第四步完成前验证（superpowers 铁律）。若交付物是落地页/营销页，可在出稿前插 **landing-page-design（接口⑥）** 定转化结构与文案；出稿/出码后若需社媒展示片，可插 **design-to-motion（接口⑦）** 生成会动的 MP4/GIF；**第六步（接口⑧）无论哪条路径都必须跑** impeccable × jakubkrehel-skills 的交付前评审闭环，把 AI 味与质量问题在交付前拦下。

**整体流向：**

```
[用户提需求]
   │
   ▼
【第一步 · 出方案矩阵（多维组合）】
   · 需求模糊 → 先触发 superpowers/brainstorming 收敛出 spec（接口①）
   · frontend-design 审美打底：定 token 设计计划 + 避开 5 大 AI 默认陷阱（接口④）
   · taste-skill / garden-skills 采集方向素材：draw.mjs 发牌 20 研究方向 / 25 种风格配方（接口⑤）
   · oil-ui 定调性：认品类 / 拆标杆 / 写 N 套（默认 3）风格方向
   · 8 大分册定技术气质：p5 粒子 / CSS Doodle 图案 / Theatre 叙事 / Spring 弹性 / Inure 微交互 / Chakra 组件 / PostFX 后期 / Craft 规范
   · 交互形态：静态稿（draw-ui）或 可拖改原型（m3e-canvas）
   → 组合成「风格 × 技术 × 形态」候选集（默认 6–9 版，可要求十几版）
   → 做成首屏对比页交给用户挑
   · 若交付物是落地页/营销页 → 先触发 landing-page-design 定转化结构/文案/视觉规则（接口⑥），再进第二/三步
   │
   ▼
★ 第一步收尾闸门（必须询问）★
   "方向已定 ✅ 第二步走哪个分支？
     分支甲：draw-ui 出【静态精细设计稿】
     分支乙：m3e-canvas 出【可拖改原型】（AI 直出设计，边看边改）
     也可只停在设计说明 / 直接做可运行实现。"
   │  ← 等用户确认，未确认不进第二步
   ▼
【第二步 · 按分支出稿】
   分支甲（draw-ui）：以选定方向卡为视觉基线，生成精细视觉稿，可还原 HTML/CSS/小程序
   分支乙（m3e-canvas）：按 M3E 协议生成设计 JSON → 分享链接 → 侧边栏/浏览器拖改
   │
   ▼
【第三步 · 生成可运行代码（双模式）】
   快速模式（原）：设计稿/prompt → v0.dev Chat / Builder.io → React/Next 代码 → 人工接项目
   工程模式（superpowers，接口②）：设计定稿 → writing-plans → test-driven-development
       → subagent-driven-development → verification-before-completion → code-review
       → 交付已验证的工程化代码
   │
   ▼
【第四步 · 完成前验证（接口③，superpowers 铁律）】
   声称完成前：跑测试 / 构建 / 检查，附验证证据；有未通过项不得宣称完成
   │
   ▼
【第五步 · 生成式 UI（json-render，接口⑨，可选）】
   若需"AI 驱动但受 catalog 护栏约束"的生成式 UI：先定 catalog → AI 生成受约束 JSON Spec → renderer 流式渲染（见 json-render/SKILL.md）
   │
   ▼
【第六步 · 动效展示导出（design-to-motion，接口⑦，可选）】
   若需"会动的展示片"（社媒 MP4 / 网页 GIF / 800×500 小 GIF / 落地页 hero·bento 卡片循环）：
   把静态设计稿（Figma/截图/UI 卡片/仪表盘/hero）按 design-to-motion 流程像素级复刻 →
   空状态加载 → 每视觉演出其功能 → 无缝循环 → 导出 MP4(X)/网页 GIF/800×500 GIF
   │
   ▼
【第七步 · 交付前评审（impeccable × jakubkrehel-skills，接口⑧，必做）】
   出稿/出码后、手动交付前，跑客观评审闭环：
   · impeccable：critique（打分 UX 评审，排出先修项）+ audit（P0–P3 技术质量：无障碍/性能/主题/响应式）
     + 对照 62 条确定性 slop 规则拦 AI 味（assets/detector-config.json）
   · jakubkrehel-skills：better-interface 跨域总评审 → better-accessibility/typography/colors/layout/writing/ui
     做证据驱动精修；只报有证据的问题，不报纯品味偏好（详见铁律 16）
   → 修复 P0/P1 后再交付
   │
   ▼
【你手动接进项目 → git 提交 → 部署】
```

### 第一步：出方案矩阵（多维组合）

1. **需求模糊时先收敛（接口①）**：用户需求不清晰（"做个好一点的界面"），先读 `superpowers/skills/brainstorming/SKILL.md`，用头脑风暴法问出真实目标、约束与验收标准，输出一句话 spec 后再进入方案矩阵。
2. **审美打底（frontend-design，接口④）**：先按 `frontend-design/SKILL.md` 写出紧凑 token 设计计划——色（4–6 个命名 hex）/ 字体及角色 / 布局概念（一句话 + ASCII 线框）/ 本页独有原则；然后对照 brief 自审：哪部分像"换个 brief 也会给的默认答案"就改掉，并主动避开 5 大 AI 默认陷阱（见铁律 12）。这一步决定整套方案的审美水位。
3. **采集方向素材（taste-skill / garden-skills，接口⑤）**：想要脚本化、可复现的研究方向 → 跑 `taste-skill/scripts/draw.mjs --options 3`（应用屏用 `--app`）从 20 个已研究方向里发牌，`taste-skill/library/` 直接给出 type/palette/hero/section 蓝图；想锚定某个具体品牌气质 → 从 `garden-skills/skills/web-design-engineer/references/style-recipes/`（先读 `INDEX.md`）挑 1 个配方（Linear/Aesop/Pentagram/Stripe…）作视觉基线。
4. 按 `oil-ui/SKILL.md` 的「1. 探索并收敛方向」：认品类、拆标杆、定调性，先写出 **N 套（默认 3）风格不同的方向**（可用第 3 步的方向素材/风格配方做种子，避免从零拍脑袋）。
5. **叠加技术气质维度**：从 8 大分册中选 1–2 种与本设计匹配的技术路线（如「p5 粒子背景 + 科技感」「Chakra 组件化 + 工具效率」「Inure 微交互 + 高级感」），把「风格 × 技术」组合成候选集。
6. 每套用三四行简述：给人什么感觉、首屏长什么样、字体与色彩、主视觉靠什么、用什么技术实现；附上推荐哪套及理由。
7. 用户要看实图 → 按 oil-ui 的「风格对比页」把候选集做成真实首屏放进对比页（含 `sheet` 总览图）交给用户挑；**这一轮到此结束**，不自动往下走。出稿与验收时用 `taste-skill` 的 look-and-fix（三宽度截图 + rubric）做质量闭环（见铁律 13）。
8. **第一步收尾闸门（强制询问，不可跳过）**：用户挑定后，必须主动询问——
   > 已定方向 ✅。第二步走哪个分支？**分支甲：draw-ui 出静态精细稿**（完整页面/长页精修视觉稿）；**分支乙：m3e-canvas 出可拖改原型**（AI 直出、边看边改）；也可以只停在设计说明，或直接做可运行实现。
   - 用户确认分支 → 进入对应第二步路径；
   - 用户选"只做设计说明 / 直接可运行实现" → 按对应分册收尾，**不强行调用 draw-ui / m3e-canvas**。

### 第二步·分支甲：出详细设计稿（draw-ui）

1. 把第一步选定的**方向卡作为视觉基线**，读 `draw-ui/SKILL.md` 的「新设计或风格探索」路径。
2. 按 `references/ui-design.md` 组织提示词、生成并检查；若是完整长页，再读 `references/full-page.md` 分段生成。
3. 交付：设计稿图片 + 简短实现说明；如需继续还原成 HTML/CSS/微信小程序，按 draw-ui 的还原路径（software-reconstruction / html-reconstruction）走。

### 第二步·分支乙：出可拖改原型（m3e-canvas）

1. 读 `m3e-canvas/SKILL.md`：按 M3E 协议把选定方向生成设计 JSON（含 frames 屏幕 + groups 部件，默认手机 412×892）。
2. 运行 `m3e-canvas/scripts/make_link.py` 把 JSON 压缩成分享链接（`#docz=` 形式，整个设计都在链接里）。
3. 交付**双模式**（用户自选、可随时切换）：模式 A 把链接贴进豆包侧边栏直接拖改；模式 B 浏览器/客户端点开拖改。
4. 用户拖改完成后，在画布右上角「提示词」按钮导出 vibe-coding prompt（可编辑、可保存单屏 PNG）。

### 第三步：生成可运行代码（快速 / 工程模式）

**快速模式（默认，人工收口）：**
1. 把第二步产出的**详细设计稿（图片/截图）**或 m3e prompt 作为视觉基准，交给 **v0.dev Chat** 或 **Builder.io**（或用户的 AI 编码工具），生成 React / Next.js 等可运行前端代码。
2. 在工具内迭代到结构、视觉接近设计稿；导出代码。
3. **你（或主 Agent 协助）手动**把生成的代码接进现有项目、跑通、`git commit`、部署。这一步是人工收口，不在 Skill 自动范围内。

**工程模式（superpowers 驱动，接口②）：**
适用：用户要求"工程化交付 / 带测试 / 质量保障"，或代码要长期维护、多人协作。
1. 读 `superpowers/SKILL.md`，从 `skills/writing-plans/SKILL.md` 开始：把设计定稿 + 需求 spec 写成可执行实现计划（任务拆解、验收标准）。
2. 按 `skills/test-driven-development/SKILL.md` 执行真·红绿 TDD：先写测试看失败（红）→ 写最小实现到通过（绿）。
3. 任务量大时按 `skills/subagent-driven-development/SKILL.md` 拆给子代理并行驱动，各任务独立验证。
4. 完成后按 `skills/verification-before-completion/SKILL.md` 全面验证；复杂功能走 `skills/requesting-code-review/SKILL.md` + `skills/receiving-code-review/SKILL.md` 收评审意见并消化。
5. 交付：可运行代码 + 测试通过证据 + 实现说明；代码接入与部署仍由你手动收口。

**分支乙衔接**：m3e 路线用户改完原型导出 prompt 后，**先呈现 prompt，询问用户**是走快速模式（直接喂 AI 编码工具）还是工程模式（superpowers 驱动带 TDD/验证）；未获指令前不自动执行。

### 第四步：完成前验证（接口③，superpowers 铁律）

1. **声称"完成"前**：必须运行最小验证集——测试（vitest/jest/对应测试框架）、构建（tsc/build）、检查（lint/typecheck），把命令输出作为**验证证据**附在交付说明里。
2. 有未通过项：不得宣称完成，修复后重跑直至通过；无法自动化验证的（视觉还原度等），明确列出人工核对项。
3. 验证范围与结果、仍存在的缺口，随交付说明一起给出。

### 第五步·生成式 UI（json-render，可选）

适用：需要「AI 驱动、但受 catalog 护栏约束」的生成式 UI——让 AI 只生成你 catalog 里声明的组件/动作/数据绑定，输出可控、可校验、失败可降级，覆盖 React/RN/Vue/Svelte/Solid/R3F(3D)/react-email/PDF/Ink(终端)。

1. 读 `json-render/SKILL.md` 建立 catalog→spec→renderer 心智；先读 `packages/core/README.md` 与 `packages/core/src/` 弄清 catalog（组件/动作/数据绑定/visibility/validation 护栏）怎么写。
2. 按目标框架读 `skills/<framework>/SKILL.md`（react / next / react-native / react-three-fiber / react-email / react-pdf / vue / svelte / solid / ink…）拿该框架的 catalog 写法与 agent 子技能。
3. 以 `examples/chat/` 为参考：看 `lib/render`（spec→UI）、`lib/tools`（catalog 里的动作）、`components/ui`（被 catalog 声明的组件）如何配合。
4. 铁律 17 不可破：必须先有 catalog 护栏，再让 AI 生成受约束 JSON Spec，最后 renderer 流式渲染；禁止无 catalog 自由生成不可预测 UI。

### 第六步·动效展示导出（design-to-motion，可选）

适用：设计稿/落地页/官网里需要"会动的展示片"——社媒视频（X/Twitter 的 MP4）、网页内嵌 GIF、800×500 小 GIF，或落地页 hero / bento 卡片的入场与故事循环。

1. 读 `ai-design-skills/skills/design-to-motion/SKILL.md`：先确定上下文（Showcase 导出视频 vs Website 嵌入站点代码），再按 PART A 做像素级复刻（Figma 走 REST API、截图则逐元素重建/剥离/裁切），用 `?still` 比对参考帧（PSNR 达标）后再动。
2. 按 PART B 做动效：空状态加载（rise + blur）、每个视觉演出其功能（图表被读、列表进项、prompt 打字…）、无缝循环；尊重 `prefers-reduced-motion`。
3. 按 PART C 用确定性逐帧捕获（`?capture` + 假时钟，禁用实时录屏）导出 `<name>-x.mp4`、`-loop.gif`、`-800x500.gif`。
4. 交付三件套（MP4/GIF）+ 保真度与溢出检查结果；Showcase 走导出，Website 则把动画片段嵌回站点代码（仅当用户要求时才导出）。

### 第七步·交付前评审（impeccable × jakubkrehel-skills，接口⑧，必做）

无论走快速还是工程模式、无论是否做动效展示，出稿/出码后、手动交付前都必须跑这一闭环（对应铁律 16）：

1. **改稿动词与客观评审（impeccable）**：读 `impeccable/SKILL.md` 与 `references/README.md`（24 指令全表）。先按需求挑窄目标下达动词——`bolder`/`quieter`/`distill`/`colorize`/`typeset`/`layout`/`animate`；再做 `critique`（打分 UX 评审，排出先修项）与 `audit`（P0–P3 技术质量：无障碍 / 性能 / 主题 / 响应式）；对照 `assets/detector-config.json` 的 62 条确定性 slop 规则自检 AI 味（Inter 包打、紫蓝渐变、卡片套卡片、灰字压彩底、标题上方圆角图标瓦片等）。
2. **证据驱动精修（jakubkrehel-skills）**：先跑 `jakubkrehel-skills/skills/better-interface/SKILL.md` 做跨域总评审，再按它路由到 `better-accessibility`（WCAG 2.2）、`better-typography`、`better-colors`、`better-layout`、`better-writing`、`better-ui`。原则：只报有证据的问题，纯品味偏好不算 finding；先 recon 项目框架/token/视口，用项目自身惯用法写修复。
3. **收敛**：先修 P0（阻断级）与 P1，P2/P3 酌情；修复后重跑评审确认无回归，再交手动接入。
4. 把评审结论（critique 排序 + audit 严重级 + 落地修复）随交付说明一起给出，作为「评审先于交付」的证据。

### 关键约定

- **下游闭环**：第一步后闸门确认 → 第二步按分支出稿（静态稿或可拖改原型）→ 第三步双模式出可运行代码 → 第四步完成前验证；最终由你手动接入项目、git 提交与部署，Skill 产出止于"可运行代码已生成且通过验证"。
- **严格顺序**：方向未定不进第二步；第二步不重新发散风格，只把已锁定的方向做成稿/原型。
- **闸门不能省**：第一步后必须询问分支选择；第三步工程模式必须先呈现计划/测试方案征得用户同意再执行，避免"替用户默认决策"。
- **分支可切换**：选定静态稿后想改可拖改原型（或反之），回到闸门重新选分支即可；已产出的稿/原型保留，以最新选择为准。
- **可回退**：选定方向后想换另一套，回到第一步对比页再选；已生成的稿/原型以最新选定的方向为准。
- **快速/工程模式可切换**：工程模式生成的代码结构与快速模式一致时可互转；默认快速，用户要求质量保障才切工程模式。
- **与其它能力衔接**：进了第二步需要真实前端实现时，再路由到 `references/08-chakra-ui.md`（组件）或 `references/07-react-postfx.md`（3D 后期）等落地分册；需要开发方法论支持时路由到 `superpowers/skills/`。
