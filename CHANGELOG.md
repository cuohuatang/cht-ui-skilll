# CHANGELOG

## v1.6.0 — 2026-10-29

**新增（设计智能数据库，来源 `nextlevelbuilder/ui-ux-pro-max-skill`，⭐ ~142k，MIT）**
- 第 21 项能力 `ui-ux-pro-max/`：可检索设计知识库——**79 UI 风格 / 192 套配色 / 74 组字体配对 / 119 条 UX 准则 / 25 种图表 / 22 个技术栈**（v2.15.0，实测强于视频里的 50/97/9），含 `scripts/` BM25 检索 CLI 与 `templates/` 输出模板。**精选参考型嫁接**：收 `README.md`/`README.zh.md`/`LICENSE`/`skill.json` + `src/ui-ux-pro-max/` 的 `data`（39 CSV 库）/ `scripts`（31 检索脚本）/ `templates`（26 输出模板）三件套共 100 文件 / 3.8MB；排除整仓 screenshots/gallery/多语言 README/CLI（整仓 8.3MB）。它是 cht-ui-skill 缺的"**可检索设计知识层**"，与 frontend-design（审美立场）、garden-skills/taste-skill（方向素材）衔接成"查库取事实 → 定方向 → 落地"。

**变更（深入嫁接，非仅入表）**
- 全局铁律新增 1 条：18 选型查库，禁止凭空杜撰（ui-ux-pro-max，涉及风格/配色/字体配对/UX 准则/技术栈时优先用其数据库检索取事实）。
- 组合模式新增「设计智能组合（接口⑩）」：ui-ux-pro-max 让选型成为查库动作，与 frontend-design 定立场、garden-skills/taste-skill 供素材串联。
- 内置工作流第一步「采集方向素材」接入 ui-ux-pro-max 检索（接口⑤⑩）。
- README 与 SKILL.md 同步：能力表 20 → 21、frontmatter description / tags（ui-ux-pro-max / design-intelligence / color-palette / typography-pairing）、决策树、触发词索引、「与其它技能的关系」（定位为设计智能数据库层）、组合模式新增设计智能组合；版本号 1.5.0 → 1.6.0。

> 注：`frontend-design`（Anthropic 官方设计哲学）早在 v1.2.0 即已作为第 13 项能力完整嫁接（选这俩时它已在包内），本次仅新增 ui-ux-pro-max 一项；能力数由 20 升 21。

## v1.5.0 — 2026-10-29

**新增（生成式 UI 框架，来源 `vercel-labs/json-render`，⭐ ~18.8k，Apache-2.0）**
- 第 20 项能力 `json-render/`：Vercel 出品的 Generative UI 框架——定义 **catalog**（组件/动作/数据绑定/visibility/validation 护栏）→ AI 生成**受约束的 JSON Spec** → **renderer** 流式渲染；覆盖 React/RN/Vue/Svelte/Solid/R3F(3D)/react-email/PDF/Ink(终端)，让"AI 生成 UI"可预测、可校验、失败可降级。**精选参考型嫁接**：收 `packages/core`（catalog/spec 模型灵魂）+ `packages/react`（主流渲染器）+ `skills/`（30 个 agent 子技能全集）+ `examples/chat`（最小可运行示例）+ 根文档与 LICENSE；未收整仓其余 36 包/apps/23 示例（整仓 ~14M）。新增入口 `json-render/SKILL.md`（嫁接索引，Apache-2.0 归属上游）。

**变更（深入嫁接，非仅入表）**
- 内置工作流新增**第五步·生成式 UI（json-render，可选，接口⑨）**：先定 catalog → AI 生成受约束 JSON Spec → renderer 流式渲染；原动效展示导出顺延为第六步、交付前评审顺延为第七步。
- 全局铁律新增 1 条：17 生成式 UI 必须 catalog 护栏约束（json-render，禁止无 catalog 自由生成不可预测 UI）。
- 组合模式新增「生成式 UI 组合（接口⑨）」：json-render 的 catalog 护栏让"AI 生成 UI"成为可控输出，与 oil-ui 定方向、design-to-motion 出展示、impeccable×jakubkrehel 做评审串联成"设计→生成式落地→动效→评审"闭环。
- README 与 SKILL.md 同步：能力表 19 → 20、frontmatter description / tags（generative-ui / json-render）、决策树、触发词索引、「与其它技能的关系」（定位为生成式 UI 框架层）、工作流新增第五步；版本号 1.4.0 → 1.5.0。

## v1.4.0 — 2026-10-29

