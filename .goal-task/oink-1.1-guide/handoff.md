# Handoff: OINK 1.1 与 Ask AI 建站入门指南

## 来源会话
- 原始会话 ID: `01a0c9c0-a17b-7e60-8014-b312f6997484`
- 原始任务名: 写作：OINK 1.1 与 Ask AI 建站入门
- 原始工作区: `~/.codex/worktrees/d61b/hugegraph-doc`
- 会话状态: 文章初稿与 8 张配图均已就绪并通过自主核验，因宿主机 Codex 达到使用上限而交接。

## 产物清单
1. **文章主体**: `oink-1.1-website-guide.md`
   - 面向没有建站经验、但会写代码/Markdown 的开发者。
   - 介绍 Hugo + OINK 1.1 + 可选 Ask AI（Kapa）的文档网站体系。
   - 包含市面文档库对比（Docsy 单独对比表，已剔除 Notion/语雀）。
   - 遵循 `writing-human` 规范（无套话口号，基于 HugeGraph 实际升级经验）。
2. **配图及 Prompt 记录**: `oink-1.1-illustrations/`
   - `01-build.png`: 构建与部署机制
   - `02-language-version.png`: 多语言与多版本
   - `03-maintenance.png`: 维护与定制边界
   - `04-ai.png`: Ask AI / Kapa 接入机制
   - `05-overview.png`: Markdown 到静态网站全景
   - `06-features.png`: 交互功能（目录、本地搜索、代码标签页、步骤、图表）
   - `07-publishing.png`: 多形态发布（网页、打印、RSS、llms.txt）
   - `08-optional-ai.png`: 本地搜索与可选 Ask AI 接入区分
   - `final-prompts.md`, `general-prompts.md`, `prompts.md`: 绘图 Prompt 记录

## 接力后续工作建议
- 根据主线需要，决定是否将该文章排版并整合入网站正式路由（如 `content/cn/docs/...` 或博客/社区板块）。
- 校验图片相对路径与网站静态资源目录映射。
- 最终合入 PR 前，从分支中清理 `.goal-task/oink-1.1-guide`。
