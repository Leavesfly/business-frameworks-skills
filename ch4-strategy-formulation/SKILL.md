---
name: ch4-strategy-formulation
description: "Chapter 4 · Strategy Formulation. Use to converge creative options into executable, measurable strategy covering business model, product, GTM, and operating plan. Contains 14 frameworks: BCG/PPM product portfolio, Ansoff growth matrix, Cross-SWOT (TOWS), STP, Positioning Map, Business Model Canvas (BMC), Architecture Diagram, AIDMA funnel, Gantt Chart, Org Chart, Roadmap, KPI Tree (North Star), AARRR pirate metrics, SMART goals. 关键词：strategy formulation, BCG matrix, PPM, Ansoff matrix, TOWS cross SWOT, STP, positioning map, business model canvas, BMC, architecture diagram, AIDMA, AIDA, Gantt chart, org chart, product roadmap, KPI tree, north star metric, AARRR pirate metrics, SMART goals, OKR, 战略规划, 定位, 商业模式, 路线图, 北极星指标, 海盗指标, 目标拆解。"
---

# 第 4 章 · 制订策略（Strategy Formulation）

**定位**：小循环② 的收敛端。把发散出来的创意收敛为结构化、可执行、可度量的战略与计划。

**与其他章的关系**：
- ⇄ `ch3-solution-ideation`（小循环②）
- → `ch5-business-improvement` / `ch6-org-management`（落地到运营和组织）
- → `ch1-problem-discovery`（大循环：执行后回到问题发现）

---

## 框架清单（32–45）

### ㉜ 产品组合矩阵（PPM / BCG Matrix）
- **用途**：判断每个产品/业务单元应加大投入、维持、收割还是放弃。
- **两维**：市场增长率（高/低）× 相对市场份额（高/低）
- **四象限**：
  - 明星 Star（高增长 × 高份额）→ 持续投入
  - 金牛 Cash Cow（低增长 × 高份额）→ 挤奶
  - 问题 Question Mark（高增长 × 低份额）→ 选择性投入
  - 瘦狗 Dog（低增长 × 低份额）→ 退出/剥离
- **模板**：
  ```
  市场增长率 ↑
       │ ★明星      │ ?问题
       │ 加大投入   │ 选择性投入
    高 ├────────────┼────────────
       │ 💰金牛     │ 🐕瘦狗
       │ 现金流来源 │ 退出/剥离
    低 └────────────┴────────────→ 相对份额
         高            低
  ```
- **英文关键词**：BCG matrix, PPM, product portfolio

### ㉝ 安索夫矩阵（Ansoff Matrix）
- **用途**：选择增长路径。
- **两维**：产品（既有/新）× 市场（既有/新）
- **四策略**：
  - 市场渗透（既有产品 × 既有市场）
  - 产品开发（新产品 × 既有市场）
  - 市场开发（既有产品 × 新市场）
  - 多角化（新产品 × 新市场，风险最高）
- **模板**：
  ```
              既有市场       新市场
  既有产品  市场渗透        市场开发
  新产品    产品开发        多角化
  ```
- **英文关键词**：Ansoff matrix, growth strategy

### ㉞ 交叉 SWOT（TOWS / Cross-SWOT）
- **用途**：把第 2 章的 `SWOT`⑫ 从静态清单升级为动态策略。
- **四组合**：
  - **SO**（强项 × 机会）：进攻策略
  - **WO**（弱项 × 机会）：改善策略
  - **ST**（强项 × 威胁）：防御策略
  - **WT**（弱项 × 威胁）：规避/撤退策略
- **模板**：
  ```
  |         | 机会 O        | 威胁 T        |
  |---------|---------------|---------------|
  | 优势 S  | SO 进攻策略   | ST 防御策略   |
  | 劣势 W  | WO 改善策略   | WT 规避策略   |
  ```
- **英文关键词**：cross SWOT, TOWS matrix

### ㉟ STP
- **用途**：营销战略三部曲。
- **步骤**：
  1. **S**egmentation 细分：按人口/行为/心理切分市场
  2. **T**argeting 目标选择：选最有吸引力的 1–3 个细分
  3. **P**ositioning 定位：一句话说明"在目标客户心中我是谁"
- **模板**：
  ```
  S 细分维度与切片：
  T 目标细分与理由：
  P 定位陈述：对【目标客户】而言，我们是【品类】中
    【独特价值】的选择，因为【支撑点】。
  ```
- **英文关键词**：STP, segmentation targeting positioning

