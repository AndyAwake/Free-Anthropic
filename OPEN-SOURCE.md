# 开源与相关项目目录

[返回 README](README.md) · [五类工作流与比较方法](WORKFLOWS.md) · [实际选择记录](selection.csv)

核对日期：**2026-11-14（北京时间）**。以下均读取了官方 GitHub 仓库、README 和许可证；**没有安装、没有逐项验证国内下载，也没有跑出与 Claude 的性能胜负**。

先区分三层：**模型**负责生成与理解；**客户端/平台**负责会话、文件和工作流；**推理服务**可能是国内 API、云服务或自己的电脑。换一个开源界面，不会自动改变实际模型，也不会自动消除 API、硬件、部署和维护成本。

## 先按要做的事选

| 你的需求 | 候选 | 为什么列在这里 | 先做哪项验收 |
| --- | --- | --- | --- |
| 在一个桌面工具里接不同模型、写作和读资料 | Cherry Studio | 桌面多模型工作台 | WORKFLOWS 的文章或摘要 |
| 将一小批资料整理成可检索问答空间 | AnythingLLM | 文档处理、检索和对话 | 同一原料的摘要与证据表 |
| 给自己搭统一对话入口 | LibreChat | 可自托管、配置多个服务端点 | 同一份文章与源文件导出 |
| 想在本机运行合适大小的模型 | Ollama | 本地模型运行工具和 API | 先做纯文本摘要，再看速度与质量 |
| 固定输入反复提取成固定格式 | Dify | 可视化模型应用与工作流平台 | 同一资料输出证据 CSV |
| 需要自己的浏览器式模型入口 | Open WebUI | 接本地或兼容 API 的自托管界面 | 相同资料的对话、来源与结果保存 |

前四项使用标准开源许可证；后两项的当前许可证有附加条件，单独说明。表中的任务是本项目建议的试跑方式，不是已证实的效果排名。

## 标准开源许可候选

### Cherry Studio：多模型桌面工作台

