# Chapter 1: Enterprise Architecture Foundation

# 第一章：企业架构基础——安全架构的顶层逻辑

> **Enterprise Architecture Foundation: The Strategic Logic of Security Architecture**

---

## 📚 章节信息

**核心定位**：建立企业架构体系框架，明确"安全服务业务"的顶层逻辑

**预计页数**：30-40 页

**目标读者**：
- Security Leaders（CSO/CISO/VP）
- Security Architects（首席/高级架构师）
- Enterprise Architects（企业架构师）
- Business Leaders（业务负责人）

---

## 🎯 核心理念

### 安全服务业务的顶层逻辑

**安全的核心是服务业务**，因此谈论安全架构需遵循 **"企业架构→业务架构→IT架构→安全架构"** 的递进逻辑，确保安全与业务目标深度对齐。

### 本书的AI视角

本书以 **AI驱动** 的视角重新审视企业安全架构。在传统安全体系基础上，系统展示AI如何在：
- 威胁检测
- 事件响应
- 漏洞分析
- 合规自动化

等关键环节提升能力（详见Ch 14-15 AI专题章节）。

更重要的是，各业务领域章节（Ch 2-13）的实战案例中均包含AI技术的实际应用场景（标注🤖），展现AI如何贯穿治理、开发、运营、业务等全生命周期，从"点状工具"升级为"体系化能力"。

---

## 📖 章节结构

本章共4节，按照从宏观到具体、从理论到实践的递进逻辑展开：

```
第1章 企业架构基础
│
├── 1.1 企业架构三层体系
│   ├── 战略层：明确业务目标与方向
│   ├── 规划层：将战略转化为架构方案
│   ├── 落地层：推动架构方案落地执行
│   └── 安全架构嵌入点
│
├── 1.2 业务架构——战略/规划/落地的一致性
│   ├── 业务价值澄清
│   ├── 业务架构原则
│   ├── 关键活动（规划层、落地层、架构治理）
│   ├── 价值链与安全活动映射
│   └── 产出
│
├── 1.3 IT架构——TOGAF BDAT与Cloud映射
│   ├── IT架构原则
│   ├── TOGAF BDAT四层架构
│   ├── 参考实施模型
│   └── 控制映射示例
│
└── 1.4 安全架构全景——从战略到落地
    ├── 安全治理三域（基础安全、应用安全、数据安全）
    ├── 四层云架构映射（Cloud/IaaS/PaaS/SaaS）
    ├── 三位一体治理模式（管理/技术/运营）
    ├── 零信任基线
    ├── 安全生命周期活动（战略→规划→落地）
    ├── 产出与目标
    └── 与后续章节的关系
```

---

## 🔑 核心知识点

### 企业架构三层体系

| 层级 | 核心定位 | 关键活动与产出 | 安全嵌入点 |
|------|----------|----------------|------------|
| **战略层** | 明确业务目标与方向 | 制定企业战略、业务愿景、核心目标 | 安全战略与业务战略对齐、GRC治理框架、风险偏好 |
| **规划层** | 将战略转化为架构方案 | 设计业务架构、IT架构（应用/数据/基础设施）、明确架构标准 | **安全架构核心层**：基础安全架构、应用安全架构、数据安全架构 |
| **落地层** | 推动架构方案落地执行 | IT系统项目开发、产品交付、运维运营 | SDL、DevSecOps、安全运营 |

### TOGAF BDAT四层架构

| 架构层 | 核心内容 | 安全控制映射 |
|--------|----------|--------------|
| **Business（业务）** | 业务能力图/价值流/服务蓝图 | 业务连续性、业务风控、反作弊 |
| **Data（数据）** | 数据域/主数据/血缘/跨境策略/生命周期 | 数据分级、加密/脱敏、血缘/访问审计、备份与恢复、驻留管理 |
| **Application（应用）** | 应用/微服务/集成/事件与API/可观测 | 认证鉴权、输入校验、SDL、WAF/RASP、API安全 |
| **Technology（技术/基础设施）** | Cloud/IaaS/PaaS/SaaS资源与平台 | CSPM/CIEM、网络分段、密钥管理（KMS/HSM）、日志集中化 |

### 安全治理三域

1. **基础安全（Infra Security）**
   - 身份与访问、网络分段、主机与容器/K8s、终端/EDR、CSPM/CIEM、PAM/堡垒机

2. **应用安全（AppSec）**
   - 认证鉴权、输入校验、日志与可观测、WAF/RASP、API管理、SAST/DAST/IAST、供应链安全

