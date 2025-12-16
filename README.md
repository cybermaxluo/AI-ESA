# AI-Driven Enterprise Security: Architecture, Methodology, and Practice

# AI驱动的企业安全：架构、方法论与实践

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
[![GitHub last commit](https://img.shields.io/github/last-commit/cybermaxluo/ai-powered-enterprise-security)](https://github.com/cybermaxluo/ai-powered-enterprise-security/commits/main)

## 本书定位

本书是一部系统化的企业安全技术专著，覆盖安全架构设计、方法论框架与工程实践。全书围绕 AISecOps 方法论框架展开，涵盖"AI for Cybersecurity"（用 AI 做安全）与"Security for AI"（保护 AI 安全）两大技术方向。

**导航：** [作者寄语](#作者寄语) | [目录导航](#目录导航) | [术语表](./docs/GLOSSARY.md) | [作者团队](#作者团队) | [如何参与](#如何参与)

---

## 快速开始

- [开始阅读](./chapters/) - 完整书籍内容
- [完整目录](./docs/AI-ESA_TOC.md) - 详细章节目录与阅读路径建议
- [术语表](./docs/GLOSSARY.md) - 专业术语速查（中英对照）
- [关于作者](./docs/AUTHORS.md) - 作者团队介绍

## 作者寄语

> 本书是作者过去十余年在网络安全领域的探索、学习与实践的总结。从传统边界防御到云原生架构，从被动响应到 AI 驱动的主动防护，从单一数据中心到全球混合云部署，这些年的学习和实践让我深刻体会到：安全是一个快速演进的领域，没有绝对的"最佳答案"，只有适合当下场景的"合理方案"。
>
> 在本书的编写过程中，我非常荣幸能与优秀的编写小组一起协作。团队成员们不仅贡献了宝贵的实战内容和专业见解，还在架构设计、案例补充、内容校对、文字优化等方面投入了大量心血。他们的专业视角、实践经验和细致工作让这本书更加完善和实用。作为联合作者，我们共同将这些年的经验和思考凝练成这本开源书籍。
>
> 在此特别感谢 SHEIN 全球网络安全管理中心（GSRM）的优秀同事们。书中很多实践经验和思考都源于与他们的交流学习，是他们的智慧启发和专业探讨让我受益匪浅。特别感谢我的直属上级、SHEIN 首席安全官（Chief Security Officer）Leon Li，他不仅为大家提供了宝贵的成长平台和实践机会，更在 AI 安全的战略布局上给予了前瞻性的指导和坚定的支持，让我们有机会在企业安全最前沿不断探索和创新。SHEIN"客户至上、全力以赴、求真务实、学习创新、多元兼容"的价值观深深影响着我们的工作方式——始终以业务真实需求为导向，保持好奇心和前瞻思维，在全球化的安全实践中持续创新。
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

## 目录导航

本书包含 6 个部分、16 章、150+ 节，覆盖 14 个安全域。

### [Part 1: 基础与战略治理](./chapters/part_01_foundation_strategic_governance/)

- **[Ch 1](./chapters/part_01_foundation_strategic_governance/chapter_01_enterprise_architecture_foundation/)**: 企业架构基础——TOGAF、SABSA 与安全架构嵌入
- **[Ch 2](./chapters/part_01_foundation_strategic_governance/chapter_02_grc_governance_risk_compliance/)**: GRC 治理——风险管理与合规框架
- **[Ch 3](./chapters/part_01_foundation_strategic_governance/chapter_03_business_security_partnership/)**: 业务安全伙伴——BISO 模式与协作机制

### [Part 2: 技术架构与基础设施安全](./chapters/part_02_technical_architecture_infrastructure_security/)

- **[Ch 4](./chapters/part_02_technical_architecture_infrastructure_security/chapter_04_security_architecture_engineering/)**: 安全架构与工程——零信任、威胁建模
- **[Ch 5](./chapters/part_02_technical_architecture_infrastructure_security/chapter_05_cloud_security_architecture/)**: 云安全架构——K8s 安全、CSPM、云 IAM
- **[Ch 6](./chapters/part_02_technical_architecture_infrastructure_security/chapter_06_application_security_architecture/)**: 应用安全架构——SDL、OWASP 防护
- **[Ch 7](./chapters/part_02_technical_architecture_infrastructure_security/chapter_07_supply_chain_security/)**: 供应链安全——SBOM、SCA 工具链

### [Part 3: 数据安全与隐私](./chapters/part_03_data_security_privacy/)

- **[Ch 8](./chapters/part_03_data_security_privacy/chapter_08_data_security/)**: 数据安全——分类分级、加密、访问控制
- **[Ch 9](./chapters/part_03_data_security_privacy/chapter_09_privacy_compliance/)**: 隐私合规——GDPR、PIPL、CCPA
- **[Ch 10](./chapters/part_03_data_security_privacy/chapter_10_information_protection/)**: 信息保护——DLP、泄露响应

### [Part 4: 安全运营与防御能力](./chapters/part_04_security_operations_defense_capabilities/)

- **[Ch 11](./chapters/part_04_security_operations_defense_capabilities/chapter_11_security_operations/)**: 安全运营（SOC）——SIEM/SOAR/威胁狩猎
- **[Ch 12](./chapters/part_04_security_operations_defense_capabilities/chapter_12_red_team/)**: 红队实践——攻防演练、紫队协作
- **[Ch 13](./chapters/part_04_security_operations_defense_capabilities/chapter_13_business_security/)**: 业务安全——反欺诈、风控引擎

### [Part 5: AI 驱动的安全创新](./chapters/part_05_ai_driven_security_innovation/)

本部分系统化构建 AISecOps 方法论框架。

- **[Ch 14](./chapters/part_05_ai_driven_security_innovation/chapter_14_ai_for_security/)**: AI for Cybersecurity——威胁检测、响应编排、漏洞治理、安全左移
- **[Ch 15](./chapters/part_05_ai_driven_security_innovation/chapter_15_security_for_ai/)**: Security for AI——OWASP LLM Top 10、对抗攻击防御、AI 治理合规

延伸阅读：[AISecOps 完整方法论框架](./chapters/part_05_ai_driven_security_innovation/README.md)

### [Part 6: 安全领导力与组织建设](./chapters/part_06_security_leadership_organizational_excellence/)

- **[Ch 16](./chapters/part_06_security_leadership_organizational_excellence/chapter_16_security_leadership/)**: 安全领导力——团队建设、文化塑造、预算管理

---

## 作者团队



| 姓名               | 角色            | 研究方向                                                             | 联系方式                                                                                                                                            |
| ------------------ | --------------- | -------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| 罗棋琛 Max Luo     | 主编 / 联合作者 | 企业安全体系建设<br />应用安全 / DevSecOps<br />AI for Cybersecurity | 📧 186616@gmail.com<br />💻 [GitHub](https://github.com/cybermaxluo)<br />🔗 [LinkedIn](https://linkedin.com/in/max-luo)<br />💬 微信公众号: 白帽子罗棋琛 |
| 潘禺涵 Caleb Pan   | 联合作者        | AI for Cybersecurity<br />机器学习                                   | 📧 now_here@yeah.net<br />💻 [GitHub](https://github.com/dreambb)                                                                                      |
| 吴国斌 Vincent Wu  | 联合作者        | 云原生安全<br />Go 工程实践<br />应用安全架构                        | 📧 wgblike@gmail.com<br />💻 [GitHub](https://github.com/wgblikeW)<br />🔗 [Blog](https://p1nant0m.xyz)                                                   |
| 王丰 Finn Wang     | 联合作者        | AI for Cybersecurity<br />AI 安全项目管理                            | 📧 fwang.sec@gmail.com                                                                                                                              |
| 侯靖 Senull Hou    | 联合作者        | 机器学习<br />AI for Cybersecurity                                   | 📧 papa4workonly@gmail.com                                                                                                                          |
| 王振宇 Shadow Wang | 联合作者        | 大数据安全<br />AI 安全应用研发                                      | 📧 ai.1024.shadow@gmail.com<br />💻 [GitHub](https://github.com/fade-shadow)                                                                           |
| 孙冲 Mori Sun      | 联合作者        | 应用安全 / DevSecOps<br />Web3 Security<br />Red Team                | 📧 moriii22@outlook.com<br />💻[GitHub](https://github.com/WhiteLee03)                                                                                 |
| 黄奕霖 Shiro Huang | 联合作者        | 红队攻防对抗、AI for Cybersecurity                                   | 📧 crystalnuts9@gmail.com<br />[💻 Github](https://github.com/AibaAsaki)                                                                               |
| 陈进 Sayid Chen    | 联合作者        | 移动应用安全、AI 移动应用安全                                        |                                                                                                                                                     |

详细介绍：[docs/AUTHORS.md](./docs/AUTHORS.md)

---

## 如何参与

欢迎通过以下方式贡献：提交 Issue、Pull Request、分享实践经验、Star 本项目。

详细指南：[docs/CONTRIBUTING.md](./docs/CONTRIBUTING.md)

---

## 项目状态

| 指标     | 状态                  |
| -------- | --------------------- |
| 当前版本 | v1.0（Draft）         |
| 内容状态 | 主体完成，持续优化中  |
| 章节覆盖 | 6 Part / 16 Chapter  |

---

## 许可证

本作品采用 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) 许可协议：署名、非商业性使用、相同方式共享。

---

## 致谢

感谢全球开源安全社区、NIST/ISO/OWASP 等标准组织，以及所有提供反馈的读者。

---

## 💝 支持项目

如果这本书对您有帮助，欢迎通过以下方式支持我们：

### 加入微信交流群

<div align="center">
<img src="./assets/qr-wechat-group.jpg" alt="微信交流群二维码" width="200"/>
<p><i>扫码加入微信交流群，与安全专家交流</i></p>
</div>

### 请作者喝一杯咖啡 ☕

您的支持是我们持续创作的动力！

<div align="center">
<img src="./assets/qr-wechat-donate.jpg" alt="微信收款码" width="200"/>
<p><i>请作者喝一杯咖啡</i></p>
</div>

---

## ⭐ Star History

如果这本书对您有帮助，请给我们一个 Star ⭐️

---

<div align="center">

**Made with ❤️ by Security Community | 由全球安全社区共同创作**

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**

</div>
