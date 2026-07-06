# 🔥 GitHub 本周 Trending Top 15（2026-05-08）

> 数据来源：[github.com/trending?since=weekly](https://github.com/trending?since=weekly) · 每周五自动推送

---

1. TauricResearch/TradingAgents 🐍 Python
模拟真实交易公司运作的多智能体金融框架，将投研流程拆解为基本面分析师、技术分析师、新闻研究员、风险管理员、交易执行员等专职 Agent 分工协作，每个 Agent 独立分析后汇总决策，比单一 LLM 直接给建议更接近机构实战逻辑。适合研究 LLM 在金融领域的落地路径，也是多 Agent 协作架构的优质参考实现。
🔗 https://github.com/TauricResearch/TradingAgents

---

2. mattpocock/skills 🐚 Shell
TypeScript 知名博主 Matt Pocock 直接开源了自己的 `.claude` 目录，里面是他真实在用的生产级 Claude Code Skills，覆盖代码审查、重构建议、文档生成等高频工程场景。不是教程示例，是可直接复用的工作流，随 Claude Code Skills 生态本周集中爆发而成为开发者第一手参考资料。
🔗 https://github.com/mattpocock/skills

---

3. warpdotdev/warp 🦀 Rust
用 Rust 重写的新一代终端，本周正式开源。核心差异不在于界面美化，而是将 AI Agent 能力原生嵌入终端工作流：支持自然语言描述意图后自动生成并执行命令、命令历史语义搜索、Agent 模式下的自主任务执行。定位是"Agentic 开发环境"，面向习惯在终端工作的开发者。
🔗 https://github.com/warpdotdev/warp

---

4. ruvnet/ruflo 🟦 TypeScript
专为 Claude 设计的 Agent 编排平台，核心能力是将多个 Claude Agent 组织成协作群体（Swarm），支持自主工作流调度、任务分发与结果聚合。内置 RAG 集成、自学习群体智能机制，并原生对接 Claude Code 和 Codex，适合需要构建复杂多 Agent 流水线的团队。
🔗 https://github.com/ruvnet/ruflo

---

5. soxoj/maigret 🐍 Python
OSINT 用户名追踪工具，输入一个用户名，自动在 3000+ 个网站上搜索该账号是否存在，并聚合所有公开信息生成完整的数字画像报告。支持 HTML、PDF、JSON 多种输出格式，内置账号关联分析，常用于安全研究、渗透测试前期侦察和个人隐私暴露面自查。
🔗 https://github.com/soxoj/maigret

---

6. virattt/dexter 🟦 TypeScript
面向金融研究场景的自主 Agent，专注"研究"而非"交易"。能自动抓取 SEC 财报、财经新闻、分析师报告等多源数据，通过 LLM 进行交叉分析后输出结构化投研报告，包含关键指标提取、风险点识别、竞争对手对比等模块，适合需要快速完成公司尽调或行业研究的投资从业者。
🔗 https://github.com/virattt/dexter

---

7. openai/symphony 💧 Elixir
OpenAI 开源的编码 Agent 任务编排框架，解决"如何管理大量并发 AI 编码任务"的工程问题。将项目工作拆解为相互隔离的自主实现单元（Run），每个 Run 独立执行互不干扰，团队通过统一界面管理任务状态，而不是盯着 Agent 逐行输出。选用 Elixir 构建，天然具备高并发和容错能力。
🔗 https://github.com/openai/symphony

---

8. docusealco/docuseal 💎 Ruby
DocuSign 的开源自托管替代方案，提供完整的电子文档签署流程：创建 PDF 表单模板、发送签署邀请、收集多方签名、归档审计记录。支持 Web 界面操作和 API 集成，数据完全存储在自己的服务器上，适合对数据主权有要求、不愿依赖第三方 SaaS 的企业和个人。
🔗 https://github.com/docusealco/docuseal

---

9. AIDC-AI/Pixelle-Video 🐍 Python
阿里巴巴 AIDC 团队开源的 AI 短视频全流程自动生成引擎。输入文本描述或参考图片，系统自动完成脚本生成、AI 配音、字幕合成、画面生成与剪辑合成，输出可直接发布的短视频。将原本需要多个工具协作完成的视频制作流程压缩为单一输入，大幅降低内容创作门槛。
🔗 https://github.com/AIDC-AI/Pixelle-Video

---

10. anthropics/financial-services 🐍 Python
Anthropic 官方开源的金融服务行业 Claude 应用示例库，收录风险评估、合规文本审查、客户服务对话、财务报告生成等典型金融场景的完整实现，涵盖 Prompt 设计、工具调用、Agent 流程编排各层面的最佳实践。是金融行业落地 Claude 最权威、最直接的参考起点。
🔗 https://github.com/anthropics/financial-services

---

11. cocoindex-io/cocoindex 🐍 Python
专为长周期 Agent 设计的增量数据索引引擎。解决的核心问题是：Agent 长时间运行时数据源持续变化，每次全量重新索引代价极高。CocoIndex 通过追踪数据变更只对新增或修改部分做增量处理，大幅降低索引维护成本，适合构建需要持续感知外部数据变化的 Agent 系统。
🔗 https://github.com/cocoindex-io/cocoindex

---

12. ComposioHQ/awesome-codex-skills 🐍 Python
针对 OpenAI Codex CLI 和 API 的实用技能合集，收录代码生成、自动化测试、CI/CD 集成、数据处理等场景的完整 Codex Skills，每个技能附有使用说明和示例。随 Codex CLI 普及而走红，是开发者快速上手和扩展 Codex 能力的重要资源库。
🔗 https://github.com/ComposioHQ/awesome-codex-skills

---

13. LearningCircuit/local-deep-research 🐍 Python
完全本地运行的深度研究 Agent，所有数据在本地加密处理，不经过任何第三方服务器。支持 Ollama、llama.cpp、Google 等多种 LLM 后端，集成 arXiv、PubMed、私有文档等 10+ 搜索引擎，在 SimpleQA 基准上使用 Qwen3.6-27B 达到约 95% 准确率，适合对数据隐私敏感的学术研究和企业内部知识检索场景。
🔗 https://github.com/LearningCircuit/local-deep-research

---

14. 1jehuang/jcode 🦀 Rust
AI 编码 Agent 的标准化评测框架（Harness），用 Rust 构建。提供统一的任务定义格式、隔离的执行沙箱和评分机制，让 Claude Code、Codex、Cursor 等不同 Agent 在相同条件下进行横向对比，适合研究者评测 Agent 编码能力，也可用于企业内部选型时的基准测试。
🔗 https://github.com/1jehuang/jcode

---

15. fspecii/ace-step-ui 🟨 JavaScript
ACE-Step 1.5 AI 音乐生成模型的开源 Web 前端，定位为 Suno 的本地免费替代方案。提供专业级的音乐创作界面，支持风格描述、歌词输入、多轨编辑、音色控制等功能，完全离线运行、无次数限制，适合不想付费或希望对生成过程有更多控制权的音乐创作者。
🔗 https://github.com/fspecii/ace-step-ui

---

📊 数据来源：github.com/trending?since=weekly · 每周五自动推送
