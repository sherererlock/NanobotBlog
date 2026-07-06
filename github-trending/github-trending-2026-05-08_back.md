# 🔥 GitHub 本周 Trending Top 15（2026-05-08）

> 数据来源：[github.com/trending?since=weekly](https://github.com/trending?since=weekly) · 每周五自动推送

---

1. TauricResearch/TradingAgents 🐍 Python
模拟真实交易公司运作模式的多智能体金融交易框架。不同于单一 LLM 直接给出交易建议，它将整个投研流程拆解为多个专职 Agent——基本面分析师、技术分析师、新闻研究员、风险管理员、交易执行员——各自独立分析后汇总决策，更接近真实机构的协作方式。适合研究 LLM 在金融领域的落地路径，也可作为多 Agent 协作架构的参考实现。
🔗 https://github.com/TauricResearch/TradingAgents

---

2. mattpocock/skills 🐚 Shell
TypeScript 教育领域知名博主 Matt Pocock 直接开源了自己的 `.claude` 目录，里面是他在实际工程项目中积累的 Claude Code Skills 集合。这些 Skills 不是教程示例，而是真实在用的生产级提示词与工作流，覆盖代码审查、重构建议、文档生成等高频场景。随着 Claude Code Skills 生态本周集中爆发，这个仓库成为开发者快速参考和复用的第一手资料。
🔗 https://github.com/mattpocock/skills

---

3. warpdotdev/warp 🦀 Rust
用 Rust 重写的新一代终端，本周正式开源。核心差异不在于界面美化，而在于将 AI Agent 能力原生嵌入终端工作流：支持自然语言描述意图后自动生成并执行命令、命令历史语义搜索、多会话并行管理，以及 Agent 模式下的自主任务执行。定位是"Agentic 开发环境"，面向习惯在终端工作的开发者，开源后迅速成为本周最热门的话题项目。
🔗 https://github.com/warpdotdev/warp

---

4. ruvnet/ruflo 🟦 TypeScript
专为 Claude 设计的 Agent 编排平台，核心能力是将多个 Claude Agent 组织成协作群体（Swarm），支持自主工作流调度、任务分发与结果聚合。内置 RAG 集成、自学习群体智能机制，并原生对接 Claude Code 和 Codex，适合需要构建复杂多 Agent 流水线的团队，提供企业级的可靠性与可观测性。
🔗 https://github.com/ruvnet/ruflo

---

5. soxoj/maigret 🐍 Python
OSINT（开源情报）工具，核心功能是"用户名追踪"：输入一个用户名，自动在 3000+ 个网站上搜索该账号是否存在，并聚合所有公开信息生成完整的数字画像报告。支持 HTML、PDF、JSON 等多种输出格式，内置账号关联分析。常用于安全研究、渗透测试前期侦察，以及个人隐私暴露面自查。
🔗 https://github.com/soxoj/maigret

---

6. virattt/dexter 🟦 TypeScript
面向金融研究场景的自主 Agent，专注于"研究"而非"交易"。能自动抓取 SEC 财报、财经新闻、分析师报告等多源数据，通过 LLM 进行交叉分析后输出结构化的投资研究报告，包含关键指标提取、风险点识别、竞争对手对比等模块。适合需要快速完成公司尽调或行业研究的投资从业者和量化研究员。
🔗 https://github.com/virattt/dexter

---

7. openai/symphony 💧 Elixir
OpenAI 开源的编码 Agent 任务编排框架，解决的核心问题是"如何管理大量并发的 AI 编码任务"。它将项目工作拆解为相互隔离的自主实现单元（Run），每个 Run 独立执行、互不干扰，团队通过统一界面管理任务状态，而不是盯着 Agent 逐行输出。选用 Elixir 构建，天然具备高并发和容错能力，适合大规模并行 Agent 任务的工程化场景。
🔗 https://github.com/openai/symphony

---

8. docusealco/docuseal 💎 Ruby
DocuSign 的开源自托管替代方案。提供完整的电子文档签署流程：创建 PDF 表单模板、发送签署邀请、收集多方签名、归档审计记录，功能覆盖 DocuSign 的核心使用场景。支持 Web 界面操作和 API 集成，数据完全存储在自己的服务器上，适合对数据主权有要求、不愿依赖第三方 SaaS 的企业和个人。
🔗 https://github.com/docusealco/docuseal

---

9. AIDC-AI/Pixelle-Video 🐍 Python
阿里巴巴 AIDC 团队开源的 AI 短视频全流程自动生成引擎。输入文本描述或参考图片，系统自动完成脚本生成、AI 配音、字幕合成、画面生成与剪辑合成，输出可直接发布的短视频。面向内容创作者和营销团队，将原本需要多个工具协作完成的视频制作流程压缩为单一输入，是国内 AI 视频生成领域的重要开源项目。
🔗 https://github.com/AIDC-AI/Pixelle-Video

---

10. anthropics/financial-services 🐍 Python
Anthropic 官方开源的金融服务行业 Claude 应用示例库。收录了风险评估、合规文本审查、客户服务对话、财务报告生成等典型金融场景的完整实现，包括 Prompt 设计、工具调用、Agent 流程编排等各层面的最佳实践。对于希望在金融业务中落地 Claude 的开发者和企业，这是最权威、最直接的参考起点。
🔗 https://github.com/anthropics/financial-services

---

11. cocoindex-io/cocoindex 🐍 Python
专为长周期 Agent 设计的增量数据索引引擎。解决的核心问题是：Agent 长时间运行时，数据源（文档、代码库、数据库）会持续变化，每次全量重新索引代价极高。CocoIndex 通过追踪数据变更，只对新增或修改的部分做增量处理，大幅降低索引维护成本。适合构建需要持续感知外部数据变化的 Agent 系统。
🔗 https://github.com/cocoindex-io/cocoindex

---

12. ComposioHQ/awesome-codex-skills 🐍 Python
针对 OpenAI Codex CLI 和 API 的实用技能合集，类似 mattpocock/skills 但专注于 Codex 生态。收录了代码生成、自动化测试、CI/CD 集成、数据处理等场景的 Codex Skills，每个技能都有完整的使用说明和示例。随 Codex CLI 普及，这个仓库成为开发者快速扩展 Codex 能力的重要资源库。
🔗 https://github.com/ComposioHQ/awesome-codex-skills

---

13. LearningCircuit/local-deep-research 🐍 Python
完全本地运行的深度研究 Agent，核心卖点是隐私安全与高准确率的结合。支持 Ollama、llama.cpp、Google 等多种 LLM 后端，集成 arXiv、PubMed、私有文档等 10+ 搜索引擎，所有数据在本地加密处理，不经过任何第三方服务器。在 SimpleQA 基准上使用 Qwen3.6-27B（3090 显卡）达到约 95% 准确率，适合对数据隐私敏感的学术研究和企业内部知识检索场景。
🔗 https://github.com/LearningCircuit/local-deep-research

---

14. 1jehuang/jcode 🦀 Rust
AI 编码 Agent 的测试与评测框架（Harness），用 Rust 构建。提供标准化的任务定义格式、隔离的执行沙箱和统一的评分机制，让不同 AI 编码 Agent（Claude Code、Codex、Cursor 等）在相同条件下进行横向对比。适合研究者评测 Agent 编码能力，也可用于企业内部选型时的基准测试。
🔗 https://github.com/1jehuang/jcode

---

15. fspecii/ace-step-ui 🟨 JavaScript
ACE-Step 1.5 AI 音乐生成模型的开源 Web 前端，定位为 Suno 的本地免费替代方案。提供专业级的音乐创作界面，支持风格描述、歌词输入、多轨编辑、音色控制等功能，完全离线运行、无次数限制。对于不想为 Suno 付费、或希望对生成过程有更多控制权的音乐创作者，这是目前最成熟的本地 AI 音乐生成方案。
🔗 https://github.com/fspecii/ace-step-ui

---

📊 数据来源：github.com/trending?since=weekly · 每周五自动推送
