# V6架构图设计规范 - 可复用Prompt

## 设计理念

**核心原则**: 极简主义 + 信息层次 + 扁平化2.0

**设计哲学**: "少即是多,空白即是力量" - 通过减法设计,让信息自己说话

---

## 通用设计规范

### 1. 画布设置

```yaml
尺寸: 1920 x 1080 px
背景色: #FAFBFC
网格系统: 8px基准网格
```

### 2. 配色系统

```yaml
主色: #0066FF (纯蓝)
边框色: #E0E7FF (淡蓝)
背景色: #FFFFFF (纯白)
文字色-标题: #1A1A1A (近黑)
文字色-副标: #6B7280 (中灰)
文字色-描述: #9CA3AF (浅灰)
强调色: #EF4444 (红色,仅用于返回箭头)
```

### 3. 卡片规范

```yaml
圆角: 16px
边框: 2px solid #E0E7FF
背景: #FFFFFF
阴影: 0 2px 8px rgba(0,102,255,0.08)
内边距: 30px
```

### 4. 字体规范

```yaml
字体族: Inter (首选) / SF Pro / Roboto
标题: 36px Semibold #1A1A1A
副标题: 16px Regular #6B7280
描述: 14px Regular #9CA3AF (最多2行)
图标字母: 64px Semibold #0066FF
```

### 5. 箭头规范

```yaml
宽度: 4-5px
颜色: #0066FF
样式: blockThin (直线箭头)
箭头头部: 10-12px
```

### 6. 元素间距

```yaml
卡片间距: 80px (水平/垂直)
内容间距: 20px (文字行距)
边距: 80px (页面边距)
```

---

## TOGAF架构图设计规范

### 布局结构: 3×3矩阵式

```
┌─────────────────────────────────────────────────────────┐
│  标题: TOGAF 架构开发方法 (ADM)                          │
│  副标题: Architecture Development Method                 │
│                                                          │
│  行1: P ──→ A ──→ B                                     │
│       ↓                ↓                                 │
│  行2: H     REQ     C                                    │
│       ↓            ↓                                     │
│  行3: G ←── F ←── E ←── D                               │
└─────────────────────────────────────────────────────────┘
```

### 卡片尺寸

```yaml
普通阶段卡片: 340 x 200 px
中心REQ卡片: 340 x 200 px (相同尺寸)
```

### 中心卡片特殊样式

```yaml
背景色: #0066FF (纯蓝背景)
边框色: #0066FF
文字颜色: #FFFFFF (白色)
图标字母: 64px Bold #FFFFFF
```

### 卡片内容结构

```
┌────────────────────┐
│ P        (字母图标) │  64px Semibold #0066FF
│                    │
│ 预备阶段 (中文标题) │  36px Semibold #1A1A1A
│ Preliminary (英文) │  16px Regular #6B7280
│                    │
└────────────────────┘
```

### 位置矩阵

```yaml
行1 (Y=250):
  - P:  X=160
  - A:  X=580
  - B:  X=1000

行2 (Y=530):
  - H:  X=160
  - REQ: X=580 (中心)
  - C:  X=1000

行3 (Y=810):
  - G:  X=160
  - F:  X=580
  - E:  X=1000
  - D:  X=1420

水平间距: 420px (中心到中心)
垂直间距: 280px (中心到中心)
```

### 箭头流程

```
P → A → B → C
        ↓
H   REQ (中心)
↑       ↓
G ← F ← E ← D
```

### 9个阶段定义

```yaml
P: 预备阶段 (Preliminary Phase)
A: 架构愿景 (Architecture Vision)
B: 业务架构 (Business Architecture)
C: 信息系统架构 (Information Systems)
D: 技术架构 (Technology Architecture)
E: 机会与解决方案 (Opportunities & Solutions)
F: 迁移规划 (Migration Planning)
G: 实施治理 (Implementation Governance)
H: 架构变更管理 (Change Management)
REQ: 需求管理 (Requirements Management)
```

---

## ZeroTrust架构图设计规范

### 布局结构: 横向流程式

```
┌─────────────────────────────────────────────────────────┐
│  标题: 零信任架构核心组件                                 │
│  副标题: Zero Trust Architecture - NIST SP 800-207      │
│                                                          │
│  ┌─────┐ ① ┌─────┐ ② ┌─────┐ ③ ┌─────┐               │
│  │  S  │──→│ PEP │──→│ PDP │──→│  R  │               │
│  └─────┘   └─────┘   └─────┘   └─────┘               │
│                         │④                             │
│                         ↓                              │
│           ┌──────────────────────┐                     │
│           │  SYS  支持系统        │                     │
│           └──────────────────────┘                     │
│                                                          │
│  ┌────────────────────────────────────────────────┐    │
│  │ 核心原则: ① 持续验证 ② 最小权限 ③ 假设失陷      │    │
│  └────────────────────────────────────────────────┘    │
└─────────────────────────────────────────────────────────┘
```

### 卡片尺寸

```yaml
主组件卡片: 380 x 240 px (S/PEP/PDP/R)
支持系统卡片: 900 x 180 px (横向长条)
底部原则横条: 1600 x 80 px
```

