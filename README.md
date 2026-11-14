# Free-Anthropic

<!-- ANDYAWAKE_V4_START -->
## Claude 平替工具与工作流 · 开源实操网站

**给正在使用 Claude / Claude Code 的人：先保全自己的资料和工作成果，再按任务找到可用替代，最后把优秀方法沉淀为自己掌握的工程资产。** 不强迫弃用某款 AI，也不要求先加微信才能获得教程。

- [打开完整交互网站](https://andyawake.github.io/Free-Anthropic/)
- [在线阅读全文手册](https://andyawake.github.io/Free-Anthropic/#main-content) · [下载全文 PDF](https://andyawake.github.io/Free-Anthropic/assets/guide.pdf)
- 关联：[数据迁移](https://github.com/AndyAwake/Out-Anthropic) / [寻找平替](https://github.com/AndyAwake/Free-Anthropic) / [方法学习与证据](https://github.com/AndyAwake/Anti-Anthropic)

教程免费，模板公开。作者 AI 酋长 Andy / 星觉科技。公司官网：[www.a6no1.cn](https://www.a6no1.cn/)。
<!-- ANDYAWAKE_V4_END -->

**换一套能用的 AI，继续把工作做完，把交付做出来。**

这是面向中文用户的 AI 替代实操手册：优先选择国内正常提供服务的豆包、Kimi、WorkBuddy 和国内 API，用具体任务决定工具。这里的 Free 是选择和切换的自由，**不代表所有工具免费**。这里收集模型服务、工作工具与相关开源项目，帮助你按自己的任务选择替代方案。

你不需要先学会写程序。先用一份公开资料完成文章或表格，再决定是否需要自动化、付费订阅和 API。

资料核对日期：**2026-11-14（北京时间）**。本版核对了公开官方文档，提供操作流程和验收标准；没有替任何账号做付费操作，也没有声称完成各工具的登录实测、速度排名或收入验证。文中的工具分工是尝试顺序，不是测评结论。

## 第一次来，按这个顺序做

1. 只想今天继续写东西：打开 [豆包](https://www.doubao.com/chat/) 或 [Kimi](https://www.kimi.com/)，用自己的账号登录。先做一个小任务，不必先购买套餐。
2. 在电脑新建 `AI工作样例` 文件夹，里面建 `input`、`output` 两个子文件夹；原料放前者，成品放后者。
3. 打开 [WORKFLOWS.md](WORKFLOWS.md)，复制「共同原料包」里的公开资料和需求卡，选一个任务照做。
4. 按该任务的验收逐项检查，下载文件并用自己的办公软件打开。聊天中出现文件名不等于文件已经保存。
5. 在 [selection.csv](selection.csv) 填一行实际结果。合格就先用它；不合格，把同一份输入交给备用工具比较。

这次先完成一个可检查的成品。确认经常需要处理同类工作后，再看订阅和 API。

## 三个项目，各管一件事

| 你要做什么 | 去哪里 |
| --- | --- |
| 了解背景、政策、公开证据与回应 | [Anti-Anthropic](https://github.com/AndyAwake/Anti-Anthropic) |
| 曾经或正在使用 Claude，想备份、迁出并减少依赖 | [Out-Anthropic](https://github.com/AndyAwake/Out-Anthropic) |
| 想找平替，按真实任务选择模型、工具和工作流 | 当前项目 Free-Anthropic |

旧数据需要迁出时先去 Out-Anthropic。新任务不必等待全部历史迁移完：把当前任务必要的背景、原料和验收单独保存，就能换工具继续做。

## 按工作挑工具

| 当前需要 | 建议先试 | 备用路线 | 最后留在自己手里的东西 |
| --- | --- | --- | --- |
| 写通知、文章、产品介绍 | 豆包或 Kimi | 另一款国内助手 | TXT/Markdown、定稿 Word |
| 读文档、摘数据、做有出处的摘要 | Kimi | 豆包；本地文件较多可试 WorkBuddy | 摘录表、来源、摘要 |
| 清理表格、计算、图表 | Kimi 表格或 WorkBuddy | 助手输出 CSV，再用 Excel/WPS 算 | CSV、含公式的表格、口径说明 |
| 内容获客、整理服务样品 | 豆包或 Kimi | WorkBuddy 批量整理成品文件 | 内容包、需求表、服务说明 |
| 简单网页、重复处理脚本 | WorkBuddy + 明确选择的国内模型 | Kimi；国内 API 配合自己的脚本 | HTML/源码、输入输出样例、运行说明 |
| 把已验证的重复任务接入程序 | 国内官方 API | 换另一家官方 API，用同一输入重跑 | 配置说明、用量记录、可重跑流程 |

这是本项目给出的工作分配建议。官方能力入口见 [豆包下载页](https://www.doubao.com/download)、[Kimi 文档与表格](https://www.kimi.com/help/docs-and-sheets/docs-and-sheets-overview)、[WorkBuddy 文件处理](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-One)、[数据分析](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-Three)和[本地应用](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-Seven)。具体文件格式、文件大小和当前权益，使用前在相应产品里核对。

### 豆包：先把一段工作做完

从 [豆包官网](https://www.doubao.com/chat/) 进入；需要桌面端时走[官方下载](https://www.doubao.com/download)。新建对话，粘贴原料和要求，先让它列出读到的关键事实，再写成品。网页读取失败就自己打开原文，复制所需段落或上传保存的文件。

拿到文字后复制到本地 TXT 或 Markdown，或放进 Word/WPS 排版。需要表格时可以先要 CSV 文本，再自己保存为 `.csv` 打开。当前界面没有导出按钮，也能完成这条路线。不要把豆包应用的使用权益当成火山方舟 API 额度。

### Kimi：把原料和最终文件一起交清楚

从 [Kimi 官网](https://www.kimi.com/) 进入，上传文件或粘贴原文。做文档、表格时可使用相应功能入口；官方说明提供[文档与表格操作指引](https://www.kimi.com/help/docs-and-sheets/docs-and-sheets-overview)。先确认读到的文件、页码或章节，再要最终文件。

下载后用本机 Word/WPS/Excel 打开，查数字、公式和排版。暂时无法下载时先保存文字/CSV，再另做排版。Kimi 应用、Kimi Code、开放平台属于不同产品入口，费用和适用范围要分别看；[API 介绍](https://www.kimi.com/help/kimi-api/api-overview)和[API 计费](https://www.kimi.com/help/kimi-api/api-pricing)不能用聊天会员权益替代。

### WorkBuddy：先核对模型，再让它动手

WorkBuddy 是工作工具，底层模型需要另外确认。[国内官方模型文档](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model)在本次核对时列有 Hy4 preview、GLM-5.3、Kimi-K3、Deepseek-V4-Pro 等；列表会变，不代表每个账号都能选到。

官方还说明：内置模型下线后优先切同系列新模型，否则用默认模型；定时任务也会在运行前切换。自定义模型不会被这样自动替换；任务已发出后失败不保证再换模型。**Auto、快速、均衡等档位不是具体模型身份。**

1. 从[国内官方入口](https://www.codebuddy.cn/)进入 WorkBuddy 下载/文档，确认所用版本和登录站点；不要混用国际版经验。
2. 新建任务，只指定刚建的样例文件夹。进入模型选择器，记录界面显示的完整模型名、版本、模式和日期。
3. 想减少对 Anthropic 的依赖，就明确选择当前可用的国内模型。若只看到 Auto，记为「实际模型未披露」，不要声称已经确定底层提供商。
4. 查看任务或请求的可见模型记录。只有选择器名称时记作「界面选择」，不能当成服务端运行证明；不要让模型自报身份来证明自己是谁。
5. 完成、重启、升级或恢复旧任务后，再看一次选择器及运行记录。若发生切换，记录切换前后名称；必要时重新做同一份样例验收。
6. 打开会员、积分或用量页，记录当前计费方式和执行前后用量。沿用你已经选择的计费模式；看不清收费时先查说明，不靠「听说限免」判断。

不要为了测试而主动卸载模型或制造付费失败。模型回退与费用规则分别见[模型配置](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model)、[定价详情](https://www.codebuddy.cn/docs/workbuddy/Pricing)。自定义 API 的费用另向其供应商结算。界面升级可能改变入口，参照[官方更新日志](https://www.codebuddy.cn/docs/workbuddy/Changelog)查找当前菜单。

## 国内 API：重复任务稳定后再接

API 适合「每次输入结构相同、输出也能验收」的工作。例如把多份公开资料提取为同一张表。普通写作先用网页或客户端即可。

| 官方服务 | 怎么选 | 官方依据 |
| --- | --- | --- |
| 火山方舟 / 豆包 API | 在控制台选已开通的模型或接入点，按对应接口文档接入 | [模型价格及计费入口](https://docs.volcengine.com/docs/ark/model-pricing?lang=zh) |
| Kimi 开放平台 | 选平台当前开放的模型，用对应 API Key 和地址 | [快速入门](https://www.kimi.com/help/kimi-api/api-overview) · [计费](https://www.kimi.com/help/kimi-api/api-pricing) |
| 阿里云百炼 / 千问 | 先选地域与业务空间，再复制对应地址和模型标识 | [模型服务概览](https://help.aliyun.com/zh/model-studio/what-is-model-studio) |
| DeepSeek 官方 API | 以官方首次调用页的地址和当前模型标识为准 | [首次调用](https://api-docs.deepseek.com/zh-cn/) · [模型与价格](https://api-docs.deepseek.com/zh-cn/quick_start/pricing/) |

具体操作：

1. 打开上表官方文档，再进入它链接的控制台。核对账户地区、计费方式、可用余额及模型权限。
2. 记录模型标识、服务端点、单价单位和核对日期；Token Plan/Coding Plan 与按量 API 的 Key、地址、用途不要混用。
3. 由你设定本次可接受的预算。平台提供限额时设置限额；仅有余额提醒时，不把它当成硬性停费开关。
4. 在客户端的官方供应商预设或自定义 API 中填入对应信息。密钥只填本地设置或环境变量，不放在公开 CSV、网页和仓库里。
5. 先跑一段公开原料，确认返回内容、模型记录和实际账单，再跑完整任务。聊天能返回不等于文件读取、工具调用也能用，要分别测到所需能力。
6. 输入、结果、用量留档。请求失败先看错误，不连续盲重试；重新提交可能产生新费用。

**使用 OpenAI 兼容格式，不等于使用 OpenAI 的模型或账户。** 例如 DeepSeek 官方文档说明可用兼容格式调用它自己的服务。更换提供商时也不能仅改一个名字：模型标识、文件能力、工具调用和输出格式都要重新核对。

## 想把工具掌握在自己手里

看 [开源与相关项目目录](OPEN-SOURCE.md)：Cherry Studio、AnythingLLM、LibreChat、Ollama，以及许可含附加条件的 Dify、Open WebUI。目录逐项链接官方仓库、README 和 LICENSE，说明用途、成本、维护状态和一个可尝试的小任务。已归档的 Flowise 单独列为历史参考。

开源客户端、模型权重、API 和云服务是不同层。选择一个客户端，仍要选择实际模型和执行环境；客户端允许接某个服务，也不代表你所在地区受该服务支持。GitHub/下载站点的国内访问与模型下载未逐一实测，不能把这份目录当成全部国内直连成功的清单。

不必为了找平替先部署一套平台。日常任务先走国内官方应用；确实需要自己的会话入口、资料库或重复工作流，再按目录选择一个项目试跑。

## 怎么比较，才知道是否适合自己的工作

不要比较两个工具随手生成的一段话。拿同一份公开输入、同一个交付要求、相同的修改机会，先按 WORKFLOWS 的五类任务验收，再记录实际费用与人工改稿时间。

如果已有 Claude 产物，就使用自己保留的原始需求、原料和成品作为基线；没有就比较两个可用替代方案，不为比较而新购账号或虚构 Claude 成绩。具体步骤见 [任务级比较方法](WORKFLOWS.md#8-任务级比较方法)，结果记入 [selection.csv](selection.csv)。本版没有证据声称任何候选全面胜过 Claude。

## Gemini / OpenAI：有官方支持条件再选

本项目的国内入门路线不依赖它们。所在地区、账户与所用产品符合官方支持条件的用户，可以用同一份原料和验收标准比较：

- Gemini Web、移动端、Workspace 与 Gemini API 的地区条件分别核对。[Gemini Web 官方地区页](https://support.google.com/gemini/answer/13575153?hl=zh-Hans)在本次核对时把中国大陆标为「仅限 Workspace」；这不能解释为普通个人账号在大陆普遍可直接使用。[AI Studio / Gemini API 地区页](https://aistudio.google.com/docs/available-regions)另列支持范围，不能由 Web 权益推断 API 权益。
- OpenAI 的 [ChatGPT 地区列表](https://help.openai.com/en/articles/7947663-chatgpt-supported-countries)与 [API 地区列表](https://help.openai.com/en/articles/5347006-openai-api-supported-countries-and-territories)本次核对均未列中国大陆。位于官方支持地区且满足账户条件时，再考虑对应产品。

## 从工作到接单：先定义交付物

客户付费购买的是完成的工作。先询问他现在哪件事反复耗时、已有何种原料、谁验收、用什么格式，再用本项目样例展示你能怎么做。

| 客户的具体需求 | 可以先谈的小单交付 | 开工前说清 | 可复购的下一次工作 |
| --- | --- | --- | --- |
| 小团队每周整理一堆材料 | 一份有来源的摘要 + 行动项表 | 文件数量、篇幅、截止日期、修订轮次 | 每周新材料整理 |
| 内容负责人缺稳定素材包 | 一篇定稿 + 三条改编短文 + 来源表 | 主题、口吻、渠道、谁提供事实与素材 | 按月主题与内容更新 |
| 门店或项目负责人报表混乱 | 整理后的表格 + 公式说明 + 异常清单 | 字段、统计口径、缺失值怎么处理 | 固定周期报表 |
| 咨询师需要展示服务 | 一页介绍网页源码 + 本地打开说明 | 文案、联系入口、页面数、修改范围 | 内容更新与维护 |
| 团队反复处理相同文件 | 可重跑脚本 + 样例 + 操作说明 | 输入格式、输出、运行环境、失败处理 | 新格式适配、维护 |

报价前先算：`交付成本 = 工具订阅分摊 + API/素材/托管实际费用 + 沟通/制作/核对/修改工时 × 你的工时成本`。双方约定的报价再覆盖预期利润与已约定维护。还没有数据时写「待估」，先记录样例耗时，不编造行业均价、成交数或月收入。

第一次只谈有明确范围的小单：对方确认需求卡 → 你展示公开样品 → 双方确定价格、时间、验收和修改次数 → 交付可编辑文件 → 记录实际成本与反馈。复购来自持续发生的工作和可靠交付，不从「买了 AI」自动产生。

## 如何留下自己的选择依据

[selection.csv](selection.csv)预置五类任务、一个 API 任务和六条开源/相关工具试跑记录，全部是**待执行模板**。没有填写任何虚构测评分数。

每次复制一行记录：相同输入、具体工具/模型、是否发生回退、费用、耗时、人工修改和最终产物。运行证据只保存不含密钥和私密数据的截图或记录。公开分享前检查文件内容，不把客户资料直接放进本仓库。

「模型未披露」「用量页尚未更新」「文件未能下载」都可以如实记录；不把未知填成零，也不把未运行填成通过。合格标准在 WORKFLOWS.md，结论写「继续用 / 换备用 / 需补测」即可。

## 星觉科技 · 产品与服务

用 AI 帮助企业增长，助力个人成长。

- [IPClaw](https://metaver.vip/ipclaw)：连接工作 Agent、专家 Agent 与真人专家。
- [MDskill 等产品](https://metaver.vip/products)：内容编辑与个人工具。
- [了解服务与合作](https://www.a6no1.cn/services)：个人 AI + IP 陪跑、职场人副业陪跑、企业 AI + IP 获客等。

微信：**AIPMAndy**，可备注「AI 替代工作流 + 你的具体任务」。

## 维护与许可

贡献时请提供：具体任务、官方来源、核对日期、输入与验收方式。测评另附实际运行证据，不靠模型自述或宣传文案打分。型号、价格和活动一旦变化，更新对应步骤和核对日期。

官方资料、仓库许可的核对范围和未实测部分见 [sources.md](sources.md)。

本仓库原创内容使用 [MIT License](LICENSE)。所链接的第三方资料、产品与商标仍按各自规则使用。
