# 第七章：供应链安全

## 章节定位

供应链安全是现代企业安全体系中复杂度最高的领域之一。本章提供软件、供应商与硬件供应链风险的综合治理框架，整合 NIST SSDF、SLSA、SBOM 等标准的工程实践，并结合典型事件的响应经验。

本章的核心关注点包括：软件成分可见性（SBOM）、构建完整性（SLSA）、第三方风险管理、以及供应链事件检测与响应。

---

## 目标读者

- **安全负责人**：建立供应链安全战略与治理框架
- **安全架构师**：设计供应链保护的技术控制架构
- **应用安全团队**：实施 SBOM、SCA 与安全 CI/CD 流水线
- **第三方风险管理（TPRM）**：供应商安全评估与持续监控
- **合规与 GRC 团队**：满足 EO 14028、NIST SSDF、SLSA 等监管要求

---

## 章节结构

### [执行摘要](7.0_executive_summary.md)

供应链威胁态势、战略框架、核心概念与度量体系概览。

### [7.1 软件供应链安全战略](7.1_software_supply_chain_strategy.md)

- 供应链攻击分类体系
- 成熟度模型（四阶段）
- 组织架构与职责分工
- 框架对齐（NIST SSDF、SLSA）

### [7.2 供应链攻击与防御](7.2_supply_chain_attacks_defense.md)

- 典型攻击案例分析：SolarWinds（构建系统入侵）、Log4Shell（开源组件漏洞）、Codecov（CI/CD 投毒）、NPM/PyPI 供应链攻击
- 攻击向量分析
- 防御策略与对策

### [7.3 开源治理](7.3_open_source_governance.md)

- 软件成分分析（SCA）
- 软件物料清单（SBOM）：SPDX 与 CycloneDX 格式、生成与管理、漏洞追踪
- 开源许可证合规
- 组件选型标准
- 依赖漏洞管理

### [7.4 CI/CD 供应链安全](7.4_cicd_supply_chain_security.md)

- CI/CD 攻击面分析
- 构建系统加固
- 制品签名与验证（Sigstore、Cosign）
- 流水线安全扫描
- 构建环境隔离
- SLSA 等级达成

### [7.5 容器镜像供应链安全](7.5_container_supply_chain_security.md)

- 容器镜像风险
- 基础镜像选型与管理
- 镜像扫描（Trivy、Clair、Snyk）
- 镜像签名（Docker Content Trust、Cosign）
- 私有镜像仓库安全
- 容器 SBOM

### [7.6 供应商与第三方安全管理](7.6_vendor_third_party_security.md)

- 供应商安全评估
- 供应商准入流程
- 第三方 SDK 安全审查
- API 供应商管理
- 持续监控机制
- 供应商事件响应

### [7.7 硬件供应链安全](7.7_hardware_supply_chain_security.md)

- 硬件篡改检测
- 固件安全
- TPM 与 Secure Boot
- 硬件供应商审计

### [7.8 供应链风险检测与响应](7.8_supply_chain_risk_detection.md)

- 供应链威胁情报
- 漏洞预警与通知
- 供应链事件响应流程
- 快速修复与缓解

### [7.9 供应链安全合规](7.9_supply_chain_compliance.md)

- 美国行政命令 14028（SBOM 强制要求）
- NIST SSDF（安全软件开发框架）
- SLSA（软件制品供应链等级）
- ISO/IEC 27036（供应链安全）
- C2PA（内容溯源与真实性）

### [7.10 案例研究](7.10_case_studies.md)

- 案例一：全球企业 SBOM 体系建设
- 案例二：CI/CD 供应链安全加固
- 案例三：容器镜像供应链治理
- 案例四：供应链攻击响应（Log4Shell 事件）

---

## 核心框架与标准

### 国际标准

| 标准 | 范围 |
|------|------|
| NIST SP 800-161 | 网络安全供应链风险管理 |
| NIST SSDF (SP 800-218) | 安全软件开发框架 |
| SLSA | 软件制品供应链等级（Level 1-4） |
| ISO/IEC 27036 | 供应商关系信息安全 |
| CISA C-SCRM | 网络供应链风险管理 |

### SBOM 标准

| 标准 | 特点 |
|------|------|
| SPDX | ISO 标准，适合合规与法务场景 |
| CycloneDX | OWASP 项目，安全聚焦，支持 VEX |
| SWID Tags | ISO/IEC 19770-2，操作系统级资产追踪 |

### 合规要求