3. **数据安全（DataSec）**
   - 分类分级、加密与密钥管理、脱敏/代币化、访问审计、驻留与跨境、备份恢复/DLP、隐私工程

---

## 💡 学习目标

完成本章学习后，你将能够：

 **理解架构递进逻辑**：掌握"企业架构→业务架构→IT架构→安全架构"的递进关系

 **明确安全业务价值**：能用业务语言阐述安全在资本、市场、用户、技术、合规五个维度的价值

 **掌握TOGAF BDAT模型**：理解业务、数据、应用、技术四层架构及其安全控制映射

 **建立安全架构全景视图**：形成"三域×四层×三位一体"的完整安全架构框架

 **理解安全生命周期**：掌握战略层、规划层、落地层的关键安全活动

---

## 📂 章节文件

- **[1.1 企业架构三层体系](./1.1_enterprise_architecture_three_layers.md)**
  - 战略层、规划层、落地层的职责与协同
  - 安全架构在各层的嵌入点

- **[1.2 业务架构](./1.2_business_architecture.md)**
  - 业务价值澄清（资本、市场、用户、技术、合规）
  - 业务架构原则与关键活动
  - 价值链与安全活动映射

- **[1.3 IT架构](./1.3_it_architecture.md)**
  - TOGAF BDAT四层架构详解
  - 云时代的架构映射（Cloud/IaaS/PaaS/SaaS）
  - 参考实施模型与控制映射

- **[1.4 安全架构全景](./1.4_security_architecture_landscape.md)**
  - 安全治理三域（基础/应用/数据）
  - 四层云架构映射
  - 三位一体治理模式
  - 零信任基线
  - 安全生命周期活动

---

## 🔗 与其他章节的关系

本章建立了企业架构→安全架构的顶层逻辑框架，后续15个章节基于此框架展开：

### Part 1: Foundation & Strategic Governance（基础与战略治理）

- **Chapter 2: GRC治理** → 对应战略层，建立治理、风险与合规框架
- **Chapter 3: 业务安全伙伴** → 战略层的业务对齐机制（BISO模式）

### Part 2: Technical Architecture（技术架构与基础设施安全）

- **Chapter 4: 安全架构与工程** → 规划层核心，安全架构方法论深化
- **Chapter 5: 云安全架构** → 技术层（Technology）的云安全架构详细设计
- **Chapter 6: 应用安全架构** → 应用层（Application）的安全架构与DevSecOps
- **Chapter 7: 供应链安全** → 应用层的供应链治理

### Part 3: Data Security & Privacy（数据安全与隐私保护）

- **Chapter 8: 数据安全** → 数据层（Data）的安全架构详细设计
- **Chapter 9: 隐私合规** → 数据层的隐私治理
- **Chapter 10: 信息保护** → 数据层的信息保护实践

### Part 4: Security Operations（安全运营与防御能力）

- **Chapter 11: 安全运营（SOC）** → 落地层的检测与响应能力
- **Chapter 12: 红队实践** → 落地层的攻防验证
- **Chapter 13: 业务安全** → 业务层（Business）的安全防护

### Part 5: AI-Driven Security Innovation（AI驱动的安全创新）

- **Chapter 14: AI for Cybersecurity** → AI技术赋能各安全域能力提升
- **Chapter 15: Security for AI** → AI系统本身的安全治理

### Part 6: Security Leadership（安全领导力与组织卓越）

- **Chapter 16: 安全领导力与组织卓越** → 支撑整个架构体系的人员、流程与文化

```mermaid
graph TB
    subgraph "第1章：企业架构基础"
    A[企业架构三层体系]
    B[业务架构]
    C[IT架构]
    D[安全架构全景]
    end

    A --> B
    B --> C
    C --> D

    subgraph "Part 1: 战略治理"
    E[Ch2: GRC]
    F[Ch3: BISO]
    end

    subgraph "Part 2: 技术架构"
    G[Ch4: 安全架构与工程]
    H[Ch5: 云安全]
    I[Ch6: 应用安全]
    J[Ch7: 供应链]
    end

    subgraph "Part 3: 数据安全"
    K[Ch8: 数据安全]
    L[Ch9: 隐私合规]
    M[Ch10: 信息保护]
    end

    subgraph "Part 4: 安全运营"
    N[Ch11: SOC]
    O[Ch12: 红队]
    P[Ch13: 业务安全]
    end

    D --> E
    D --> F
    D --> G
    D --> H
    D --> I
    D --> J
    D --> K
    D --> L
    D --> M
    D --> N
    D --> O
    D --> P

    style A fill:#e1f5ff
    style D fill:#ffe6e6
```

---

## 🌟 本章亮点