**新增（设计词汇表与界面评审打磨，来源 A 方案执行）**
- 第 18 项能力 `impeccable/`（来源 `pbakaus/impeccable`，⭐ ~92.8k）：编码 Agent 的「设计词汇表」——24 条可执行改稿指令（bolder/quieter/distill/critique/audit…）+ 62 条确定性反-slop 规则 + critique/audit 评审。**参考型嫁接**：只收人读词汇与规则文档（`references/` 含 24 指令全表与设计系统、`assets/` 含 slop 检测器配置与 design-system token），不含 Rust CLI 引擎。与「AI 审美三件套」互补：frontend-design 给立场、taste-skill/garden-skills 给方向、impeccable 给改稿动词与客观评审。
- 第 19 项能力 `jakubkrehel-skills/`（来源 `jakubkrehel/skills`，⭐ ~9k）：14 个纯 agent 子技能整包嫁接（`skills/` 含 better-interface/accessibility/typography/colors/layout/writing/ui、interface-review、explain-interface、break、build-design、teardown、state-machine、variant）。补全出稿 / 出码后的证据驱动精修与评审（无障碍 / 字体 / 色彩 / 布局 / 文案 / UI + 组件状态机 / 变体 / 拆解）。

**变更（深入嫁接，非仅入表）**
- 内置工作流新增接口⑧「交付前评审」作为**第六步（必做）**：impeccable 的 critique/audit + 62 条 slop 规则 + jakubkrehel `better-*` 证据驱动精修，把「评审先于交付」落成可执行步骤（对应新增铁律 16）。
- 全局铁律新增 1 条：16 评审先于交付（impeccable × jakubkrehel-skills，客观评审闭环，只报有证据的问题）。
- README 与 SKILL.md 同步：能力表 17 → 19、frontmatter description / tags（impeccable / jakubkrehel-skills / review / accessibility / ui-polish）、决策树、触发词索引、「与其它技能的关系」（二者定位为设计词汇表方向盘 / 界面评审打磨套件）、组合模式新增「交付前评审组合」、闭环句子纳入评审打磨层；版本号 1.3.0 → 1.4.0。

## v1.3.0 — 2026-10-27

**新增（设计演示与转化引擎，来源 `elayadesign/ai-design-skills`）**
- 第 16 项能力 `ai-design-skills/skills/design-to-motion/`：把静态设计稿（Figma / 截图 / UI 卡片 / 仪表盘 / hero）像素级 HTML 复刻 → 空状态加载 → 每个视觉「演出」其功能 → 无缝循环 → 导出 MP4（X）/ 网页 GIF / 800×500 GIF；含确定性逐帧捕获（PART A 保真 / PART B 动效 / PART C 录制导出）。与 Theatre.js、motion-showreel 互补。
- 第 17 项能力 `ai-design-skills/skills/landing-page-design/`：落地页 / 营销页完整系统——intake 提问、页面结构、布局选择、转化文案、SEO，外加严格视觉规则（字体 / 间距 / 圆角 / 背景 / hero / 图标 / 动效）；核心理念 one offer → one audience → one primary action。与 oil-ui、draw-ui 互补，补上「转化率」这块拼图。

**变更（深入嫁接，非仅入表）**
- 内置工作流新增接口⑥ `landing-page-design`（落地页 / 营销页场景，出稿前定转化结构与文案）与接口⑦ `design-to-motion` 作为第五步·动效展示导出（设计稿 / 出码后生成会动的 MP4 / GIF）。
- 全局铁律新增 1 条：15 一页一意图（landing-page-design，禁止首屏多 CTA、背景渐变、单侧卡片描边、正文连字符 / 斜体 / 900 字重）。
- README 与 SKILL.md 同步：能力表 15 → 17、frontmatter description / tags、决策树、触发词索引、「与其它技能的关系」（二者定位为设计演示与转化引擎）、组合模式 / 工作流新增接口⑥⑦；版本号 1.2.0 → 1.3.0。

## v1.2.1 — 2026-10-24

**更名**
- 技能全局更名：`CHT-UI-SKILLS` → `cht-ui-skill`（目录名、SKILL.md `name` 字段、README 安装指令、GitHub 仓库 slug 全部统一为小写 `cht-ui-skill`，保持目录名 == `name` 字段）。
- GitHub 仓库 `cuohuatang/CHT-UI-SKILLS` → `cuohuatang/cht-ui-skill`（旧 URL 自动重定向）。

## v1.2.0 — 2026-10-23