| 法规/标准 | 核心要求 |
|-----------|----------|
| 美国 EO 14028 | 联邦采购 SBOM 强制 |
| 欧盟网络弹性法案 | 软件供应链安全义务 |
| 金融行业 | FFIEC、GLBA、SOX 第三方控制 |

---

## 与全书架构的关系

### Part 2 定位

本章属于"技术架构与基础设施安全"部分，与前序章节形成递进关系：

- **第 4 章（安全架构工程）**：架构设计原则在供应链场景的应用
- **第 5 章（云安全架构）**：云供应链与 SaaS 供应商安全
- **第 6 章（应用安全架构）**：SBOM、SCA 与安全 CI/CD 的集成

### 跨章节关联

| 章节 | 关联点 |
|------|--------|
| 第 2 章（GRC） | 供应链风险管理与合规框架 |
| 第 3 章（BISO） | 供应商准入的业务对齐 |
| 第 8 章（数据安全） | 供应商关系中的数据保护 |
| 第 11 章（SOC） | 供应链威胁检测与事件响应 |
| 第 14 章（AI 赋能安全） | AI 驱动的漏洞优先级排序与威胁情报 |

---

## 阅读路径建议

根据角色和时间预算，可选择以下阅读路径：

### 安全负责人（2-3 小时）

优先阅读战略框架与合规要求：执行摘要 → 7.1 战略与成熟度 → 7.9 合规要求 → 7.10 案例研究。

### 安全架构师（6-8 小时）

聚焦技术架构设计：7.1 战略框架 → 7.3-7.5 技术架构（SBOM、CI/CD、容器） → 7.6 供应商管理架构 → 7.8 检测与响应机制。

### 应用安全工程师（8-10 小时）

深入工程实践：7.2 攻击案例 → 7.3 SCA 与 SBOM 实施 → 7.4 CI/CD 安全控制 → 7.5 容器安全实践 → 7.10 实施案例。

### TPRM/GRC 团队（4-6 小时）

关注治理与合规：7.1 治理框架 → 7.6 供应商评估与监控 → 7.8 风险检测与响应 → 7.9 合规映射。

---

## 章节预期收获

完成本章学习后，读者应能够：

- 建立端到端的供应链安全治理框架
- 理解主要供应链攻击模式及其防御策略
- 实施 SBOM 生成、管理与漏洞追踪
- 加固 CI/CD 流水线与容器镜像供应链
- 管理第三方供应商安全风险的全生命周期
- 达成 NIST SSDF、SLSA 及监管 SBOM 要求
- 有效响应供应链安全事件

---

## 文件结构

```
chapter_07_supply_chain_security/
├── README.md                              # 本文件
├── 7.0_executive_summary.md               # 执行摘要
├── 7.1_software_supply_chain_strategy.md  # 战略与治理
├── 7.2_supply_chain_attacks_defense.md    # 攻击案例分析
├── 7.3_open_source_governance.md          # SCA 与 SBOM
├── 7.4_cicd_supply_chain_security.md      # CI/CD 安全
├── 7.5_container_supply_chain_security.md # 容器安全
├── 7.6_vendor_third_party_security.md     # 供应商管理
├── 7.7_hardware_supply_chain_security.md  # 硬件安全
├── 7.8_supply_chain_risk_detection.md     # 检测与响应
├── 7.9_supply_chain_compliance.md         # 合规标准
└── 7.10_case_studies.md                   # 实施案例
```

---

## 参考资源

### 标准与框架

- NIST SP 800-161 Rev. 1: Cybersecurity Supply Chain Risk Management
- NIST SP 800-218: Secure Software Development Framework (SSDF)
- SLSA Framework: https://slsa.dev
- SPDX Specification: https://spdx.dev
- CycloneDX Specification: https://cyclonedx.org

### 工具与平台

| 类别 | 工具 |
|------|------|
| SBOM 生成 | Syft、SPDX tools、CycloneDX generators |
| SCA | Snyk、MurphySecurity（墨菲安全）、Dependabot、Renovate |
| 签名验证 | Sigstore、Cosign、Notary |
| 镜像扫描 | Trivy、Clair、Grype、Anchore |

---

## 导航

**[← 上一章：第 6 章 应用安全架构](../chapter_06_application_security_architecture/)** | **[返回 Part 2](../)** | **[返回总目录](../../)** | **[→ 下一章：第 8 章 数据安全](../../part_03_data_security_privacy/chapter_08_data_security/)**

---

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**

