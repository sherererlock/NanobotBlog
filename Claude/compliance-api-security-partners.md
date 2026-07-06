# Claude now works with more security and compliance tools

> 原文链接：https://claude.com/blog/compliance-api-security-partners
> 总结日期：2026-05-22

---

# Claude 新增28项安全与合规工具集成——深度总结

---

## 核心主题

Anthropic 于2026年5月21日正式宣布，Claude 现已通过全新的 **Claude Compliance API**，与28家主流企业安全与合规工具平台完成深度集成。此举标志着 Claude 在企业级安全治理能力上的重大突破——IT 与安全团队可以像管理其他企业应用一样，对 Claude 实施统一的安全策略与合规监控。

---

## 主要内容

### 1. 核心技术：Claude Compliance API

本次所有集成均由 **Claude Compliance API** 驱动。该 API 为企业安全与合规团队提供了对两类关键数据的程序化访问能力：

- **对话内容访问**：涵盖 Claude Enterprise 中的聊天记录、上传文件及项目内容，使管理团队能够将已有的安全监控、数据丢失防护（DLP）策略无缝延伸至 Claude 的使用场景，无需另起炉灶。

- **活动事件追踪**：覆盖 Claude Enterprise 及 Claude Platform 的全平台活动日志，包括用户登录行为、管理员操作记录以及配置变更事件，帮助安全团队在组织层面建立统一的 Claude 使用视图。

这一设计理念的核心在于"融入现有工作流"——企业无需重新搭建监控体系，只需将 Claude 的数据流接入已有的安全仪表板与告警机制即可。

### 2. 集成覆盖范围：28家顶级安全合规厂商

本次集成涵盖企业安全生态中的多个关键细分领域：

| 安全领域 | 代表性合作伙伴 |
|---|---|
| **DLP（数据丢失防护）** | Forcepoint、Proofpoint、Mimecast |
| **SASE（安全访问服务边缘）** | Zscaler、Netskope、Fortinet |
| **数据安全** | Varonis、Cyera、Rubrik |
| **SIEM 与安全运营** | CrowdStrike、Sumo Logic、ReliaQuest、Trellix |
| **身份管理** | Okta、SailPoint |
| **eDiscovery（电子取证）** | Relativity、Smarsh、Theta Lake |
| **AI 安全态势管理** | Wiz（现属 Google Cloud）、Tenable、Snyk |
| **AI 可观测性与遥测** | Datadog、Cribl、IBM Guardium、Geordie AI |
| **网络安全基础设施** | Cloudflare、Palo Alto Networks、Microsoft Purview |

完整的28家合作伙伴包括：Cloudflare、Cribl、CrowdStrike、Cyera、Datadog、Forcepoint、Fortinet、Geordie AI、IBM Guardium、Microsoft Purview、Mimecast、Netskope、Okta、Palo Alto Networks、Proofpoint、Relativity、ReliaQuest、Rubrik、SailPoint、Smarsh、Snyk、Sumo Logic、Tenable、Theta Lake、Trellix、Varonis、Wiz 及 Zscaler。

### 3. 部署流程：极低的接入门槛

对于已使用上述任意平台的企业客户，启用流程高度简化：**连接并配置 Claude 实例 → 数据自动流入现有仪表板与告警工作流**。无需复杂的二次开发，最大限度降低了企业的迁移与接入成本。

---

## 关键数据与结论

- **集成数量**：一次性上线 **28个** 安全与合规工具集成，覆盖面极为广泛；
- **发布时间**：2026年5月21日，集成**即日起可用**；
- **覆盖层次**：同时支持 **Claude Enterprise**（面向终端用户的对话产品）与 **Claude Platform**（面向开发者的 API 平台），实现全产品线统一治理；
- **数据类型**：兼顾内容层面（对话与文件）与行为层面（操作日志），构建立体化合规视图；
- **合作伙伴生态开放性**：Anthropic 同时向更多安全厂商开放申请入驻通道，预示着合作伙伴网络将持续扩展。

---

## 实际意义

### 对企业 IT 与安全团队

这次更新从根本上解决了企业在引入 AI 工具时面临的**合规治理盲区**问题。过去，员工使用 Claude 进行工作时，安全团队难以将其纳入统一的数据安全监控框架；而现在，Claude 的使用行为可以像 Slack、Microsoft 365 等企业协作工具一样，被DLP策略覆盖、被SIEM系统收录、被eDiscovery工具检索。这对于金融、法律、医疗、政府等强监管行业的企业而言，具有至关重要的合规价值。

### 对 Anthropic 企业战略

此举是 Anthropic 深化企业市场布局的关键一步。通过融入企业现有安全生态，而非要求企业为 AI 工具单独建立监管机制，Claude 大幅降低了大型组织的采购决策阻力。安全与合规往往是企业级 AI 采购的最大障碍，此次集成直接回应了这一核心痛点。

### 对整个 AI 行业

Claude Compliance API 的推出，树立了一个企业级 AI 工具主动融入安全生态的范本——**AI 产品不应成为安全治理的例外，而应成为企业安全体系的有机组成部分**。这一理念对行业具有示范意义，也反映出随着 AI 工具在企业中的深度渗透，"AI 原生合规"正在成为不可回避的产品能力标配。

---

**总结而言**，本次 Claude 与28家安全合规工具的集成，不仅是一次产品层面的功能扩展，更是 Anthropic 将"负责任 AI"理念落地于企业实践的重要体现——让安全可管理、让合规可执行、让 AI 真正融入企业信任体系。