### ㊱ 定位图（Positioning Map / Perceptual Map）
- **用途**：在两维坐标中可视化竞品 vs 自家的位置，寻找空白地。
- **步骤**：
  1. 选两个对用户最关键的维度（如"价格 × 品质"、"功能 × 情感"）
  2. 把所有竞品按感知打点
  3. 找到没被占据的象限 → 自家定位
- **模板**：
  ```
      维度 Y 高
         │ • 竞品A        • 竞品B
         │
  ───────┼─────────────→ 维度 X 高
         │ • 我们?        • 竞品C
      低 │
  ```
- **英文关键词**：positioning map, perceptual map

### ㊲ 商业模式图（Business Model Canvas）
- **用途**：用 9 格一页纸说清一门生意（右半侧=价值与客户，左半侧=交付与成本）。
- **九格**：KP 关键伙伴 / KA 关键活动 / KR 关键资源 / VP 价值主张 / CR 客户关系 / CH 渠道通路 / CS 客户细分 / C$ 成本结构 / R$ 收入来源
- **布局**：
  ```
  ┌──────┬──────┬──────────┬──────┬──────────┐
  │关键   │关键   │          │客户   │          │
  │伙伴   │活动   │          │关系   │          │
  │       ├──────┤ 价值主张 ├──────┤ 客户细分 │
  │       │关键   │          │渠道   │          │
  │       │资源   │          │通路   │          │
  ├───────┴──────┴──────────┴──────┴──────────┤
  │ 成本结构                   │  收入来源      │
  └────────────────────────────┴────────────────┘
  ```
- **推荐填写顺序**：CS 客户 → VP 价值主张 → CH 渠道 → CR 关系 → R$ 收入 → KR 资源 → KA 活动 → KP 伙伴 → C$ 成本。
- **英文关键词**：business model canvas, BMC, Osterwalder, value proposition canvas

### ㊳ 架构图（Architecture Diagram）
- **用途**：把业务/产品/系统的要素与关系画成图。
- **常见类型**：
  - 业务架构：客户 → 渠道 → 产品 → 能力 → 数据
  - 产品架构：模块层级 + 依赖
  - 技术架构：前端/后端/中间件/基础设施分层
- **模板**：分层横切 + 纵向贯通线 + 外部接口
- **英文关键词**：architecture diagram, layered architecture

### ㊴ AIDMA
- **用途**：描述消费者决策漏斗。
- **五阶段**：**A**ttention 注意 → **I**nterest 兴趣 → **D**esire 欲望 → **M**emory 记忆 → **A**ction 行动
- **模板**：每一阶段列出【用户心理状态 + 对应营销动作 + 转化指标】。
  ```
  | 阶段 | 用户心理 | 营销动作 | 转化指标 |
  |------|---------|---------|---------|
  | A    |         |         |         |
  | I    |         |         |         |
  | D    |         |         |         |
  | M    |         |         |         |
  | A    |         |         |         |
  ```
- **英文关键词**：AIDMA, AIDA, marketing funnel

### ㊵ 甘特图（Gantt Chart）
- **用途**：项目任务排期可视化。
- **要素**：任务名 / 负责人 / 起止时间 / 依赖关系 / 里程碑
- **模板**：
  ```
  任务       负责人  W1 W2 W3 W4 W5 W6
  需求调研   张      ██
  方案设计   李         ████
  开发       王            ████████
  测试       赵                   ████
  上线       —                        ▲
  ```
- **英文关键词**：Gantt chart, schedule, milestones

### ㊶ 组织结构图（Organizational Chart）
- **用途**：呈现岗位、汇报线、职责。
- **常见形态**：直线职能型 / 事业部型 / 矩阵型 / 扁平型
- **要素**：职位名 + 在岗人 + 汇报关系 + 职责一句话
- **英文关键词**：org chart, reporting line

### ㊷ 路线图（Roadmap）
- **用途**：把战略按时间轴和主题铺开。
- **维度**：纵轴主题（产品/市场/组织/技术）× 横轴时间（季度/半年/年）
- **模板**：
  ```
                Q1        Q2        Q3        Q4
  产品         ▇▇▇▇      ▇▇▇▇      ▇▇▇▇      ▇▇▇▇
  市场         ▇▇▇       ▇▇▇▇▇▇    ▇▇▇▇      ▇▇▇▇▇
  组织         ▇▇        ▇▇▇▇      ▇▇▇▇▇▇    ▇▇▇▇
  技术         ▇▇▇▇▇▇    ▇▇▇▇      ▇▇▇       ▇▇▇▇▇
  里程碑      ▲ α       ▲ β        ▲ GA     ▲ v2.0
  ```
