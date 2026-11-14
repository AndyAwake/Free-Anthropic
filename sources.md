# 官方资料与核对范围

[返回 Free-Anthropic](README.md) · [开源项目目录](OPEN-SOURCE.md)

核对日期：**2026-11-14（北京时间）**。本表记录公开官方资料，产品版本、价格、限时活动和地区条件可能变化，实际使用前重新核对。

本版完成了官方文档阅读、公开示例数据校验、项目内文件链接检查及参考脚本验证；没有用豆包、Kimi、WorkBuddy 的登录账号逐项运行五类任务，没有完成真实 API 计费调用，没有客户成交数据。`selection.csv` 是待执行模板，运行结果栏保持空白。

## 工具、模型与费用

| 编号 | 官方来源 | 本版采用的事实 | 核对边界 |
| --- | --- | --- | --- |
| D1 | [豆包官网](https://www.doubao.com/chat/) · [下载](https://www.doubao.com/download) | 使用官方应用和下载入口；不引用其他相似域名作为官网 | 公开页面动态渲染，未获取登录后功能清单；不写当前模型型号、固定免费额度或上传上限 |
| K1 | [Kimi 文档与表格功能说明](https://www.kimi.com/help/docs-and-sheets/docs-and-sheets-overview) | 官方提供文档与表格入口，说明文档生成及数据处理能力 | 功能说明不证明样例已完成；账号权益、下载成功及文件实际质量另验 |
| K2 | [Kimi API 介绍](https://www.kimi.com/help/kimi-api/api-overview) | 官方开放平台提供模型 API；兼容格式不改变实际提供商 | 不以应用会员权益推断 API 额度；不硬编码当前旗舰型号 |
| K3 | [Kimi API 计费](https://www.kimi.com/help/kimi-api/api-pricing) | 输入与输出 token 计费，附加工具可能另收费 | 未做余额或账单调用，不填写实际成本 |
| W1 | [WorkBuddy 模型配置](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Function-Description/Model) | 国内文档列举内置模型及自定义 API；内置模型下线存在自动切换规则，自定义模型不按该规则替换 | 文档列有 Hy4 preview、GLM-5.3、Kimi-K3、Deepseek-V4-Pro 等，不代表每账号可用；未查看任何账号当前选择，也未触发回退 |
| W2 | [WorkBuddy 定价](https://www.codebuddy.cn/docs/workbuddy/Pricing) | 有体验与付费版本；不同权益与用量规则需要分别核对 | 不固化限时赠送、价格和可用额度；不将自定义 API 当成内置免费权益 |
| W3 | [WorkBuddy 更新日志](https://www.codebuddy.cn/docs/workbuddy/Changelog) | 入口与版本会变化，需按当前客户端找任务及模型设置 | 本次日志有 5.11.0 灰度条目，未断言已对全部账号发布 |
| W4 | [WorkBuddy 文件处理实践](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-One) | 官方提供文件输入、纪要整理等工作范例 | 本项目用自建公开原料练习，不复制官方范例为实测结果 |
| W5 | [WorkBuddy 数据分析实践](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-Three) | 官方说明可提交表格并要求分析、图表及报告 | 计算与文件输出仍需本机复核 |
| W6 | [WorkBuddy 本地应用实践](https://www.codebuddy.cn/docs/workbuddy/From-Beginner-to-Expert-Guide/Practice-Cases/Practice-Seven) | 官方提供自然语言开发本地应用路线 | 本地打开和正式部署分别验收 |
| A1 | [火山方舟模型价格](https://docs.volcengine.com/docs/ark/model-pricing?lang=zh) | 模型、输入输出、工具及服务类型有不同计费项 | 不承诺固定价格和试用额度，实际开通与账单未测 |
| A2 | [阿里云百炼模型服务概览](https://help.aliyun.com/zh/model-studio/what-is-model-studio) | 提供模型 API 和兼容接口接入说明 | 端点、地域、业务空间与套餐需配套；本版不抄用旧端点当通用配置 |
| A3 | [DeepSeek 首次调用](https://api-docs.deepseek.com/zh-cn/) · [模型与价格](https://api-docs.deepseek.com/zh-cn/quick_start/pricing/) | 官方服务支持兼容格式；当前标识和费用查对应文档 | 官方还说明部分旧模型名可能映射到新模型，因此不能用请求别名证明固定底层版本；本版没有 API 调用成绩 |

## 地区支持

| 编号 | 官方来源 | 本次观察 | 写法边界 |
| --- | --- | --- | --- |
| R1 | [Gemini Web 支持地区](https://support.google.com/gemini/answer/13575153?hl=zh-Hans) | 中国大陆条目标注「仅限 Workspace」 | 不写成普通个人账号在大陆普遍可直接使用；也不忽略 Workspace 特例 |
| R2 | [Google AI Studio 与 Gemini API 地区](https://aistudio.google.com/docs/available-regions) | 地区列表单独列示，本次未列中国大陆 | 不把 Web/Workspace 支持推导成 AI Studio/API 支持 |
| R3 | [ChatGPT 支持地区](https://help.openai.com/en/articles/7947663-chatgpt-supported-countries) | 本次未列中国大陆 | 不把可访问某个网页等同于官方服务支持 |
| R4 | [OpenAI API 支持地区](https://help.openai.com/en/articles/5347006-openai-api-supported-countries-and-territories) | 本次未列中国大陆，官方说明未列地区不受支持 | 与 ChatGPT 分开核对；不推荐为大陆普通用户的默认路线 |

## 公开练习原料

**S1：[国家统计局关于 2024 年国内生产总值最终核实的公告](https://www.stats.gov.cn/sj/zxfbhjd/202512/t20251226_1962144.html)，2025-12-26。**

读取官方 HTML 中的附件 1，核对 GDP 与三次产业四行：

| 项目 | 现价总量（亿元） | 不变价增速（%） | 产业结构（%） |
| --- | ---: | ---: | ---: |
| GDP | 1348066 | 5.0 | 100.0 |
| 第一产业 | 91636 | 3.7 | 6.8 |
| 第二产业 | 490305 | 5.0 | 36.4 |
| 第三产业 | 766125 | 5.1 | 56.8 |

只使用这个四行历史数据快照。原表另外列出行业，不能把各级分类全部加在一起。WORKFLOWS 的三次产业合计为 1348066；占比由本项目自行计算。网页工具抓取该站曾超时，随后用直接公开 HTTP 读取正文及表格成功；不能把前面的超时说成原文不存在。

公开来源用于练习，不代表国家统计局推荐本项目或任何产品。仓库 MIT 许可仅适用于本项目原创部分，第三方资料按其自身规则使用。

## 星觉科技入口与项目导航

- 产品：[IPClaw](https://metaver.vip/ipclaw)、[产品介绍](https://metaver.vip/products)。
- 服务：[星觉科技服务站](https://www.a6no1.cn/services)。
- 入口文案参考[Anti-Anthropic 的 COMPANY.md](https://github.com/AndyAwake/Anti-Anthropic/blob/main/COMPANY.md)，仅使用「星觉科技」称呼。
- [Out-Anthropic](https://github.com/AndyAwake/Out-Anthropic)、[Anti-Anthropic](https://github.com/AndyAwake/Anti-Anthropic)。

以上服务和产品链接本次返回公开页面；没有据此认定购买、预约、付款或咨询交付已经发生。主对话负责远程仓库创建与发布；本项目文件编写不等于这些仓库已经上线。

## 开源与相关项目核对

目录与许可证据见 [OPEN-SOURCE.md](OPEN-SOURCE.md)。已通过 GitHub 连接器读取 7 个官方仓库的元数据、README 与 LICENSE，并记录默认分支提交用于定位：4 个标准开源许可候选、2 个许可含附加条件的相关项目、1 个已归档的历史项目。

这里的核对是仓库存在、用途、维护状态与许可文本核对，不是下载、安装、国内访问或性能测评。未安装这些项目，也未声称它们全面胜过 Claude。

## 本版文件验证

项目内 18 处相对链接已解析到现有文件；CSV 模板可正常解析为 12 行、29 列。参考 Python 代码和 CSV 已实际运行：正常输入与重复运行通过；原料未改变；缺少一行、错误年份的副本分别被拒绝。实际应用、各客户端与 API 的端到端任务未运行。

`selection.csv` 是待执行模板，运行日期、模型实测、费用、耗时及验收结果栏保持空白。未使用浏览器界面，未操作登录账号，未创建或推送远程仓库。