### 步骤编号样式

```yaml
形状: 圆形
尺寸: 32 x 32 px
背景: #0066FF
数字: 18px Bold #FFFFFF
位置: 箭头正上方居中
```

### 卡片内容结构

```
┌──────────────────────┐
│ S       (字母标识)    │  48px Semibold #0066FF
│                      │
│ 主体 (中文标题)       │  32px Semibold #1A1A1A
│ Subject (英文)       │  15px Regular #6B7280
│                      │
│ 描述文字(2行以内)     │  14px Regular #9CA3AF
└──────────────────────┘
```

### 支持系统卡片样式

```yaml
背景色: #F8F9FF (浅蓝)
边框: 2px solid #E0E7FF
字母标识: SYS (48px)
内容: 横向排列
```

### 底部原则横条

```yaml
背景色: #EEF2FF (极浅蓝)
圆角: 12px
边框: none
文字: 24px Regular #0066FF
内容: 核心原则: ① 持续验证 ② 最小权限 ③ 假设失陷
```

### 位置布局

```yaml
Subject (S):  X=100,  Y=300
PEP:          X=540,  Y=300
PDP:          X=980,  Y=300
Resources (R): X=1420, Y=300
Support (SYS): X=510,  Y=600
原则横条:      X=160,  Y=860

水平间距: 440px (主卡片中心到中心)
主卡片到支持系统: 300px (垂直)
支持系统到原则: 260px (垂直)
```

### 箭头流程

```
S ──①→ PEP ──②→ PDP ──③→ R
              │
              ④
              ↓
           Support
```

### 返回箭头 (可选)

```yaml
从 R 到 S: 红色弧线 (#EF4444)
标注: ⑤ 响应返回
位置: 顶部弧线
```

### 5个组件定义

```yaml
S (Subject): 主体
  描述: 发起访问请求的实体,用户/设备/应用程序

PEP: 策略执行点 (Policy Enforcement Point)
  描述: 执行访问控制的网关,拦截请求/执行决策

PDP: 策略决策点 (Policy Decision Point)
  描述: 决策引擎和大脑,评估请求/应用策略

R (Resources): 资源
  描述: 受保护的目标资源,应用系统/数据资产

SYS (Support Systems): 支持系统
  描述: Identity Management / Security Intelligence / Continuous Monitoring
```

---

## DrawIO实现要点

### 1. XML基本结构

```xml
<mxfile host="app.diagrams.net" version="22.0.0">
  <diagram name="图表名称" id="唯一ID">
    <mxGraphModel dx="1920" dy="1080" grid="1" gridSize="8"
                  pageWidth="1920" pageHeight="1080" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />
        <!-- 元素定义 -->
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
```

### 2. 卡片元素定义

```xml
<!-- 阴影层 -->
<mxCell id="card-shadow" value=""
  style="rounded=1;fillColor=#E5E7EB;strokeColor=none;arcSize=12;"
  vertex="1" parent="1">
  <mxGeometry x="84" y="254" width="340" height="200" />
</mxCell>

<!-- 主卡片 -->
<mxCell id="card-bg" value=""
  style="rounded=1;fillColor=#FFFFFF;strokeColor=#E0E7FF;strokeWidth=2;arcSize=12;"
  vertex="1" parent="1">
  <mxGeometry x="80" y="250" width="340" height="200" />
</mxCell>

<!-- 图标字母 -->
<mxCell id="card-icon" value="P"
  style="text;fontSize=64;fontStyle=1;fontColor=#0066FF;fontFamily=Inter;align=left;"
  vertex="1" parent="1">
  <mxGeometry x="110" y="280" width="80" height="80" />
</mxCell>

<!-- 标题 -->
<mxCell id="card-title" value="预备阶段"
  style="text;fontSize=36;fontStyle=1;fontColor=#1A1A1A;fontFamily=Inter;align=left;"
  vertex="1" parent="1">
  <mxGeometry x="110" y="370" width="200" height="45" />
</mxCell>

<!-- 英文副标 -->
<mxCell id="card-subtitle" value="Preliminary Phase"
  style="text;fontSize=16;fontColor=#6B7280;fontFamily=Inter;align=left;"
  vertex="1" parent="1">
  <mxGeometry x="110" y="420" width="200" height="25" />
</mxCell>
```

### 3. 箭头定义

```xml
<mxCell id="arrow-p-a" value=""
  style="endArrow=blockThin;strokeColor=#0066FF;strokeWidth=4;
         endSize=10;endFill=1;"
  edge="1" parent="1">
  <mxGeometry relative="1" as="geometry">
    <mxPoint x="420" y="350" as="sourcePoint" />
    <mxPoint x="580" y="350" as="targetPoint" />
  </mxGeometry>
</mxCell>
```

### 4. 中心高亮卡片 (TOGAF REQ)

