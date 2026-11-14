# Claude / Claude Code 平替路线 · 按任务选，而不是按热度选

> 2026-11-14 编辑版。这里的「先试」是推荐尝试顺序，不是任何一家工具全面胜出。账号、地区、价格、API 与功能随时会变；相同品牌的网页、桌面端、CLI、API 权益不能混为一谈。

## 1. 从你的原工作出发

| 在 Claude 上做什么 | 第一轮候选 | 不付费或低门槛的尝试 | 保留什么 | 最容易失败的地方 |
| --- | --- | --- | --- | --- |
| 聊天、写文章、咨询摘要 | 账号可用的豆包 / Kimi；支持地区也可比较 ChatGPT / Gemini | 用一段公开素材免费或现有账号试做 | 事实、来源、风格、Markdown 原稿 | 长聊天记忆不等于可移入新工具 |
| Claude Projects / 长期知识库 | 工具的项目空间，或可控的本地资料目录 + 目标模型 | 先用一个 `PROJECT-HANDOFF.md` | 重要文件、索引、角色与验收 | 原上传附件常常不在官方聊天导出内 |
| Claude Code / 编程 Agent | Codex；WorkBuddy；适配自有模型的编程工作台 | 用小的公开 Git 项目跑回归测试 | Git 仓库、可移植项目上下文、Skills | Hooks / MCP / 权限 / 工具调用不兼容 |
| Agent 工作流 / 任务自动化 | WorkBuddy / 自建可审计流程 / 合法可用的 Agent 框架 | 先用一项手动编排任务 | 任务卡、输入输出、触发器、日志 | 重复执行、隐式模型回退和付费 |
| 文档、PDF 与表格 | Kimi / WorkBuddy / 支持范围内的文档工作台 | 公开原料一次试做 | 可编辑源文件、公式、抽查证据 | 美观但数字错、只有截图无源文件 |
| 内部资料保密或离线需求 | 组织批准的私有服务，或硬件允许时本地模型 | 先测试文本摘要与权限 | 数据目录、模型许可、审计记录 | 本地运行≠自动等于安全或免费 |

> 中国大陆与其他地区的可用条件不同。任何涉及 ChatGPT、Gemini 或 Anthropic 的方案，都以当期官方支持地区及具体产品为准；本项目不介绍规避访问控制的方法。

## 2. 同题比较，别让成本和误差藏起来

固定四类文件：`input/brief.md`、`input/source.md`、`output/final.*`、`evidence/acceptance.md`。用同一份输入、明确的人工作业时限及验证标准，让两个候选各完成一轮。记录真实模型、输入是否完整、输出可编辑、事实错误、文件可打开、权限和费用。未做的项目写「未测」。

**推荐用 P0 任务试跑**：如果上一家工具原来帮你整理一个产品网站，不必把全部 200 个对话迁入，只需要当前源码、产品定位、技术限制、已有决策和一个能验收的具体问题。

## 3. 平替不等于削弱能力：复用 Claude 值得学习的做事方法

- 先计划、后执行，把目标与验收写成文档。
- 用项目级指令固化规则；把规则从聊天窗口带回仓库。
- 用小的 `SKILL.md` 封装重复任务，不把上百个 Skills 一股脑灌入上下文。
- MCP 只授予任务需要的最小权限；读写分开测试。
- 通过测试、截图、diff 和运行日志决定是否通过，而不是听模型自报「完成」。

详见 [如何把 Claude Code 能力迁出来](https://github.com/AndyAwake/Out-Anthropic/blob/main/CLAUDE-CODE-MIGRATION.md) 和 [方法迁移手册](https://github.com/AndyAwake/Anti-Anthropic/blob/main/PORTABLE-CLAUDE.md)。

## 4. 作者的可复用项目：有链接，但不编测评成绩

| 项目 | 复用点 | 备注 |
| --- | --- | --- |
| [anthropic-claude-code-agent-handbook](https://github.com/AIPMAndy/anthropic-claude-code-agent-handbook) | Claude Code、Agent、Skills、MCP、企业团队实践 | 作者已有研究库；按仓库当前版本核对 |
| [DNASkill](https://github.com/AIPMAndy/DNASkill) | 上下文与长期知识沉淀 | 需保护个人数据；并非跨所有平台自动恢复 |
| [Andy-Video-Skill](https://github.com/AIPMAndy/Andy-Video-Skill) | 视频制作过程的输入、分镜、验收 | 可作为可复用任务卡的教学案例 |
| [FreeCover](https://github.com/AIPMAndy/FreeCover) | 内容制作链路中的可编辑封面资产 | 产品能力以各自 README 为准 |
| [FreeRedact](https://github.com/AIPMAndy/FreeRedact) | 内容图片处理中的敏感信息安全 | 不把公开输出等同于安全审计 |
| [FreePhoto](https://github.com/AIPMAndy/FreePhoto) | 图片处理/交付链路 | 实际功能按对应源码核对 |

## 5. 官方核验

- [Claude 账号数据导出](https://support.claude.com/en/articles/9450526-export-your-claude-data)
- [Codex 工程工作流与 AGENTS.md](https://developers.openai.com/cookbook/examples/codex/iterating-development-workflows-with-codex)
- [OpenAI Skills 规范](https://developers.openai.com/api/docs/guides/tools-skills)
- [Gemini CLI 上下文文件](https://geminicli.com/docs/cli/gemini-md/)
- [WorkBuddy 模型配置](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model)
