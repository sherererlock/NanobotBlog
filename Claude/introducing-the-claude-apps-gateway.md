# Introducing The Claude Apps Gateway

> 原文链接：https://claude.com/blog/introducing-the-claude-apps-gateway
> 总结日期：2026-06-30

---

# Claude Apps Gateway 深度总结

## 核心主题

Anthropic 于 2026 年 6 月 29 日正式推出 **Claude Apps Gateway**，这是一个专为 Amazon Bedrock 和 Google Cloud 平台设计的自托管控制平面（Self-hosted Control Plane）。该产品旨在解决企业在大规模部署 Claude Code 时面临的身份认证、权限管理、成本归因和安全合规等核心痛点，标志着 Anthropic 在企业级 AI 基础设施领域迈出了重要一步。

---

## 主要内容

### 一、问题背景：企业部署的现实困境

在 Claude Apps Gateway 推出之前，企业在 Amazon Bedrock 或 Google Cloud 上运行 Claude Code 面临三大典型问题：

1. **凭证管理混乱**：需要为每位开发者单独配置云端凭证，管理成本极高；
2. **策略推送繁琐**：企业设置需要手动推送到每台开发者机器，缺乏集中管控能力；
3. **成本归因缺失**：没有独立工具实现按用户维度的费用追踪，财务透明度不足。

这些问题在团队规模扩大时会成倍放大，成为企业 AI 工具落地的实际障碍。

### 二、解决方案：Gateway 的核心架构

Claude Apps Gateway 以**单一无状态容器**的形式部署在 Linux 环境下，配合 PostgreSQL 数据库运行。其设计哲学是"轻量部署、集中管控"，具体体现在以下五大功能模块：

#### 1. 身份认证（Identity）
Gateway 充当 **OpenID Connect（OIDC）依赖方**，支持对接主流企业身份提供商，包括 Google Workspace、Microsoft Entra ID、Okta 以及任何符合标准的 OIDC 提供商。系统颁发短期会话令牌，**开发者机器上不保存任何长期密钥**，显著降低安全风险。员工入职只需在 IdP 中添加账户，离职则直接移除，操作极为简洁。

#### 2. 策略管理（Policy）
管理员可在服务器端**统一定义托管设置**，客户端在登录时自动接收并应用策略。Gateway 在每次请求时强制执行策略，支持集中调整允许使用的模型范围和默认参数配置，实现真正意义上的"一次配置、全局生效"。

#### 3. 遥测数据（Telemetry）
客户端为每次请求生成使用指标，Gateway 通过 **OTLP 协议**将数据转发至企业自行配置的采集器，数据存储在企业自有网络中，保留周期由企业自主决定，充分保障数据主权。

#### 4. 流量路由（Routing）
Gateway 持有上游凭证，可将推理请求路由至 **Claude API、Amazon Bedrock 或 Google Cloud**，并支持多提供商之间的**故障转移（Failover）**，提升服务可用性和灵活性。

#### 5. 消费上限（Spend Caps）
支持按**组织、群组或用户**三个维度设置每日、每周、每月的消费限额，从制度层面管控 AI 工具的使用成本，避免预算超支。

### 三、技术集成方式

Gateway 直接内置于开发者已安装的 `claude` 二进制文件中，由 Anthropic 统一构建和发布。这意味着：

- `/login` 流程天然感知 Gateway 存在；
- 客户端在登录时自动应用托管设置；
- 策略在每次请求中得到一致性执行。

部署流程分三步：下载 CLI 二进制文件并配置 `gateway.yaml`；在客户端机器的 `managed-settings.json` 中设置 `forceLoginMethod` 和 `forceLoginGatewayUrl` 参数；客户端首次启动时自动连接 Gateway。

### 四、隐私与开放性承诺

Anthropic 明确声明：**除非企业主动配置使用 Claude API，否则 Gateway 不会将推理流量或使用数据发送给 Anthropic**，真正实现数据的私有化闭环。此外，Anthropic 将公开 Gateway 使用的协议规范，允许第三方开发者实现相同功能，体现出一定的生态开放姿态。

---

## 关键数据与结论

| 维度 | 关键信息 |
|------|----------|
| 发布时间 | 2026 年 6 月 29 日 |
| 部署形态 | 单一无状态容器 + PostgreSQL |
| 支持平台 | Amazon Bedrock、Google Cloud、Claude API |
| 支持 IdP | Google Workspace、Microsoft Entra ID、Okta 及标准 OIDC |
| 数据传输协议 | OTLP（OpenTelemetry Protocol） |
| 数据隐私承诺 | 默认不向 Anthropic 传输推理流量或使用数据 |
| 产品状态 | 正式可用（Generally Available） |

---

## 实际意义

**对于企业 IT 与安全团队而言**，Claude Apps Gateway 填补了企业级 AI 工具在身份治理、访问控制和合规审计方面的关键空白。它将 AI 工具的管理范式从"个人自治"转变为"集中管控"，与企业现有的 IAM 体系无缝衔接，大幅降低安全合规风险。

**对于工程团队负责人而言**，消费上限功能和按用户维度的遥测数据，使 AI 工具的 ROI 核算成为可能，为资源分配和预算管理提供了数据支撑。

**对于 Anthropic 的战略布局而言**，此举代表 Anthropic 正在从"模型提供商"向"企业 AI 基础设施服务商"延伸，通过深度嵌入企业 IT 生态来加固客户粘性，同时以开放协议的方式吸引更广泛的生态合作伙伴。

**总体而言**，Claude Apps Gateway 是一个务实、架构清晰的企业级产品，它以最小化的部署复杂度解决了企业 AI 工具规模化落地中最棘手的治理问题，是 Anthropic 企业产品线走向成熟的重要标志。
