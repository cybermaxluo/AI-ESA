# 第二章：治理、风险与合规

> Chapter 2: GRC — Governance, Risk & Compliance

---

## 章节定位

本章建立企业级治理、风险与合规（GRC）框架，为安全体系提供决策机制、风险管控与合规保障。GRC 框架的核心价值在于：将分散的治理活动整合为统一体系，使风险决策可量化、合规状态可追溯、治理成效可衡量。

**目标读者**：CISO/CRO/安全负责人、合规负责人/DPO/法务、风险管理团队/内审、业务高管/董事会成员

---

## 核心概念

### GRC 三支柱

GRC 体系由治理、风险、合规三个相互关联的支柱构成：

| 支柱                         | 核心定位             | 关键活动                     | 主要产出                       |
| ---------------------------- | -------------------- | ---------------------------- | ------------------------------ |
| **治理（Governance）** | 建立方向与决策机制   | 政策制定、组织设计、监督机制 | GRC 章程、政策体系、治理架构   |
| **风险（Risk）**       | 识别、评估与应对风险 | 风险识别、量化评估、处置决策 | 风险登记册、处置计划、KRI 指标 |
| **合规（Compliance）** | 满足法规与标准要求   | 法规监测、差距分析、审计准备 | 合规报告、认证证书、审计证据   |

三支柱之间存在紧密的依赖关系：治理为风险管理和合规活动提供决策框架与资源保障；风险评估结果影响合规优先级与资源分配；合规要求反向约束治理决策与风险容忍度设定。

### GRC 成熟度模型

GRC 成熟度评估为组织提供能力基准与改进方向：

| 级别              | 名称                   | 特征                                 |
| ----------------- | ---------------------- | ------------------------------------ |
| **Level 1** | 初始级（Ad-hoc）       | 无正式流程，被动响应，依赖个人经验   |
| **Level 2** | 可重复级（Repeatable） | 部分流程文档化，关键活动可重复执行   |
| **Level 3** | 已定义级（Defined）    | 完整流程体系，工具支持，跨部门协作   |
| **Level 4** | 量化管理级（Managed）  | 数据驱动决策，持续优化，自动化程度高 |

成熟度评估的价值在于：识别当前能力短板、确定改进优先级、设定阶段性目标、衡量投资效果。

### 风险量化方法

风险量化是将定性风险判断转化为可比较、可决策的定量数据的过程。本章介绍两种主流方法：

**FAIR 模型（Factor Analysis of Information Risk）**：

```
风险 = 损失事件频率（LEF）× 损失幅度（LM）

LEF = 威胁事件频率（TEF）× 脆弱性（Vulnerability）
LM = 主要损失 + 次要损失
```

**ALE 模型（Annual Loss Expectancy）**：

```
ALE = SLE × ARO
- SLE（Single Loss Expectancy）= 单次损失期望
- ARO（Annual Rate of Occurrence）= 年度发生率
```

两种方法各有适用场景：FAIR 模型适合复杂风险场景的深度分析，ALE 模型适合快速估算与横向比较。

---

## 章节结构

本章共 8 节，覆盖 GRC 体系的完整生命周期：

| 节号 | 主题           | 核心内容                                     |
| ---- | -------------- | -------------------------------------------- |
| 2.1  | GRC 治理框架   | 三支柱模型、成熟度评估、组织架构设计         |
| 2.2  | 风险管理体系   | 风险生命周期、量化方法、第三方风险、新兴风险 |
| 2.3  | 合规管理框架   | 全球合规地图、差距分析、审计与认证           |
| 2.4  | 政策与标准体系 | 四级政策框架、控制措施库、生命周期管理       |
| 2.5  | GRC 平台与工具 | 工具选型、合规自动化、系统集成               |
| 2.6  | 治理例会与报告 | 风险委员会、高管报告、董事会汇报             |
| 2.7  | 实战案例       | 跨国 GRC 平台、ISO 认证、供应链风险、AI 治理 |
| 2.8  | 附录与模板     | 风险登记册、合规清单、政策模板、KPI/KRI 体系 |

---

## 章节文件

- **[2.0 执行摘要](./2.0_executive_summary.md)**：本章核心要点与决策框架
- **[2.1 GRC 治理框架](./2.1_grc_governance_framework.md)**

  - GRC 三支柱与成熟度模型
  - GRC 与业务战略对齐
  - GRC 组织架构设计