```xml
<mxCell id="req-bg" value=""
  style="rounded=1;fillColor=#0066FF;strokeColor=#0066FF;strokeWidth=2;arcSize=12;"
  vertex="1" parent="1">
  <mxGeometry x="580" y="530" width="340" height="200" />
</mxCell>

<mxCell id="req-icon" value="REQ"
  style="text;fontSize=64;fontStyle=1;fontColor=#FFFFFF;fontFamily=Inter;"
  vertex="1" parent="1">
  <mxGeometry x="610" y="560" width="120" height="80" />
</mxCell>

<mxCell id="req-title" value="需求管理"
  style="text;fontSize=36;fontStyle=1;fontColor=#FFFFFF;fontFamily=Inter;"
  vertex="1" parent="1">
  <mxGeometry x="610" y="650" width="280" height="45" />
</mxCell>
```

### 5. 步骤编号圆圈 (ZeroTrust)

```xml
<mxCell id="step-1-bg" value=""
  style="ellipse;fillColor=#0066FF;strokeColor=none;"
  vertex="1" parent="1">
  <mxGeometry x="455" y="230" width="32" height="32" />
</mxCell>

<mxCell id="step-1-num" value="1"
  style="text;fontSize=18;fontStyle=1;fontColor=#FFFFFF;fontFamily=Inter;"
  vertex="1" parent="1">
  <mxGeometry x="462" y="237" width="18" height="18" />
</mxCell>
```

---

## 导出规范

### DrawIO CLI导出命令

```bash
/Applications/draw.io.app/Contents/MacOS/draw.io \
  -x -f png -s 2 -t \
  文件名.drawio
```

### 导出参数说明

```yaml
-x: 批量导出模式
-f png: PNG格式
-s 2: 2倍分辨率 (1920x1080 → 3842x2162)
-t: 透明背景
```

### 输出规范

```yaml
格式: PNG RGBA
分辨率: 3842 x 2162 px
色彩深度: 8-bit/color
交错: non-interlaced
文件大小: 400-500KB (合理范围)
```

---

## 质量检查清单

### 设计合规性检查

- [ ] 画布尺寸: 1920x1080
- [ ] 背景色: #FAFBFC
- [ ] 主色: #0066FF
- [ ] 边框: 2px #E0E7FF
- [ ] 圆角: 16px
- [ ] 阴影: 0 2px 8px rgba(0,102,255,0.08)
- [ ] 字体: Inter/SF Pro/Roboto

### 内容完整性检查

- [ ] 无emoji或特殊符号
- [ ] 所有文字正确无误
- [ ] 箭头流程清晰
- [ ] 步骤编号完整
- [ ] 图标字母大写

### 布局精确性检查

- [ ] 8px网格对齐
- [ ] 元素间距80px
- [ ] 卡片尺寸精确
- [ ] 箭头端点对齐
- [ ] 文字位置统一

### 输出质量检查

- [ ] PNG分辨率: 3842x2162
- [ ] 文件格式: RGBA
- [ ] 文字清晰可读
- [ ] 颜色准确无偏差
- [ ] 无锯齿或模糊

---

## 使用示例

### 创建新的TOGAF架构图

```
1. 使用本prompt的"TOGAF架构图设计规范"部分
2. 创建1920x1080画布,背景#FAFBFC
3. 按照3×3矩阵布局放置9个阶段卡片
4. 中心REQ卡片使用纯蓝背景+白字
5. 添加箭头连接(4px #0066FF)
6. 导出PNG (2倍分辨率)
```

### 创建新的ZeroTrust架构图

```
1. 使用本prompt的"ZeroTrust架构图设计规范"部分
2. 创建1920x1080画布,背景#FAFBFC
3. 横向排列4个主组件卡片(380x240px)
4. 中间添加支持系统横条(900x180px)
5. 底部添加原则横条(1600x80px)
6. 添加步骤编号圆圈和箭头
7. 导出PNG (2倍分辨率)
```

---

## 版本信息

```yaml
版本: V6
创建日期: 2025-10-30
设计师: AISecOps Design Team
设计理念: 极简主义 + 扁平化2.0
适用场景: 企业级架构图、技术白皮书、专业出版物
授权: 可复用于所有 AISecOps 项目相关图表
```

---

## 附录: 颜色参考

### 主色板

```
#0066FF - 纯蓝 (主色)
#E0E7FF - 淡蓝 (边框)
#F8F9FF - 极淡蓝 (支持系统背景)
#EEF2FF - 超淡蓝 (原则横条背景)
#FAFBFC - 灰白 (画布背景)
#FFFFFF - 纯白 (卡片背景)
```

### 文字色板

```
#1A1A1A - 近黑 (标题)
#6B7280 - 中灰 (副标题)
#9CA3AF - 浅灰 (描述文字)
#E5E7EB - 极浅灰 (阴影)
```

### 强调色

```
#EF4444 - 红色 (返回箭头)
```

---

**文件路径要求：在 diagrams 各自目录下生成 drawio 文件和 png文件，然后copy png 到images 中对应的目录。
**


**备注**: 本prompt为V6版本设计规范的完整固化文档,可直接用于指导AI或设计师创建符合标准的架构图。所有尺寸、颜色、间距均已精确定义,确保输出一致性和专业性。
