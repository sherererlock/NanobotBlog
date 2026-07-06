# Claude In Microsoft Foundry

> 原文链接：https://claude.com/blog/claude-in-microsoft-foundry
> 总结日期：2026-07-02

---

# Claude in Microsoft Foundry：深度总结

## 核心主题

Anthropic 正式宣布 Claude 模型在 **Microsoft Foundry（Azure 平台）上全面可用（Generally Available）**，标志着两大科技巨头在企业级 AI 基础设施领域的深度整合迈入新阶段。这一举措旨在为企业用户提供兼具顶级模型能力与企业级安全合规需求的 AI 解决方案。

---

## 主要内容

### 一、产品正式上线

自 2026 年 6 月 29 日起，Claude 模型正式在 Microsoft Foundry 中全面可用，运行于 Azure 云环境之上。此前该功能处于预览阶段（Foundry Preview），此次升级至 GA（正式发布）状态，意味着产品稳定性、支持力度与功能完整性均达到企业生产级别标准。

### 二、可用模型与核心能力

初始阶段提供两款模型：
- **Claude Opus 4.8**：面向复杂推理、高难度任务
- **Claude Haiku 4.5**：面向轻量级、高频次场景

两款模型均通过 **Messages API** 提供服务，支持以下核心能力：
- **Prompt Caching（提示词缓存）**：降低重复调用成本，提升响应效率
- **Extended Thinking（扩展思考）**：增强模型在复杂逻辑推理任务中的表现

应用场景涵盖：代码生成、智能代理（Agentic Work）、复杂推理等企业高价值场景。

### 三、两种部署模式

Anthropic 提供灵活的双轨部署选项，满足不同企业合规与功能需求：

| 部署模式 | 特点 | 适用场景 |
|----------|------|----------|
| **托管于 Azure（Hosted on Azure）** | Azure 原生身份认证、计费、治理，支持美国数据区（US Data Zone） | 有数据驻留合规要求的企业 |
| **托管于 Anthropic（Hosted on Anthropic）** | 完整 API 功能集，更多模型选择 | 需要最新功能或尚未登陆 Azure 模型的开发者 |

Anthropic 明确表示，未来将逐步实现两种部署模式在功能和模型上的**完全对等**。

### 四、企业级集成优势

Claude in Microsoft Foundry 具备以下企业级特性：

- **Azure 原生**：与现有 Azure 身份体系、网络架构、治理控制无缝集成
- **统一账单**：用户收到单一整合发票，符合条件的 Microsoft 企业协议（Enterprise Agreement）客户，Claude 使用量可直接抵扣 Azure 承诺消费额度
- **数据主权**：支持选择推理处理的地理位置，包括专属的**美国数据区**，满足金融、医疗、政府等高度监管行业的数据驻留要求
- **推理运营**：Anthropic 作为数据处理方（Data Processor）负责运营推理服务，确保模型质量与安全标准

---

## 关键数据与用户案例

文章引用了多家企业的真实使用证言，具体呈现了 Claude in Foundry 的实际落地价值：

### NVIDIA
> Justin Boitano（企业计算副总裁兼总经理）指出，Claude 模型在推理、编程和企业能力方面表现突出，适合复杂技术工作中的自主 AI 代理任务。Claude 现运行于搭载 **NVIDIA GB300 GPU** 的 Microsoft Foundry 之上，为大规模生产部署提供性能保障。

### Bolt（企业开发平台）
> Gary Ballabio（合作关系副总裁）强调，Azure 上运行 Claude 提供了**持续的吞吐量与可靠性**，使 Bolt 能够服务于财富 500 强企业，将前沿模型质量与企业级基础设施相结合。

### 核能安全分析领域（核电企业）
> Matt Huang（创始产品负责人）分享了最具冲击力的数据：借助 Claude 与 Azure 的结合，一项原本需要 **200 个人工天**的安全分析任务被压缩至**仅需 1 天**完成，效率提升约 **200 倍**。他特别强调，核能行业对能力与安全性有着极致要求，而 Anthropic + Azure 的组合恰好同时满足两者。

### Momentic（AI 测试平台）
> Jeff An（联合创始人兼 CTO）表示，Momentic 使用自然语言描述测试用例，由 Claude Opus 驱动自动化界面验证。目前在 Azure Foundry 上已实现**每分钟数百万 Token** 的服务规模，满足客户对稳定性的高要求。

---

## 实际意义

### 1. 企业 AI 落地的关键障碍被打通
长期以来，企业采用 AI 的核心顾虑在于**数据安全、合规监管与系统集成成本**。Claude in Microsoft Foundry 通过 Azure 原生集成、数据区选择与统一计费，系统性地解决了这三大障碍，降低了企业的决策门槛。

### 2. 加速高价值垂直行业的 AI 渗透
核能安全分析 200 倍效率提升的案例表明，Claude 已具备在**高度专业化、强监管行业**中发挥实质性价值的能力。这对医疗、金融、法律等传统 AI 渗透较慢的行业具有重要的示范意义。

### 3. 云平台竞争格局的战略意义
Claude 同时在 Microsoft Azure、Amazon Bedrock 和 Google Cloud 上提供服务（结合相关博客提及的"Claude apps gateway for Amazon Bedrock and Google Cloud"），体现了 Anthropic **多云中立**的战略定位，避免单一平台依赖，为企业提供更大的选择灵活性。

### 4. 推动 AI 代理（Agentic AI）进入企业主流
本次发布与 NVIDIA、Bolt、Momentic 等企业的合作，均与**自主 AI 代理**应用场景深度绑定。Claude 在 Foundry 上的规模化部署，标志着 Agentic AI 正从实验阶段走向企业生产主流，具有重要的行业风向标意义。

---

## 总结

Claude in Microsoft Foundry 的全面可用，是 Anthropic 企业化战略的重要里程碑。它不仅仅是一次技术集成发布，更代表着**顶尖 AI 能力与企业级合规基础设施的系统性融合**
