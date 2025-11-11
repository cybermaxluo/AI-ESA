# 贡献指南 | Contributing Guide

感谢您对《AI-Driven Enterprise Security: Architecture, Methodology, and Practice》项目的关注！

我们欢迎所有形式的贡献，无论是内容改进、案例补充、错误修正还是新想法。

---

## 🤝 贡献方式

### 1. 📝 提交 Issue

**适用场景**:
- 发现内容错误（技术错误、拼写错误、格式问题）
- 提出改进建议（内容补充、结构优化）
- 讨论新想法（新章节、新案例、新工具）
- 提问和求助

**操作步骤**:
1. 前往 [GitHub Issues](https://github.com/cybermaxluo/ai-powered-enterprise-security/issues)
2. 点击 "New Issue"
3. 选择合适的模板（Bug Report / Feature Request / Question）
4. 填写详细信息并提交

---

### 2. 🔧 提交 Pull Request

**适用场景**:
- 修正内容错误
- 补充实战案例
- 改进架构图或代码示例
- 优化文档结构

**操作步骤**:

#### Step 1: Fork 本仓库
```bash
# 点击 GitHub 页面右上角的 "Fork" 按钮
```text

#### Step 2: Clone 到本地
```bash
git clone https://github.com/YOUR_USERNAME/ai-powered-enterprise-security.git
cd ai-powered-enterprise-security
```text

#### Step 3: 创建分支
```bash
# 创建并切换到新分支
git checkout -b feature/your-feature-name

# 分支命名建议:
# - fix/typo-chapter-5       (修正错误)
# - feat/add-case-study-xxx  (添加案例)
# - docs/improve-readme      (文档改进)
```text

#### Step 4: 进行修改
- 编辑相关文件
- 确保格式一致（参考现有章节）
- 添加必要的链接和引用

#### Step 5: 提交更改
```bash
git add .
git commit -m "feat: 添加云安全案例研究"

# Commit message 建议格式:
# - feat: 新增功能/内容
# - fix: 修复错误
# - docs: 文档改进
# - style: 格式调整
```text

#### Step 6: 推送到 GitHub
```bash
git push origin feature/your-feature-name
```text

#### Step 7: 创建 Pull Request
1. 前往你的 Fork 仓库页面
2. 点击 "Compare & pull request"
3. 填写 PR 描述：
   - 说明修改内容
   - 关联相关 Issue（如 `Closes #123`）
   - 添加截图（如有必要）
4. 提交 PR 并等待审核

---

### 3. 💬 参与讨论

**适用场景**:
- 分享实践经验
- 讨论技术问题
- 提出行业观点
- 与作者和社区交流

**参与方式**:
- [GitHub Discussions](https://github.com/cybermaxluo/ai-powered-enterprise-security/discussions)
- 通过作者邮箱：186616@gmail.com

---

### 4. ⭐ 推广传播

**适用场景**:
- Star 本项目
- 分享给同事和朋友
- 在社交媒体推广
- 在技术博客中引用

---

## 📖 内容贡献规范

### 文档格式要求

1. **Markdown 格式**
   - 使用标准 Markdown 语法
   - 参考现有章节的格式风格
   - 确保标题层级正确（H1, H2, H3...）

2. **中英双语**
   - 关键术语提供中英对照
   - 标题建议中英双语
   - 示例：`# Part 1: Foundation & Strategic Governance | 基础与战略治理`

3. **代码和命令**
   - 使用代码块标注语言
   ````markdown
   ```bash
   kubectl get pods
```text
   ````

4. **图表和架构图**
   - 优先使用 Mermaid 图表
   - 图片放在 `assets/images/` 目录
   - 使用相对路径引用

5. **链接规范**
   - 使用相对路径（如 `../part_01/`）
   - 确保所有链接有效
   - 外部链接使用完整 URL

### 内容质量要求

1. **准确性**
   - 确保技术内容准确无误
   - 引用权威来源（NIST、ISO、OWASP 等）
   - 标注信息来源

2. **实用性**
   - 提供实战案例和最佳实践
   - 避免纯理论堆砌
   - 包含可操作的检查清单或步骤

3. **完整性**
   - 内容逻辑完整
   - 章节结构清晰
   - 包含必要的导航链接

4. **原创性**
   - 确保内容原创或已获得授权
   - 引用他人内容需注明出处
   - 遵守 CC BY-NC-SA 4.0 许可协议

### 案例贡献要求

如果您希望贡献实战案例，请确保：

1. **脱敏处理**
   - 完全脱敏，不包含公司专有信息
   - 不包含商业机密或敏感数据
   - 使用通用化的描述

2. **案例结构**
   ```markdown
   ### 案例：[案例标题]

   **背景**: 简要说明业务场景和挑战

   **解决方案**: 详细描述技术方案和架构设计

   **实施过程**: 关键步骤和里程碑

   **效果评估**: 量化指标和业务价值

   **经验教训**: 关键经验和避坑指南
```bash

3. **案例质量**
   - 真实场景（脱敏后）
   - 包含架构图或流程图
   - 提供量化指标
   - 总结经验教训

---

## 🔍 审核流程

### PR 审核标准

所有 Pull Request 将经过以下审核：

1. **内容审核**
   - ✅ 内容准确性
   - ✅ 技术深度
   - ✅ 实用价值

2. **格式审核**
   - ✅ Markdown 格式正确
   - ✅ 链接有效性
   - ✅ 图表清晰

3. **风格审核**
   - ✅ 与现有内容风格一致
   - ✅ 语言表达清晰
   - ✅ 结构逻辑合理

### 审核时间

- 一般 PR：3-7 个工作日
- 紧急修复：1-2 个工作日
- 大型贡献：7-14 个工作日

### 反馈与修改

- 审核人员可能会提出修改建议
- 请及时响应并进行修改
- 修改后会重新审核

---

## 👥 贡献者权益

### 贡献者名单

所有贡献者将被列入：
- 项目 README.md 的致谢部分
- CONTRIBUTORS.md 文件（如有重大贡献）

### 贡献者认可

- **5+ 次 PR 合并**: 列入 Contributors 名单
- **10+ 次 PR 合并**: 标注为 Active Contributor
- **重大内容贡献**: 可成为联合作者

---

## 📧 联系方式

如有任何问题，请通过以下方式联系：

- **GitHub Issues**: [提交 Issue](https://github.com/cybermaxluo/ai-powered-enterprise-security/issues)
- **GitHub Discussions**: [参与讨论](https://github.com/cybermaxluo/ai-powered-enterprise-security/discussions)
- **Email**: 186616@gmail.com (Max Luo - 主编)

---

## 📜 行为准则

### 基本原则

1. **尊重**: 尊重所有贡献者和社区成员
2. **专业**: 保持专业的沟通方式
3. **开放**: 对不同意见保持开放态度
4. **建设性**: 提供建设性的反馈

### 禁止行为

- ❌ 人身攻击或侮辱性言论
- ❌ 发布与项目无关的内容
- ❌ 抄袭他人内容
- ❌ 发布商业广告或垃圾信息

---

## 🙏 致谢

感谢所有为本项目做出贡献的朋友们！

您的每一次贡献，无论大小，都让这本书变得更好。

共同，构建更安全的数字世界！

---

**© 2025 AI-ESA Project. Licensed under CC BY-NC-SA 4.0**