- **英文关键词**：roadmap, product roadmap, strategic roadmap

### ㊸ KPI 树状图（KPI Tree）
- **用途**：把北极星指标拆成可驱动的子指标，确保每个团队都有直接影响的动作层。
- **步骤**：
  1. 顶层：北极星指标（如 GMV、MAU、NPS）
  2. 第二层：按公式/逻辑拆（如 GMV = UV × 转化率 × 客单价）
  3. 继续拆到团队可直接影响的动作层
  4. 每个叶子节点配 **Owner + 目标值 + 成本**
- **模板**：
  ```
  北极星指标
  ├─ 子指标 A（= x × y）
  │   ├─ x 动作（Owner: 张）
  │   └─ y 动作（Owner: 李）
  └─ 子指标 B
  ```
- **英文关键词**：KPI tree, north star metric, metric tree, OKR, input vs output metric

### ㊹ AARRR（海盗指标 / 用户增长漏斗）
- **用途**：互联网产品的增长五步漏斗。
- **五阶段**：
  - **A**cquisition 获取
  - **A**ctivation 激活
  - **R**etention 留存
  - **R**evenue 收入
  - **R**eferral 推荐
- **模板**：
  ```
  | 阶段        | 定义 | 关键指标 | 当前值 | 目标值 | 动作 |
  |-------------|------|---------|-------|-------|------|
  | Acquisition |      |         |       |       |      |
  | Activation  |      |         |       |       |      |
  | Retention   |      |         |       |       |      |
  | Revenue     |      |         |       |       |      |
  | Referral    |      |         |       |       |      |
  ```
- **英文关键词**：AARRR, pirate metrics, growth funnel

### ㊺ SMART（目标设定）
- **用途**：检验目标是否"可执行"。
- **五要素**：
  - **S**pecific 具体
  - **M**easurable 可衡量
  - **A**chievable 可达成
  - **R**elevant 相关
  - **T**ime-bound 有时限
- **模板**：
  ```
  原始目标：___
  | 要素       | 检查 | 改写 |
  |------------|------|------|
  | Specific   |      |      |
  | Measurable |      |      |
  | Achievable |      |      |
  | Relevant   |      |      |
  | Time-bound |      |      |
  SMART 化目标：___
  ```
- **英文关键词**：SMART goals, goal setting

---

## 常用组合

- **战略总盘** → `交叉 SWOT`㉞ → `STP`㉟ → `定位图`㊱ → `商业模式图`㊲
- **业务增长** → `安索夫`㉝ → `AARRR`㊹ → `KPI 树`㊸
- **产品投资** → `产品组合矩阵`㉜ → `商业模式图`㊲ → `路线图`㊷
- **营销设计** → `AIDMA`㊴ + `定位图`㊱
- **落地执行** → `路线图`㊷ + `甘特图`㊵ + `组织结构图`㊶ + `SMART`㊺ + `KPI 树`㊸

## 输出契约

完成本章后必须产出：
1. **一句话战略陈述**（用 `STP`㉟ 定位句或 `商业模式图`㊲ 价值主张）
2. **季度/年度路线图**（`路线图`㊷）
3. **北极星指标 + KPI 树**（`KPI 树`㊸）
4. **甘特图 + 责任分工**（`甘特图`㊵ + `组织结构图`㊶）
5. **建议下一步**：
   - 执行层 → 转入 `ch5-business-improvement`（流程）+ `ch6-org-management`（人）
   - 对外沟通 → 转入 `ch7-communication-sharing`（汇报）
   - 执行一段时间后 → 大循环回到 `ch1-problem-discovery`

---

## 扩展资源

- **BMC 行业样例**（SaaS / 餐饮连锁 / 双边平台 三个完整填写范例 + 九格自检清单）：见 [references/bmc-examples.md](references/bmc-examples.md)
- **增长策略实战案例**（安索夫矩阵、BCG矩阵、AARRR海盗指标、KPI树拆解、SMART目标改写）：见 [references/growth-strategy-examples.md](references/growth-strategy-examples.md)
- **STP定位与定位图案例**（STP完整案例、定位图分析、TOWS交叉SWOT、定位陈述公式）：见 [references/stp-positioning-examples.md](references/stp-positioning-examples.md)
