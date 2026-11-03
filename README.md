# clinical-trial-appraiser

> **通用型“1+6+1”临床试验全景解构、方法学审稿与衍生课题立项（IIT Protocol & SAP）智能体技能**  
> *A Claude Code & AI Agent Skill for Comprehensive Clinical Trial Appraisal, Methodological Peer Review, and Investigator-Initiated Trial (IIT) Design based on the "1+6+1" Framework.*

---

## 🌟 核心理念：从“被动接收药效”到“主动挖掘立项矿脉”

面对顶刊（NEJM、Lancet、JAMA、ARD、ERJ 等）发表的重磅新药确证性临床试验，大多数临床医生往往停留在“主要终点阳性与否”的药效记忆层面。

**`clinical-trial-appraiser`** 将顶级医学期刊方法学审稿人（Peer Reviewer）、临床生物统计学家与转化医学科学家的审稿智慧固化为一套结构化的 **“1 + 6 + 1”全景分析闭环体系**：
1. **穿透入排漏斗**：审视表面宣称与底层筛选人群的严重偏倚（如 78.8% UIP 模式把控）；
2. **刺破对标谬误**：横向对标历史基石试验，严格遵守跨研究不可比原则；
3. **闭环药理机制**：用分子靶点、微血管内皮保护解释临床“肺功能与生存获益割裂”的矛盾表象；
4. **逆向映射立项（Gap-to-Protocol）**：将顶刊为保证内部真实性妥协排减的一线标准治疗（如 MMF 排除），转化为中国学者可直接落地的国家级前瞻性队列与 IIT 方案；
5. **生物统计极限崩溃点**：复盘时间轴、样本量灵敏度、多重门控断裂、复合终点稀释与倾覆点（Tipping-Point）压力测试。

---

## 🏗️ “1 + 6 + 1”三段式闭环架构

```
                     ┌─────────────────────────────────────────┐
                     │ 模块 A (前置 1)：原文速览与基本面锚定    │
                     │  • 核心科学悬念 (Core Question)          │
                     │  • 结构化 PICOs 图谱快照                 │
                     │  • 顶线结果判定 (Topline Verdict)        │
                     └────────────────────┬────────────────────┘
                                          │
                                          ▼
                     ┌─────────────────────────────────────────┐
                     │ 模块 B (核心 6)：六维方法学深度透视      │
                     │  • D1: PICO 深层动机与人群异质性控场术    │
                     │  • D2: 历史基石群像横向对标 (SLS/INBUILD) │
                     │  • D3: 全谱系适应症审计与未满足需求      │
                     │  • D4: 药理机制闭环与因果合理性互证      │
                     │  • D5: 从论文到临床落地鸿沟 (SoC 违背)   │
                     │  • D6: 中国学者自主课题衍生 (IIT 孵化)   │
                     └────────────────────┬────────────────────┘
                                          │
                                          ▼
                     ┌─────────────────────────────────────────┐
                     │ 模块 C (收尾 +1)：生物统计极限崩溃点审视 │
                     │  • S1: 试验架构、时间轴与样本量灵敏度    │
                     │  • S2: 终点选择效能与复合终点稀释效应    │
                     │  • S3: 缺失假设、MNAR 与 Tipping-Point  │
                     │  • S4: 跨研究对比禁忌与 100PY 暴露校正   │
                     └─────────────────────────────────────────┘
```

---

## 🚀 安装指南 (Installation)

### 适用平台
- **Claude Code** (`~/.claude/skills/` 或项目目录)
- **Codex / Agentic IDE** (`.agents/skills/`)
- **Orca / Antigravity Agent**

### 一键安装

```bash
# 方式 1：全局安装到 Claude Code skills
git clone https://github.com/qitong/clinical-trial-appraiser ~/.claude/skills/clinical-trial-appraiser

# 方式 2：克隆至项目本地 agents 技能库
mkdir -p .agents/skills
git clone https://github.com/qitong/clinical-trial-appraiser .agents/skills/clinical-trial-appraiser
```

---

## 💡 触发方式与使用示例 (Usage)

在与 Agent 对话时，只需提供临床试验文献（PDF、DOI、或试验名称，如 FIBRONEER、INBUILD、SENSCIS、RECITAL），并输入提示词：

### 常用触发词
- *“请用‘1+6+1’框架对这篇 NEJM 临床试验进行全景方法学解构。”*
- *“拆解 FIBRONEER 试验的入组漏斗、统计门控断裂与中国学者衍生立项方向。”*
- *“评价这篇临床论文的真实世界落地鸿沟，并逆向生成一份多中心前瞻性 IIT 方案。”*

### 典型输出成果
1. **万字审稿人级全景解构报告**（Markdown 格式，含 PICOs 图谱、基石对标矩阵表与统计门控图）；
2. **立项级临床研究方案初稿（Protocol）**（遵循 SPIRIT / ICH-GCP 规范）；
3. **统计分析计划初稿（SAP）**（包含 MMRM 模型设定、最差分位数插补及倾覆点参数设置）。

---

## 🔗 配套推荐技能 (Ecosystem)

- **`clinical-biostat-writer`**：负责运行真实世界临床队列数据，拟合 MMRM、竞争风险模型并一键生成 Nature/NEJM 级三线表与 SCI 初稿。
- **`develop-resp-question`**：呼吸与风湿免疫领域科研立题教练技能 ([qitong/develop-resp-question](https://github.com/qitong/develop-resp-question))。
- **`appraise-paper`**：基于 Nature 2026 七步法的通用文献批判性精读技能 ([qitong/appraise-paper](https://github.com/qitong/appraise-paper))。

---

## 📄 开源许可 (License)

MIT License. 欢迎临床科研工作者、审稿人与医学统计同行 Star 与贡献！