- **[2.2 风险管理体系](./2.2_risk_management_system.md)**

  - 风险管理生命周期
  - 风险量化方法（FAIR/ALE）
  - 第三方风险管理（TPRM）
  - 新兴风险（AI/云/跨境数据）
- **[2.3 合规管理框架](./2.3_compliance_framework.md)**

  - 全球合规地图
  - 合规差距分析
  - 审计与认证流程
- **[2.4 政策与标准体系](./2.4_policy_standards.md)**

  - 政策框架设计
  - 控制措施库
  - 政策生命周期管理
- **[2.5 GRC 平台与工具](./2.5_grc_platforms_tools.md)**

  - GRC 工具选型
  - 合规自动化
  - GRC 集成与数据流
- **[2.6 治理例会与报告](./2.6_governance_meetings.md)**

  - 风险委员会
  - 高管风险报告
  - 董事会安全汇报
- **[2.7 实战案例](./2.7_case_studies.md)**

  - 跨国企业 GRC 一体化
  - ISO 27001 认证路径
  - 供应链风险治理
  - AI 治理框架
- **[2.8 附录与模板](./2.8_appendix_templates.md)**

  - 风险登记册模板
  - 合规检查清单
  - 政策模板库
  - GRC KPI/KRI 体系

---

## 与其他章节的关系

### 承接第 1 章

第 1 章建立了企业架构到安全架构的顶层逻辑。第 2 章在此基础上深化战略层的治理机制：

- 战略层：GRC 治理框架提供决策支撑
- 规划层：风险评估影响架构决策
- 落地层：合规要求嵌入 SDL 流程

### 支撑后续章节

本章建立的 GRC 框架为后续章节提供治理基础：

| 后续章节                    | 依赖关系                                                         |
| --------------------------- | ---------------------------------------------------------------- |
| Part 2（技术架构，Ch4-7）   | 架构设计满足合规要求；风险评估指导技术选型；政策标准约束架构决策 |
| Part 3（数据安全，Ch8-10）  | GDPR/PIPL 等隐私法规要求；数据分类分级标准；跨境数据传输合规     |
| Part 4（安全运营，Ch11-13） | 事件响应的合规要求；风险监控与 KRI 指标；审计证据管理            |
| Part 5（AI 安全，Ch14-15）  | AI 治理框架；AI 风险评估；AI 伦理合规                            |
| Part 6（组织卓越，Ch16）    | GRC 团队组织设计；角色能力要求；培训与文化建设                   |

---

## 关键术语

| 术语 | 英文全称                            | 说明                         |
| ---- | ----------------------------------- | ---------------------------- |
| GRC  | Governance, Risk & Compliance       | 治理、风险与合规整体管理体系 |
| ERM  | Enterprise Risk Management          | 企业风险管理体系             |
| FAIR | Factor Analysis of Information Risk | 风险量化分析方法             |
| ALE  | Annual Loss Expectancy              | 年度预期损失                 |
| TPRM | Third-Party Risk Management         | 第三方风险管理               |
| KRI  | Key Risk Indicator                  | 关键风险指标                 |
| KPI  | Key Performance Indicator           | 关键绩效指标                 |
| RCSA | Risk and Control Self-Assessment    | 风险控制自评                 |
| IRM  | Integrated Risk Management          | 集成风险管理                 |

---


## 延伸阅读

### 风险管理框架

- ISO 31000: Risk Management Guidelines
- NIST RMF: Risk Management Framework
- FAIR Institute: Factor Analysis of Information Risk
- COSO ERM: Enterprise Risk Management Framework

### 合规与隐私标准

- GDPR: General Data Protection Regulation
- PIPL: 中国《个人信息保护法》
- ISO/IEC 27001: Information Security Management
- SOC 2: Service Organization Control
- PCI DSS: Payment Card Industry Data Security Standard

---

## 导航

**[← 上一章：第 1 章 企业架构基础](../chapter_01_enterprise_architecture_foundation/)** | **[返回 Part 1](../)** | **[返回总目录](../../)** | **[下一章：第 3 章 业务安全伙伴 →](../chapter_03_business_security_partnership/)**

---

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**
