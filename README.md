# AISecOps: AI-Driven Enterprise Security

# AISecOps：AI 驱动的安全体系

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![GitHub last commit](https://img.shields.io/github/last-commit/cybermaxluo/AISecOps)](https://github.com/cybermaxluo/AISecOps/commits/main)

---

## 本书定位

《AISecOps：AI 驱动的安全体系》是一部系统化的企业安全技术专著，覆盖安全架构设计、方法论框架与工程实践。全书围绕 AISecOps 方法论框架展开，涵盖"AI for Cybersecurity"（用 AI 做安全）与"Security for AI"（保护 AI 安全）两大技术方向。

导航：**[目录导航](#目录导航)** | [快速开始](#快速开始) | [术语表](./docs/GLOSSARY.md) | [作者寄语](#作者寄语) | [如何参与](#如何参与)

---

## 快速开始

- **[前言](./docs/前言.md)** - 这本书想解决什么问题、写给谁、怎么读、以及它的局限
- [开始阅读](./chapters/) - 完整书籍内容
- [完整目录](./docs/AISecOps_TOC.md) - 详细章节目录与阅读路径建议
- **[附录 B：安全框架与标准映射](./docs/附录B_安全框架与标准映射.md)** - 本书章节 ↔ NIST CSF 2.0 / ISO 27001:2022 Annex A / CIS Controls v8.1 三向对照，**含诚实的覆盖缺口清单**
- [术语表](./docs/GLOSSARY.md) - 专业术语速查（中英对照）
- [关于作者](./docs/AUTHORS.md) - 作者团队介绍

---

## 目录导航

本书包含 7 个部分、19 章、190+ 节。覆盖范围与边界见下方「本书的范围边界」，与 NIST CSF 2.0 / ISO 27001 Annex A / CIS Controls v8.1 的三向对照见[附录 B](./docs/附录B_安全框架与标准映射.md)。

### [第1部分 基础与战略治理](./chapters/第01部分_基础与战略治理/)

- [第1章](./chapters/第01部分_基础与战略治理/第01章_企业架构基础/)：企业架构基础——TOGAF、SABSA 与安全架构嵌入
- [第2章](./chapters/第01部分_基础与战略治理/第02章_GRC治理/)：GRC 治理——风险管理与合规框架
- [第3章](./chapters/第01部分_基础与战略治理/第03章_业务安全伙伴/)：业务安全伙伴——BISO 模式与协作机制

### [第2部分 技术架构与基础设施安全](./chapters/第02部分_技术架构与基础设施安全/)

- [第4章](./chapters/第02部分_技术架构与基础设施安全/第04章_安全架构与工程/)：安全架构与工程——零信任、威胁建模
- [第5章](./chapters/第02部分_技术架构与基础设施安全/第05章_云安全架构/)：云安全架构——Kubernetes 安全、CSPM、云 IAM
- [第6章](./chapters/第02部分_技术架构与基础设施安全/第06章_应用安全架构/)：应用安全架构——SDL、OWASP 防护
- [第7章](./chapters/第02部分_技术架构与基础设施安全/第07章_供应链安全/)：供应链安全——SBOM、SCA 工具链

### [第3部分 数据安全与隐私](./chapters/第03部分_数据安全与隐私/)

- [第8章](./chapters/第03部分_数据安全与隐私/第08章_数据安全/)：数据安全——分类分级、加密、访问控制
- [第9章](./chapters/第03部分_数据安全与隐私/第09章_隐私合规/)：隐私合规——GDPR、PIPL、CCPA
- [第10章](./chapters/第03部分_数据安全与隐私/第10章_信息保护与内部风险/)：信息保护与内部风险——文档标签、IRM、DLP、内部威胁

### [第4部分 安全运营与防御能力](./chapters/第04部分_安全运营与防御能力/)

- [第11章](./chapters/第04部分_安全运营与防御能力/第11章_安全运营/)：安全运营（SOC）——SIEM / SOAR / 威胁狩猎
- [第12章](./chapters/第04部分_安全运营与防御能力/第12章_红队实践/)：红队实践——攻防演练、紫队协作
- [第13章](./chapters/第04部分_安全运营与防御能力/第13章_业务风控与反欺诈/)：业务风控与反欺诈——账号、交易、内容、营销四线对抗


### [第5部分 身份、网络与业务连续性](./chapters/第05部分_身份网络与业务连续性/)

企业安全里预算最大、事故最密集的三个域。

- [第14章](./chapters/第05部分_身份网络与业务连续性/第14章_企业身份与访问管理/)：企业身份与访问管理——JML 入转离、抗钓鱼 MFA、访问审阅、PAM、AD 分层加固、非人类身份
- [第15章](./chapters/第05部分_身份网络与业务连续性/第15章_网络基础设施与终端安全/)：网络、基础设施与终端安全——网络分段、DMARC 落地、EDR 策略、出网治理、资产与暴露面
- [第16章](./chapters/第05部分_身份网络与业务连续性/第16章_业务连续性与灾难恢复/)：业务连续性与灾难恢复——BIA、不可变备份、勒索软件端到端处置、危机指挥、演练与度量

> 本地基础设施为主的读者，建议把这一部提到第2部分之前读——第14章的企业身份体系是 5.2 云 IAM 的本体。[详见第5部分 README](./chapters/第05部分_身份网络与业务连续性/README.md)。
### [第6部分 AI 驱动的安全创新](./chapters/第06部分_AI驱动的安全创新/)

本部分系统化构建 AISecOps 方法论框架。

- [第17章](./chapters/第06部分_AI驱动的安全创新/第17章_AI驱动网络安全/)：AI 驱动网络安全——Agentic 安全智能体、AI 安全运营、AISecOps 落地方法论
- [第18章](./chapters/第06部分_AI驱动的安全创新/第18章_AI系统安全/)：AI 系统安全——OWASP LLM Top 10 2025、对抗攻击防御、AI 安全架构、AI 治理合规

延伸阅读：[AISecOps 完整方法论框架](./chapters/第06部分_AI驱动的安全创新/README.md)

### [第7部分 安全领导力与组织建设](./chapters/第07部分_安全领导力与组织建设/)

- [第19章](./chapters/第07部分_安全领导力与组织建设/第19章_安全领导力/)：安全领导力——团队建设、文化塑造、预算管理

---

## 作者寄语

> 本书是作者过去十余年在网络安全领域的探索、学习与实践的总结。从传统边界防御到云原生架构，从被动响应到 AI 驱动的主动防护，从单一数据中心到全球混合云部署，这些年的学习和实践让我深刻体会到：安全是一个快速演进的领域，没有绝对的"最佳答案"，只有适合当下场景的"合理方案"。
>
> 在本书的编写过程中，我非常荣幸能与优秀的编写小组一起协作。团队成员们不仅贡献了宝贵的实战内容和专业见解，还在架构设计、案例补充、内容校对、文字优化等方面投入了大量心血。他们的专业视角、实践经验和细致工作让这本书更加完善和实用。作为联合作者，我们共同将这些年的经验和思考凝练成这本开源书籍。
>
> 在此特别感谢 SHEIN 全球网络安全管理中心（GSRM）的优秀同事们。书中很多实践经验和思考都源于与他们的交流学习，是他们的智慧启发和专业探讨让我受益匪浅。特别感谢我的直属上级、SHEIN 首席安全官（Chief Security Officer）Leon Li，他不仅为大家提供了宝贵的成长平台和实践机会，更在 AI 安全的战略布局上给予了前瞻性的指导和坚定的支持，让我们有机会在企业安全最前沿不断探索和创新。SHEIN "客户至上、全力以赴、求真务实、学习创新、多元兼容" 的价值观深深影响着我们的工作方式——始终以业务真实需求为导向，保持好奇心和前瞻思维，在全球化的安全实践中持续创新。
>
> 我想感谢的人还有很多，特别是那些在挑战中给予我帮助的全球合作伙伴们——Charlotte Xu、Joseph Zhou、Jenny Xie、Danny Chi、Andrew Black、Leo Shum、Veronique Lu、Canon Xu、Walker Fang、Grace Yin、James Lu、Lili Guo、Elijah Pacis 等。坦白讲，我从未想过会有机会加入这样一个全球化的团队。在与他们的合作中，我收获的不仅是专业知识、思辨逻辑、以及全球化的视野，甚至是跨文化的生活哲学。这段经历，是我职业生涯中最宝贵的财富之一。感谢你们。
>
> 开源这本书的初衷，是希望将我们的学习和思考回馈给行业和社区。如果这本书能为正在从事或准备从事企业网络安全工作的朋友提供一些参考价值，那将是我们最大的荣幸。
>
> 知识因分享而增值，智慧因交流而升华。我们期待你的反馈、质疑和共创——欢迎通过 GitHub Issues 与我们交流，也期待你成为下一位贡献者。共同，构建更安全的数字世界。
>
> ——罗棋琛（Max Luo）
>
> 2025 年 11 月 11 日

---

## 本书的范围边界

一本讲"企业安全体系"的书如果不声明边界，读者会默认它什么都覆盖，然后在最需要的地方扑空。以下是本书**明确不覆盖**的领域，以及应当转向的权威资源：

| 不覆盖 | 原因 | 建议转向 |
| --- | --- | --- |
| OT / ICS / SCADA 工业控制系统安全 | 工艺安全、确定性实时约束、停机代价模型与 IT 安全是两套方法论，混写会两边都不到位 | IEC 62443 系列、NIST SP 800-82 Rev.3、ISA-99 |
| IoT 与嵌入式设备安全 | 同上，且硬件信任根、固件签名、低功耗约束需要独立篇幅 | ETSI EN 303 645、NIST IR 8259 系列、OWASP IoT Top 10 |
| 车联网与自动驾驶安全 | 功能安全（ISO 26262）与信息安全的耦合是独立学科 | ISO/SAE 21434、UN R155/R156 |
| 医疗设备安全 | 受 FDA/NMPA 独立监管框架约束 | FDA 上市前网络安全指南、IEC 81001-5-1 |
| 密码算法的数学原理与密码分析 | 本书讲密码学的**工程使用**（选型、密钥管理、迁移），不讲算法设计与破解 | 《Serious Cryptography》、NIST SP 800-57 系列 |
| 具体产品的部署手册 | 产品迭代快于图书生命周期；本书给的是选型判据与架构模式 | 各厂商官方文档 |

本书覆盖的是**以 IT 为主体、云为重心的企业安全体系**——如果你的组织有大量工业现场、车队或医疗终端，本书的治理、运营、数据与 AI 部分仍然适用，但技术控制部分需要按上表补充专门资料。

一条相关提示：书中偶尔以制造业、工业数据为例说明数据分类或预算分配（如 8.2、19.7），那是**举例**，不构成对 OT 安全的覆盖。

---

## 内容基准与版本声明

**内容截止日：2026 年 7 月。** 本书涉及的法规、标准与产品形态均以该时点的公开信息为准。安全领域演进快，引用前请核对当期版本。截至基准日，全书引用的主要标准版本如下：

| 标准 / 框架 | 本书采用版本 | 备注 |
| --- | --- | --- |
| NIST CSF | 2.0 | 现行 |
| NIST SP 800-53 | Rev.5（含 Release 5.2.0 更新） | 现行 |
| NIST SP 800-207 / 800-218 (SSDF) | 现行版 | — |
| ISO/IEC 27001 / 27002 | 2022 | 注意 2013 版的 A.5–A.18 分组编号已废止 |
| ISO/IEC 27701 | 2025 | 已由 27001 扩展标准改为独立可认证标准 |
| ISO/IEC 42001 | 2023 | **不是** EU AI Act 协调标准，不产生推定合规效力 |
| PCI DSS | v4.0.1 | v4.0 已于 2024-12-31 退役；51 项未来日期要求自 2025-03-31 起强制 |
| OWASP Top 10 | 2025 | A03 为软件供应链失效；SSRF 已不单列 |
| OWASP Top 10 for LLM Applications | 2025 | 与 2023 版的编号对照见 18.3 |
| OWASP Top 10 for Agentic Applications | 2026（ASI01–ASI10） | 见 18.3 末节 |
| OWASP ASVS / MASVS | ASVS 5.0.0 / MASVS 2.1.0 | MASVS 自 v2.0 起已取消 L1/L2 分级 |
| MITRE ATT&CK | v19 | — |
| CIS Controls | v8.1 | — |
| CSA CCM / CAIQ | v4.1 | 207 控制 / 17 域；v4.0.x 于 2028-01-31 退役 |
| SLSA | v1.1 | v1.0 已被取代 |

> 时效提示：EU CRA 的漏洞与严重事件报告义务自 2026-09-11 起适用、主要义务自 2027-12-11 起适用。
>
> **EU AI Act 的时间表在 2026 年 7 月被改写**：Regulation (EU) 2026/1744（Digital Omnibus on AI，2026-07-08 通过、2026-07-27 生效）修订了 Regulation (EU) 2024/1689，把独立的 Annex III 高风险义务从 2026-08-02 推迟到 **2027-12-02**，把嵌入受管制产品的 Annex I 高风险义务从 2027-08-02 推迟到 **2028-08-02**；同时把"为偏见检测与纠正而处理特殊类别个人数据"的法律依据从高风险系统提供者扩展到全部 AI 系统与通用目的 AI 模型，附严格必要性标准。GPAI 义务自 2025-08-02 已适用，**执法权自 2026-08-02 起**由 AI Office 与成员国机关行使。
>
> 需要注意一处常见误读：AI Act 义务的推迟**不顺延 GDPR 第 35 条的 DPIA 义务**——只要处理涉及个人数据的高风险场景，DPIA 该做还得做，与 AI Act 的时间表无关。相关内容见 9.0 与 18.6。
>
> 美国 EO 14028 的 SBOM/SSDF 强制机制已由 OMB 于 **2026-01-23** 发布的 M-26-05 撤销（该备忘录撤销 M-22-18 与 M-23-16，SSDF 自证的通用表格改为可选、SBOM 改为各机构按风险自行裁量），技术规格仍为事实标准，相关内容见 6.0 与 7.9。需要一并纠正的口径：**SLSA 是自证框架，没有第三方认证机制**，M-26-05 全文未提及 SLSA；截至基准日未查到把某一 SLSA 等级写成硬性准入条件的公开采购文件。

---

## 内容来源与第三方权利声明

**商标**：本书涉及的产品名称、服务名称、公司名称及标识，均为其各自所有者的商标或注册商标。使用这些名称仅为编辑说明与技术讨论之目的，不构成对相关商标权的主张，亦不表示相关权利人对本书内容的认可或背书。

**第三方框架**：书中对 TOGAF®、ArchiMate®（The Open Group）、SABSA®（SABSA Institute）、Zachman Framework（Zachman International）、COBIT®（ISACA）、ITIL®（PeopleCert）、Cyber Kill Chain®（Lockheed Martin）、FAIR（The Open Group Risk Taxonomy / FAIR Institute）、BSIMM™、CSA CCM（Cloud Security Alliance）、AWS 责任共担模型（Amazon）等框架的图示，均为作者依据公开资料重新绘制的示意图，用于说明与教学，非原图复制；原框架的著作权与商标权归各权利人所有。凡本书对原框架做了裁剪或改编（例如将 SABSA 六层裁剪合并为四层用于组织本书章节），均在正文就地标注，**不代表原框架的官方形态**。

**MITRE**：© The MITRE Corporation. 本书对 MITRE ATT&CK®、ATLAS™、D3FEND™ 的战术、技术与编号的引用，遵循 MITRE 的使用条款。ATT&CK® 为 The MITRE Corporation 的注册商标。

**OWASP**：本书对 OWASP Top 10、OWASP Top 10 for LLM Applications、OWASP Top 10 for Agentic Applications、OWASP SAMM、ASVS、MASVS 的风险分类体系的引用，遵循 OWASP Foundation 的 CC BY-SA 4.0 许可并注明来源。**该部分内容适用 CC BY-SA 4.0，不适用本书整体的 CC BY-NC-SA 4.0**——CC BY-SA 不允许下游附加 NC 等额外限制，相关小节（尤其 18.3、6.1、6.2）已就地单独声明。

**开源规则与工具**：书中的 Falco 规则参考 [The Falco Project](https://falco.org/) 默认规则集（Apache License 2.0）改写；Sigma 规则遵循 [Detection Rule License (DRL)](https://github.com/SigmaHQ/sigma/blob/master/LICENSE.Detection.Rules.md)；Atomic Red Team 命令引自 [Red Canary Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)（MIT License）；OPA/Rego 与 Kyverno 策略参考各自官方 policy library（Apache License 2.0）。上述内容的著作权归各项目所有，本书按其许可使用并注明来源。

**插图**：本书全部插图由作者团队使用 draw.io 原创绘制，drawio 源文件随本仓库开源（见 `assets/diagrams/`），无外部截图。

---

## 作者团队

| 姓名               | 角色            | 研究方向                                                                | 联系方式                                                                                                                                               |
| ------------------ | --------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 罗棋琛 Max Luo     | 主编 / 联合作者 | 企业安全体系建设<br />应用安全<br />DevSecOps<br />AI for Cybersecurity | 📧 186616@gmail.com<br />💻[GitHub](https://github.com/cybermaxluo) <br /> 🔗 [LinkedIn](https://linkedin.com/in/max-luo) <br /> 💬 微信公众号：白帽子罗棋琛 |
| 潘禺涵 Caleb Pan   | 联合作者        | AI for Cybersecurity<br /> 机器学习                                     | 📧 now_here@yeah.net<br /> 💻[GitHub](https://github.com/dreambb)                                                                                         |
| 孙冲 Mori Sun      | 联合作者        | 应用安全<br />DevSecOps <br />  Web3 security <br /> red team           | 📧 moriii22@outlook.com<br /> 💻[GitHub](https://github.com/WhiteLee03)                                                                                   |
| 黄奕霖 Shiro Huang | 联合作者        | 红队攻防对抗<br />AI for Cybersecurity                                  | 📧 crystalnuts9@gmail.com<br />  💻[GitHub](https://github.com/AibaAsaki)                                                                                 |
| 陈进 Sayid Chen    | 联合作者        | 移动应用安全<br />AI 移动应用安全                                       | 📧 1052756668@qq.com<br /> 💻[GitHub](https://github.com/DSFLY100)<br /> 💬 微信公众号：从黑客到保安                                                       |

详细介绍：[docs/AUTHORS.md](./docs/AUTHORS.md)

---

## 如何参与

欢迎通过以下方式贡献：提交 Issue、Pull Request、分享实践经验、Star 本项目。

详细指南：[docs/CONTRIBUTING.md](./docs/CONTRIBUTING.md)

---

## 项目状态

| 指标     | 状态                 |
| -------- | -------------------- |
| 当前版本 | v1.0（Draft）        |
| 内容状态 | 主体完成，持续优化中 |
| 章节覆盖 | 7 Part / 19 Chapter  |

---

## 许可证

本作品采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可协议：署名、非商业性使用、相同方式共享。

---

## 致谢

感谢全球开源安全社区、NIST / ISO / OWASP 等标准组织，以及所有提供反馈的读者。

---

## 💝 支持项目

如果这本书对您有帮助，欢迎通过以下方式支持我们：

### 交流与支持

<div align="center">

<table>
<tr>
<td align="center" width="50%">
<img src="./assets/qr-wechat-group.jpg" alt="微信交流群二维码" width="200"/><br/>
<b>加入微信交流群</b><br/>
<i>扫码加入，与安全从业者交流</i>
</td>
<td align="center" width="50%">
<img src="./assets/qr-wechat-donate.jpg" alt="微信收款码" width="200"/><br/>
<b>请作者喝一杯咖啡 ☕</b><br/>
<i>您的支持是持续创作的动力</i>
</td>
</tr>
</table>

</div>

---

## ⭐ Star History

如果这本书对您有帮助，请给我们一个 Star ⭐

---

<div align="center">

**Made with ❤️ by Security Community | 由全球安全社区共同创作**

**© 2025-2026 AISecOps Project. Licensed under CC BY-NC-SA 4.0**

</div>
