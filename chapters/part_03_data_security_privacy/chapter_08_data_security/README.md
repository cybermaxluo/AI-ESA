# Chapter 8: 数据安全 (Data Security)

## 数据安全治理

**目标读者**：data security engineers, data governance leaders, security architects, compliance officers

**核心价值**：建立全生命周期数据安全治理体系，保护企业数据资产

---

## 章节概述

本章系统阐述数据安全治理的战略、架构、技术与运营体系，涵盖数据分类分级、生命周期保护、加密密钥管理、访问控制、数据丢失防护（Data Loss Prevention，DLP）、安全监控审计及跨境数据治理等核心主题。结合全球化企业实践，提供可落地的数据安全架构方案与实施路径。

---

## 内容结构

### [8.1 数据安全战略](./8.1_data_security_strategy.md)
- 数据安全治理框架
- 数据安全成熟度模型
- 数据安全目标与原则
- 数据安全组织架构

### [8.2 数据分类与标记](./8.2_data_classification_labeling.md)
- 数据分类标准（Public、Internal、Confidential、Restricted）
- 数据标记技术（标签、水印、指纹）
- 敏感数据发现（sensitive data discovery）
- 数据资产清单（data inventory）

### [8.3 数据生命周期安全](./8.3_data_lifecycle_security.md)
- 数据创建安全
- 数据存储安全（加密、访问控制）
- 数据传输安全（TLS、VPN、加密传输）
- 数据使用安全（最小权限、审计）
- 数据归档与销毁

### [8.4 数据加密体系](./8.4_data_encryption_system.md)
- 静态加密（encryption at rest）
- 传输加密（encryption in transit）
- 使用中加密（encryption in use，同态加密）
- 密钥管理（KMS）
- 加密算法选择（AES、RSA、ECC）

### [8.5 数据访问控制](./8.5_data_access_control.md)
- 基于角色的访问控制（RBAC）
- 基于属性的访问控制（ABAC）
- 数据权限模型
- 特权访问管理（PAM）
- 数据脱敏（data masking）

### [8.6 数据丢失防护（DLP）](./8.6_data_loss_prevention.md)
- DLP 架构与部署模式
- 网络 DLP（network DLP）
- 端点 DLP（endpoint DLP）
- 云 DLP（cloud DLP）
- DLP 策略设计与调优

### [8.7 数据安全监控与审计](./8.7_data_security_monitoring_audit.md)
- 数据访问审计
- 异常行为检测（UEBA）
- 数据外泄检测
- 数据安全事件响应
- 数据取证

### [8.8 跨境数据治理](./8.8_cross_border_data_governance.md)
- 数据本地化（data localization）
- 数据跨境传输机制（SCC、BCR）
- 数据驻留（data residency）
- 多区域数据架构
- 数据主权（data sovereignty）

### [8.9 实战案例](./8.9_case_studies.md)
- 全球电商数据分类体系建设
- 金融行业 DLP 实施案例
- 跨境数据传输合规架构
- 数据加密全生命周期案例

---

## SABSA 四层架构映射

本章按照 SABSA 四层架构框架组织内容，从业务需求到运营服务形成完整闭环：

| SABSA 层级 | 章节 | 核心内容 |
|-----------|------|---------|
| **业务需求层** | 8.1 数据安全战略 | 治理框架、成熟度模型、目标原则、组织架构 |
| **架构逻辑层** | 8.2-8.3 分类 + 生命周期 | 数据分类标准、标记技术、敏感数据发现、生命周期保护设计 |
| **工程技术层** | 8.4-8.6 加密 + 访问 + DLP | 加密体系、KMS、RBAC/ABAC、脱敏、DLP 部署 |
| **运营服务层** | 8.7 监控与审计 | 访问审计、UEBA、外泄检测、事件响应、取证 |

> 关于 SABSA 四层架构框架的详细说明，参见 [1.4.6 SABSA 四层架构框架](../../part_01_foundation_strategic_governance/chapter_01_enterprise_architecture_foundation/1.4_security_architecture_landscape.md#146-sabsa-四层架构框架)

---

## 学习目标

完成本章学习后，读者将能够：

1. 建立企业级数据安全治理框架与组织架构
2. 设计并实施数据分类分级与标记体系
3. 构建覆盖全生命周期的数据保护控制措施
4. 实施数据加密、密钥管理与访问控制方案
5. 部署 DLP 系统并优化防泄漏策略
6. 建立数据安全监控、审计与事件响应机制
7. 应对跨境数据流动的合规与技术挑战
8. 将数据安全与隐私合规、GRC 体系有机融合

---

## 关键术语

| 术语 | 英文 | 说明 |
|------|------|------|
| 数据分类 | data classification | 按敏感度、重要性对数据进行分级管理 |
| 数据脱敏 | data masking | 隐藏或替换敏感数据，保护隐私 |
| 数据丢失防护 | data loss prevention (DLP) | 防止敏感数据未经授权外泄 |
| 密钥管理服务 | key management service (KMS) | 集中管理加密密钥的生命周期 |
| 敏感数据发现 | sensitive data discovery | 自动识别系统中的敏感信息 |
| 数据安全态势管理 | data security posture management (DSPM) | 持续评估数据安全风险状态 |
| 同态加密 | homomorphic encryption | 在加密状态下进行计算 |
| 零信任数据访问 | zero trust data access | 永不信任、持续验证的数据访问模式 |

---

## 与其他章节的关系

- 与 Chapter 1（企业架构基础）：数据安全是安全架构三域之一，需嵌入企业架构体系
- 与 Chapter 2（GRC）：数据安全治理与风险管理、合规要求紧密对齐
- 与 Chapter 3（业务安全伙伴）：数据安全需与业务场景深度结合，通过 BISO 协作落地
- 与 Chapter 5（云安全）：云数据保护是数据安全在云环境的延伸与实践
- 与 Chapter 9（隐私合规）：数据安全与隐私保护协同，共同满足 GDPR、PIPL 等法规
- 与 Chapter 10（信息保护）：信息保护团队负责 DLP 等技术控制的运营实施
- 与 Chapter 14（AI for Cybersecurity）：AI 技术赋能数据分类、异常检测、自动化响应

---

## 导航

**[← 上一章：第 7 章](../../part_02_technical_architecture_infrastructure_security/chapter_07_supply_chain_security/README.md)** | **[返回 Part 目录](../)** | **[下一章：第 9 章 →](../chapter_09_privacy_compliance/)**

---

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**
