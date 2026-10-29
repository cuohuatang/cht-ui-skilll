# impeccable（嫁接来源）

来源仓库：[pbakaus/impeccable](https://github.com/pbakaus/impeccable)（⭐ ~92.8k）

「编码 Agent 的设计词汇表」：24 条设计指令（bolder/quieter/distill/critique/audit…）+ 62 条确定性反-slop 规则 + critique/audit 评审。

本目录为**参考型嫁接**：原仓库的引擎是 Rust CLI（`crates/`、`cli/`），无法在 skill 内运行，故只收其人读的设计词汇与规则文档：
- `references/` — README（24 指令说明）、DESIGN.md（设计系统参考）、STYLE.md、PRODUCT.md、NOTICE.md
- `assets/` — detector-config.json（slop 检测器规则配置）、design-system.json（设计 token，含 kinpaku 暗色系统色板）

完整引擎与实时模式见上游 `npx impeccable install`。