- 官方：[CherryHQ/cherry-studio](https://github.com/CherryHQ/cherry-studio) · [README](https://github.com/CherryHQ/cherry-studio/blob/main/README.md) · [LICENSE](https://github.com/CherryHQ/cherry-studio/blob/main/LICENSE)。
- 用途核对：Windows、macOS、Linux 桌面工作台，提供模型服务配置、对话、资料库和 Agent 等能力。
- 当前仓库许可：**AGPL-3.0**；不是 MIT。实际使用或修改发行时读取对应版本原文。
- 成本：客户端之外还要计算选用模型的 API/订阅或本地运行成本。知识库另涉及嵌入、解析等配置。
- 状态：本次官方仓库未归档；这里不承诺某个安装包在你的机器上可用。

**第一轮怎么试：** 从仓库 README 的官方下载安装入口开始 → 在模型服务设置中选你的国内供应商或适配的自定义服务 → 填自己的端点、Key 和模型 → 新开对话粘贴共同原料包 → 做 WORKFLOWS 第 1 或第 2 项 → 保存结果并记录实际模型、成本与修改。先用纯文本，再单独验收文件解析和工具能力。

### AnythingLLM：资料与模型放进同一个工作空间

- 官方：[Mintplex-Labs/anything-llm](https://github.com/Mintplex-Labs/anything-llm) · [README](https://github.com/Mintplex-Labs/anything-llm/blob/master/README.md) · [LICENSE](https://github.com/Mintplex-Labs/anything-llm/blob/master/LICENSE)。
- 用途核对：提供文档导入、资料检索、对话与 Agent，可连接本地或云端模型；有桌面与自托管路线。
- 当前仓库许可：**MIT**。模型、第三方服务与素材仍各有自己的使用条件。
- 成本：生成模型、嵌入模型、向量存储，以及安装和维护时间分别计算。不要把「应用在本地」写成所有模型请求都留在本机。
- 状态：本次官方仓库未归档。不同安装形式的功能可能不同。

**第一轮怎么试：** 走 README 的桌面下载或自托管说明 → 建一个只含公开样例的小工作空间 → 明确生成模型和嵌入模型各使用谁 → 导入 `source.md` → 按 WORKFLOWS 第 2 项问第三产业增速、资料年份和资料没有提供的内容 → 对照来源检查。检索到文件不等于答案有正确出处，证据表仍要逐项回查。

### LibreChat：自己的统一会话入口

- 当前官方：[LibreChat-AI/LibreChat](https://github.com/LibreChat-AI/LibreChat) · [README](https://github.com/LibreChat-AI/LibreChat/blob/main/README.md) · [LICENSE](https://github.com/LibreChat-AI/LibreChat/blob/main/LICENSE)。旧 `danny-avila/LibreChat` 地址本次会跳转至这里。
- 用途核对：自托管对话与多模型入口，README 提供兼容 API 的自定义端点配置路线。
- 当前仓库许可：**MIT**。
- 成本：运行环境、数据库和维护，以及所接服务的推理/文件工具费用。自托管入口不是免费模型订阅。
- 状态：本次官方仓库未归档。

**第一轮怎么试：** 按 README 的安装说明在自己的测试环境启动 → 用官方文档配置自定义服务端点 → 明确选定实际国内模型 → 把共同原料包粘贴到新对话 → 做一篇文章和摘要 → 检查成品保存、再打开和模型记录。文件搜索、代码执行等能力分开验收，不由基础聊天成功推断。

### Ollama：在本机运行模型

- 官方：[ollama/ollama](https://github.com/ollama/ollama) · [README](https://github.com/ollama/ollama/blob/main/README.md) · [LICENSE](https://github.com/ollama/ollama/blob/main/LICENSE)。
- 用途核对：模型运行工具，提供本地运行与 API；仓库也介绍云模型能力，选择时要区分。
- 当前仓库许可：**MIT**。**Ollama 工具的许可不等于所有模型权重的许可。** 下载某个模型时另看其模型卡与许可。
- 成本：模型下载、磁盘、内存/显存、电力和自己的维护时间；使用云模型则另算云服务费用。
- 状态：本次官方仓库未归档；没有验证当前电脑的硬件或推理速度。

**第一轮怎么试：** 从 README 进入官方安装与模型目录 → 按本机内存/显存选一个明确标为本地运行、大小合适的模型 → 记录完整模型标签、量化、下载大小和机器配置 → 输入 `source.md` 做短摘要 → 验收数字和原文未提供问题，再记录等待和人工修改。不要把云模型结果填成本机模型成绩；模型太大就改选合适配置或回到国内 API，不先购买新硬件。

## 许可有附加条件的相关项目

### Dify：把重复任务画成工作流

- 官方：[langgenius/dify](https://github.com/langgenius/dify) · [README](https://github.com/langgenius/dify/blob/main/README.md) · [LICENSE](https://github.com/langgenius/dify/blob/main/LICENSE)。
- 用途核对：模型应用、工作流、检索管线、Agent 和模型配置；有自托管路线。
- 当前许可：**Dify Open Source License，基于 Apache-2.0 并有附加条件**，涉及多租户与前端标识等，不能简写成无附加条件的 Apache-2.0。
- 成本：平台部署、数据库/存储、模型与插件调用、维护时间。云端托管服务和自行部署分别计算。
- 状态：本次官方仓库未归档；未测试插件、国内镜像下载和账号权益。

**第一轮怎么试：** 按当前 README 的自托管说明建测试实例 → 配置自己可用的国内模型服务 → 建「输入文字 → 模型提取 → 输出」的最小工作流 → 输入共同原料包 → 输出 WORKFLOWS 第 2 项的证据 CSV → 下载并验收 → 保存工作流配置、实际模型和运行记录。再用另一份同结构资料验证可复用，之后再考虑团队应用。

### Open WebUI：自托管模型界面

- 官方：[open-webui/open-webui](https://github.com/open-webui/open-webui) · [README](https://github.com/open-webui/open-webui/blob/main/README.md) · [LICENSE](https://github.com/open-webui/open-webui/blob/main/LICENSE) · [历史许可](https://github.com/open-webui/open-webui/blob/main/LICENSE_HISTORY)。
- 用途核对：自托管对话界面，可连接 Ollama 或兼容 API；「可自托管」不保证你接的服务离线可用。
- 当前许可：**Open WebUI License**，含品牌保留条款与相应例外，历史贡献还涉及原有许可。不能把当前全部代码直接标为 MIT/BSD。
- 成本：部署与维护、本地模型资源或 API、可选资料处理服务的费用。
- 状态：本次官方仓库未归档；未验证安装和实际对话。

**第一轮怎么试：** 按 README 选择一种安装路线 → 接入明确选定的本地模型或国内兼容服务 → 新建对话，使用同一份公开原料完成摘要 → 验收数字、来源和结果保存 → 记录端点、模型与用量。安装界面打开，只能证明平台启动，不能证明模型和文件能力都可用。

## 历史参考：Flowise

[FlowiseAI/Flowise](https://github.com/FlowiseAI/Flowise) 的官方仓库本次明确标记为 **已归档**，README 也写明归档；不列为本项目新手默认安装路线。[LICENSE.md](https://github.com/FlowiseAI/Flowise/blob/main/LICENSE.md) 说明一般部分为 Apache-2.0，同时部分企业目录和指定文件适用商业许可，不能只摘 README 的简写。

保留这条是为了帮助使用旧教程的人识别当前状态，不据此判断旧部署是否仍能运行。

## 本次核对版本

以下是核对时默认分支的提交，用来定位资料。安装时按自己选择的发布版本重新读取 README 与许可，不把开发分支提交当成推荐安装版本。

| 官方仓库 | 核对提交 | 对应许可快照 |
| --- | --- | --- |
| CherryHQ/cherry-studio | `9952477297bea3deba0122ab496b0060c6909f47` | [LICENSE](https://github.com/CherryHQ/cherry-studio/blob/9952477297bea3deba0122ab496b0060c6909f47/LICENSE) |
| Mintplex-Labs/anything-llm | `4d09fa5f730698d39f1d783e47316744b260a700` | [LICENSE](https://github.com/Mintplex-Labs/anything-llm/blob/4d09fa5f730698d39f1d783e47316744b260a700/LICENSE) |
| LibreChat-AI/LibreChat | `fad2c51da41bb46c9cdd44a720cea4df0d47876b` | [LICENSE](https://github.com/LibreChat-AI/LibreChat/blob/fad2c51da41bb46c9cdd44a720cea4df0d47876b/LICENSE) |
| ollama/ollama | `a5864fcb33969705de3c0ebfedf4b2a16c970bcc` | [LICENSE](https://github.com/ollama/ollama/blob/a5864fcb33969705de3c0ebfedf4b2a16c970bcc/LICENSE) |
| langgenius/dify | `1ee97a71474f78ffff36bf25d1e09531eff9830b` | [LICENSE](https://github.com/langgenius/dify/blob/1ee97a71474f78ffff36bf25d1e09531eff9830b/LICENSE) |
| open-webui/open-webui | `b0e6098e940942281d9c83f3529ea117287a3a22` | [LICENSE](https://github.com/open-webui/open-webui/blob/b0e6098e940942281d9c83f3529ea117287a3a22/LICENSE) |
| FlowiseAI/Flowise（已归档） | `9291856d1ea4a4ceea9f8fef8ce14f4f6c81e8eb` | [LICENSE.md](https://github.com/FlowiseAI/Flowise/blob/9291856d1ea4a4ceea9f8fef8ce14f4f6c81e8eb/LICENSE.md) |

## 如何补充项目与比较结果

先提供官方仓库和 README、许可、核对日期、要替代的具体任务，再提交实际输入、模型与执行环境、产物、验收、人工修改和成本。已有 Claude 基线才做同任务对照，没有基线就比较可用方案，不填写想象中的 Claude 成绩。

目录收录是候选资格，任务验收才决定是否进入你自己的常用工具列表。