**新增（AI 审美三件套）**
- 第 13 项能力 `frontend-design/`（`anthropics/skills`，Anthropic 官方）：设计哲学底座——像设计工作室主设那样思考，主题优先、避默认字体、列出并避开 5 大 AI 默认陷阱、两遍流程（先 token 设计计划 → 审校 → 再写码）。
- 第 14 项能力 `taste-skill/`（`Leonxlnx/taste-skill`，name: design-taste-frontend）：研究方向引擎——`scripts/draw.mjs` 从 247 个策展站提炼的 20 个研究方向发牌，`library/` 提供 type/palette/hero/section 蓝图，`scripts/inspect.mjs` 真实浏览器实测，三宽度截图 + rubric + fix 的 look-and-fix 循环；含 11 篇 `references/` 方法论文档。
- 第 15 项能力 `garden-skills/`（`ConardLi/garden-skills`）：风格配方库 + 设计工程师全流程——`skills/web-design-engineer` 内置 25 种锚定风格配方（Linear/Aesop/Pentagram/Bloomberg/Stripe…）+ Step 0 事实核查 + Design Direction Advisor 模式；另含 `web-video-presentation`/`gpt-image-2`/`beautiful-article`/`kb-retriever`/`motion-showreel` 共 6 技能。

**变更（深入嫁接，非仅入表）**
- 内置工作流第一步新增「审美打底（接口④，frontend-design）」与「采集方向素材（接口⑤，taste-skill/garden-skills）」两步，收尾用 taste-skill look-and-fix 做实测验收闭环。
- 全局铁律新增 3 条：12 反 AI 默认陷阱（frontend-design 5 tells）、13 实测而非空想（taste-skill）、14 事实先于设计（garden web-design-engineer Step 0）。
- README 与 SKILL.md 同步：能力表 12 → 15、frontmatter description/tags、决策树、触发词索引、「与其它技能的关系」（三者定位为审美底座/方向引擎/配方库）、组合模式新增「AI 审美三件套」；版本号 1.1.1 → 1.2.0。

> 本版总结：嫁接 Anthropic frontend-design、Leonxlnx/taste-skill、ConardLi/garden-skills 为第 13/14/15 项能力，把「审美哲学 + 方向引擎 + 风格配方」深度织入内置工作流第一步与全局铁律，专治 AI 生成界面的「模板味 / AI 味」。

## v1.1.1 — 2026-10-21

**新增**
- 第 12 项能力 `superpowers/`：开发方法论（obra/superpowers，15 个组合式技能：brainstorming / writing-plans / test-driven-development / subagent-driven-development / systematic-debugging / verification-before-completion / code-review 等），含总入口 `SKILL.md`。

**变更**
- 内置工作流升级为「快速 / 工程」双模式（嫁接点①）：第三步新增工程模式——设计定稿后走 superpowers（计划 → TDD → 子代理执行 → 验证 → 评审）交付已验证代码。
- 第一步需求模糊时触发 `superpowers/brainstorming` 收敛（嫁接点②）；新增第四步「完成前验证」——声称完成前必须跑测试/构建并附证据（嫁接点③）。
- 全局铁律新增 3 条：TDD 不可跳过、计划先行、完成前验证（方案 C 铁律融合）。
- README 与 SKILL.md 同步：能力表 11 → 12、路由/决策树/分册索引/技能关系/铁律/工作流全量更新；版本号 1.1.0 → 1.1.1。

> 本版总结：嫁接 superpowers 开发方法论为第 12 项能力，内置工作流实现「设计（cht-ui-skill）× 工程（superpowers）」接口对接：需求模糊先头脑风暴、代码生成可切工程模式、完成前强制验证。

## v1.1.0 — 2026-10-20

**新增**
- 第 11 项能力 `m3e-canvas/`：可拖拽 UI 设计（AI 生成 Material 3 设计 JSON → 分享链接 → 侧边栏/浏览器拖改 → 导出 vibe-coding 提示词），含 `scripts/make_link.py` 与 M3E 协议全文 `references/agent-spec.md`。
- `CHANGELOG.md`：版本迭代记录。

**变更**
- 内置工作流第七节升级为「方案矩阵」：第一步从 oil-ui 3 套方向升级为「oil-ui 调性 × 8 大分册技术气质 × 交互形态」多维组合（默认 6–9 版，可出十几版）。
- 第二步增加分支选择闸门：分支甲 draw-ui 出静态精细稿（原路径）；分支乙 m3e-canvas 出可拖改原型（新路径）。
- 第三步分支乙路径：改完原型导出 prompt，按用户指令喂给 AI 代码生成（默认不自动执行）。
- README 与 SKILL.md 同步：能力表 10 → 11、路由/决策树/分册索引/技能关系全量更新；版本号 1.0.0 → 1.1.0。

> 本版总结：技能集由 10 大能力扩至 11 大，新增可拖拽 UI 设计能力，并将内置工作流升级为「风格×技术×形态」方案矩阵 + 双分支出稿。
