# The Full Claude Desktop Experience On Aws Google Cloud And Microsoft Foundry

> 原文链接：https://claude.com/blog/the-full-claude-desktop-experience-on-aws-google-cloud-and-microsoft-foundry
> 总结日期：2026-06-23

---

# Claude Desktop 全面登陆 AWS、谷歌云与微软 Foundry：企业级 AI 部署新里程碑

## 核心主题

Anthropic 于 2026 年 6 月 22 日宣布，通过 AWS、谷歌云（Google Cloud）和微软 Foundry 使用 Claude Desktop 的企业用户，现可获得**完整的 Claude Desktop 体验**，包括聊天（Chat）、Claude Cowork 和 Claude Code 三大核心功能模块，实现真正意义上的统一企业 AI 工作平台。

---

## 主要内容

### 一、从"部分体验"到"完整体验"的跨越

在此次更新之前，通过上述三大云平台部署 Claude Desktop 的企业客户**仅能访问 Claude Cowork 和 Claude Code**，Chat 功能并不可用。此次升级填补了这一空白，使得单一部署方案即可覆盖组织内所有角色的需求：

- **Chat（对话）**：适用于快速问答和问题思考，面向所有员工。
- **Claude Cowork（协作工作）**：面向需要将繁复任务外包给 AI 的团队。Claude 可跨经审批的数据源进行研究，处理设备上已有的文件，并在任务完成后交付成果，实现"后台处理、前台交付"的工作流。
- **Claude Code（代码助手）**：面向工程师群体，提供无需常驻终端的 Agent 式编程体验。

### 二、企业级部署控制能力

此次更新的另一重点在于为 IT 团队提供了一整套**贴近现有企业 IT 体系**的部署与管控工具：

#### 1. 身份认证与单点登录（SSO）
支持 IAM Identity Center（AWS）、Workforce Identity Federation（Google Cloud）、Microsoft Entra ID 以及 Okta 等主流 OIDC 提供商，员工无需使用额外凭证或在终端设备上留存云密钥，安全合规门槛大幅降低。

#### 2. MDM 策略模板与离线安装
管理员可直接从配置界面导出策略模板，并通过 **Intune、GPO 或 Jamf** 等主流移动设备管理（MDM）工具进行推送，与现有 IT 工作流高度融合。同时提供**离线安装包**，满足气隙（air-gapped）环境的严苛需求。

#### 3. 分阶段权限管控
Chat、Claude Cowork、Claude Code 三个功能模块**各自拥有独立的策略密钥（Policy Key）**，IT 团队可精细化控制：例如先向非技术团队开放 Chat 和 Cowork，再向工程团队开放 Code，随采用率逐步扩大权限范围。所有硬性拒绝规则在每个标签页上均一致生效。

#### 4. 上线前验证机制
提供预发布验证功能，管理员可在正式推出前测试每个数据连接器、确认云服务商支持的 Claude 模型版本，并核验连接状态。内置**模型守护机制（Model Guard）**确保即使设置存在误配置，推理路由仍保持在 Claude 之上，在 GovCloud 环境中同样有效。

#### 5. Microsoft 365 深度集成
新增 **Microsoft 365 连接器**，通过企业自身的 Entra 应用授权，使 Claude 能够访问邮件和文档，支持租户许可名单（Tenant Allowlisting）配置。同时提供 Beta 版对 **GCC High/DoD**（美国政府高安全级云）端点的支持。对于数据驻留要求最为严格的场景，可使用**本地连接器**，数据连接仅在设备与微软服务之间流转，完全不经过第三方。

### 三、数据主权与隐私控制

在数据治理层面，该方案的设计逻辑高度尊重企业主权：
- 推理（Inference）在企业自行配置的云区域内完成；
- 对话历史**存储在本地设备**，而非上传至 Anthropic；
- 企业自主控制数据连接器可访问的端点；
- 企业可决定向 Anthropic 上报的聚合遥测数据范围。

---

## 关键数据与实际案例

文章引用了**韩华解决方案（Hanwha Solutions）分析/AI 团队负责人 Sarang Oh** 的真实部署案例：

> "我们通过现有云环境快速部署了 Claude Desktop——无需单独的供应商合同。我们自己的 LLM 网关让一个团队就能将其部署给全球数百名用户，无需大量基础设施建设。"

这一案例验证了该方案在大规模组织落地方面的可行性与低摩擦性。

---

## 实际意义

### 对企业 IT 的意义
这次更新标志着企业 AI 工具从"点状试用"走向"系统性全员部署"的关键转折。IT 团队无需为 AI 工具单独构建一套管理体系，Claude Desktop 可以像任何标准企业应用一样被纳入现有的身份管理、设备管理和合规体系中。

### 对员工的意义
不同职能角色（从普通员工到工程师）可在**同一个客户端应用**中获取与自身角色匹配的 AI 能力，降低了学习成本，也避免了多工具切换带来的效率损耗。

### 对行业的意义
Anthropic 此举直接回应了企业客户最核心的两类顾虑：**数据安全与合规**（推理不离云、历史不上传）以及**部署复杂度**（无缝融入现有 MDM/SSO 体系）。在政府、金融、医疗等高监管行业，GovCloud 支持和 GCC High/DoD Beta 接入更是具有明确的战略价值。

总体而言，此次更新是 Anthropic 在企业市场深耕的重要信号——Claude 不再只是一款 AI 工具，而是在向**企业级 AI 基础设施**的方向迈进。
