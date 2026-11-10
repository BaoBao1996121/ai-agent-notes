# AI Agent 工程学习笔记

从理解一个工具调用循环，到组织知识、设计验证，再到审视自优化实验。这里整理的是学习中反复用到的解释、例子与纠错记录。

**适合谁**：会写一点程序，希望理解 Agent 为什么能工作、什么时候不可靠、怎样判断改动有没有价值的人。

这不是产品排行榜，也不是“从零到生产”的完成证书。每篇围绕一个具体问题展开，附练习和判断边界。内容由个人 Obsidian 笔记经 AI 协助整理、校订；上游概念、个人归纳和实验结果分别注明。

## 从哪里开始

| 路线 | 阅读内容 | 读完应能做什么 |
|---|---|---|
| 先理解系统 | [01 Agent 循环](notes/01-agent-loop.md) → [02 工作流组合](notes/02-workflow-patterns.md) | 画出一次工具调用，选择简单且合适的控制方式 |
| 再管理信息 | [03 上下文工程](notes/03-context-engineering.md) → [04 知识与记忆](notes/04-knowledge-and-memory.md) | 解释索引、原文、检索与持久状态各自的职责 |
| 最后约束和验证 | [05 Skill 工程化](notes/05-skill-engineering.md) → [06 评估](notes/06-evaluation.md) → [07 长任务可靠性](notes/07-long-running-agents.md) | 写出验收条件，识别假提升，留下可接续的工作状态 |

只想看一次真实探索，可以直接读 [“同一版本上涨了 6.7 个百分点”](https://github.com/BaoBao1996121/agent-evolution-lab/blob/main/docs/findings.md)。

## 这套积累的四个入口

| 仓库 | 解决的问题 |
|---|---|
| **本仓库：学习笔记** | 概念怎样连起来，哪些直觉需要修正 |
| [agent-engineering-playbook](https://github.com/BaoBao1996121/agent-engineering-playbook) | 选型、源码分析、跨会话交接怎样实际开展 |
| [agent-evolution-lab](https://github.com/BaoBao1996121/agent-evolution-lab) | 怎样用代码、结果文件和反例审视“自优化” |
| [ai-research-archive](https://github.com/BaoBao1996121/ai-research-archive) | 完整一些的历史积累：RAG、Agent、记忆、模型、评估与部署，378 份文档及配套文件 |

## 积累是怎样发生的

原教程的文件日期为 **2026-04-12**；后续实验归档形成于 **2026-11-05 至 11-06**；这一公开整理版于 **2026-11-09** 建立。前两者来自本地材料自带日期，不是第三方时间认证；Git 提交记录使用真实发布时间，不补造历史提交。

[探索记录](JOURNEY.md) 说明思路怎样变化，[修订说明](EDITORIAL_NOTES.md) 记录这次撤回或收紧了哪些说法，[来源清单](PROVENANCE.md) 给出对应原稿和快照校验值。

## 使用与反馈

可以从任意一篇开始。练习使用自己的虚构数据或获准处理的材料。发现错误时，请在 Issue 中给出文章位置、反例和可核验来源；不要提交密钥、个人聊天记录或工作内部文档。

公开可见不等于上游材料的版权发生转移。本轮未对整套材料添加统一再许可，见 [内容与权利说明](CONTENT_POLICY.md)。