### 1. 顶层逻辑的系统性

不同于碎片化的安全实践，本章提供从企业架构到安全架构的**完整递进逻辑**，确保读者建立系统化思维。

### 2. 业务价值的量化

明确安全在**资本、市场、用户、技术、合规**五个维度的价值贡献，并提供量化方法（ROI/ROSI、ALE、安全债务等模型）。

### 3. 云时代的架构演进

将经典TOGAF框架与云计算时代的**Cloud/IaaS/PaaS/SaaS**模型相结合，提供符合现代技术栈的架构指导。

### 4. AI驱动的架构视角

贯穿全书的AI视角，展示AI如何从"点状工具"升级为"体系化能力"，贯穿治理、开发、运营、业务全生命周期。

### 5. 实战导向的设计

每个架构层级都提供：
- 关键活动清单
- 控制映射矩阵
- 产出物模板
- 度量指标体系

---

## 🤔 思考题

1. **战略对齐**：你所在企业的安全战略是如何与业务战略对齐的？是否存在脱节现象？

2. **价值量化**：如何向CEO/CFO说明安全投资的ROI？请尝试使用本章的价值澄清框架设计一个汇报方案。

3. **架构嵌入**：在企业架构三层体系中，安全团队应该在哪一层介入最早？为什么？

4. **云时代挑战**：TOGAF的BDAT四层架构在云原生时代是否仍然适用？需要做哪些调整？

5. **零信任vs传统边界**：零信任架构与传统边界防护相比，在企业架构层面有哪些本质区别？

---

## 📚 延伸阅读

### 参考框架

- **SABSA**：Sherwood Applied Business Security Architecture - https://sabsa.org
- **TOGAF**：The Open Group Architecture Framework - https://www.opengroup.org/togaf
- **NIST CSF**：NIST Cybersecurity Framework - https://www.nist.gov/cyberframework
- **ISO/IEC 42010**：Systems and Software Engineering - Architecture Description

### 推荐资源

- 《Enterprise Security Architecture》- Nicholas A. Sherwood
- 《TOGAF 9.2 Specification》- The Open Group
- 《Security Architecture: Design, Deployment & Operations》- Christopher King
- 企业架构设计方法与实践 - https://tonydeng.github.io/EA-practices/

---

## 📌 关键术语

| 术语 | 英文 | 说明 |
|------|------|------|
| 企业架构 | Enterprise Architecture (EA) | 连接业务战略与IT实施的桥梁 |
| TOGAF | The Open Group Architecture Framework | 企业架构设计的通用方法论 |
| BDAT | Business/Data/Application/Technology | TOGAF核心的四层架构模型 |
| SDL | Security Development Lifecycle | 安全开发生命周期 |
| BISO | Business Information Security Officer | 业务安全伙伴/业务信息安全官 |
| CSPM | Cloud Security Posture Management | 云安全态势管理 |
| CIEM | Cloud Infrastructure Entitlement Management | 云基础设施权限管理 |
| ADR | Architecture Decision Record | 架构决策记录 |
| ROSI | Return on Security Investment | 安全投资回报率 |
| ALE | Annual Loss Expectancy | 年度预期损失 |

---

##  学习检查清单

完成本章学习后，请检查你是否能够：

- [ ] 用自己的话解释"企业架构→业务架构→IT架构→安全架构"的递进逻辑
- [ ] 绘制出企业架构三层体系图，并标注安全架构的嵌入点
- [ ] 列举安全在五个维度（资本、市场、用户、技术、合规）的业务价值
- [ ] 说明TOGAF BDAT四层架构的核心内容和安全控制映射
- [ ] 解释安全治理三域（基础安全、应用安全、数据安全）的职责范围
- [ ] 描述"三位一体"治理模式（管理/技术/运营）的协同机制
- [ ] 理解零信任架构的核心原则（永不信任、持续验证、最小权限）
- [ ] 区分战略层、规划层、落地层的关键安全活动

---

**现在开始第一节的学习。**

 [1.1 企业架构三层体系](./1.1_enterprise_architecture_three_layers.md)

---

## 📍 导航 | Navigation

**[← 返回 Part 1](../)** | **[返回章节导航](../../)** | **[→ 下一章： 第2章](../chapter_02_grc_governance_risk_compliance/)**

### 本章节目录

- **[1.1 企业架构三层体系](./1.1_enterprise_architecture_three_layers.md)**
- **[1.2 业务架构](./1.2_business_architecture.md)**
- **[1.3 IT架构](./1.3_it_architecture.md)**
- **[1.4 安全架构全景](./1.4_security_architecture_landscape.md)**

---

© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0
