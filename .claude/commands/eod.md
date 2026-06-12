---
description: 收尾命令——更新 WORKLOG、沉淀经验、提议 commit
---

执行 alcoholic 项目的 AgentOS 会话收尾流程。步骤：

1. **总结本次会话** —— 2~5 条要点，做了什么、为什么。要具体（文件、酒款、
   结论），链接到实际文件而不是重复内容。

2. **追加 WORKLOG** —— 在 `project_management/WORKLOG.md` 顶部（`---` 之下、
   最新条目之上）新增一条带日期的记录。保持简短，它是索引不是全文。

3. **沉淀持久知识** ——
   - 项目相关的事实（用户偏好、品评体系决定）→ Claude memory（写文件并在
     MEMORY.md 加一行）。本会话已存过的跳过。
   - *可泛化的工作流*经验（跨项目可复用的流程洞察，非品酒知识）→ 在
     `project_management/agentos_lesson_candidates.md` 加一行。未经用户明确
     批准，不得上报到 AgentOS hub。

4. **展示变更** —— 运行 `git status` 和简短的 `git diff --stat`，列出将要
   提交的文件。

5. **提议 commit** —— 起草简洁的中文 commit message，请用户确认后再提交。
   默认分支 `main`。

6. **push 前确认** —— 这是**公开仓库**（DavidQyz/alcoholic），push 即发布。
   品鉴记录公开是有意为之，但 push 前仍需：确认用户意图；检查 diff 中没有
   个人身份信息、行程细节之外的隐私内容或任何凭据。

保持轻量。如果本次没有实质性变更，直接说明并跳过 commit。
