---
name: ch5-business-improvement
description: Chapter 5 · Business Improvement. Use during execution to streamline processes, boost efficiency, enforce quality, and run retrospectives. Contains 10 frameworks: KPT retro, YWT retro, PDCA cycle, Business Inventory, BPMN Flowchart (swimlane), PERT/CPM, RACI matrix, Muda/Mura/Muri (lean 3M), ECRS, Kaizen Improvement Proposal. 关键词：business improvement, kaizen, lean manufacturing, muda mura muri, 7 wastes, KPT retrospective, YWT, PDCA Deming cycle, business inventory, work audit, BPMN flowchart, swimlane, PERT chart, critical path, RACI matrix, responsibility assignment, ECRS, improvement proposal, 精益, 改善, 流程优化, 复盘, 职责分工, 浪费识别, 关键路径。
---

# 第 5 章 · 改善业务（Business Improvement）

**定位**：支援性活动。当战略已在执行、需要提升内部运营效率与流程质量时使用。

**与其他章的关系**：
- ← `ch4-strategy-formulation`（战略落地到业务流程）
- 可与 `ch6-org-management` 并行使用（流程 × 人员）
- 复盘结果反馈到 `ch1-problem-discovery` 开启大循环

---

## 框架清单（46–55）

### ㊻ KPT（Keep / Problem / Try）
- **用途**：敏捷团队每个迭代末的快速复盘。
- **三栏**：
  - **K**eep：做得好、要继续做的
  - **P**roblem：遇到的问题
  - **T**ry：下个周期想尝试的改进
- **模板**：
  ```
  ┌─────────────┬─────────────┐
  │ Keep 保持    │ Problem 问题│
  │ - ...       │ - ...       │
  ├─────────────┴─────────────┤
  │ Try 下次尝试              │
  │ - ...                     │
  └───────────────────────────┘
  ```
- **英文关键词**：KPT retrospective, agile retro

### ㊼ YWT（やったこと / わかったこと / 次にやること）
- **用途**：日式复盘三段法，比 KPT 更强调"学到了什么"。
- **三段**：
  - **Y**atta こと 做过的事（事实）
  - **W**akatta こと 学到的事（洞察）
  - **T**sugini やること 下一步要做的事（行动）
- **模板**：
  ```
  | 做过（事实） | 学到（洞察） | 下一步（行动） |
  |-------------|-------------|---------------|
  |             |             |               |
  ```
- **英文关键词**：YWT retrospective, did learned next

### ㊽ PDCA（核验表 / Plan-Do-Check-Act）
- **用途**：持续改善循环。
- **四步**：
  - **P**lan 计划：目标 + 方法 + 指标
  - **D**o 执行：按计划实施，记录过程
  - **C**heck 检查：对比目标与实际结果，分析差异
  - **A**ct 处置：标准化成功做法 / 修正问题 / 启动下一轮
- **模板（核验表）**：
  ```
  | 阶段 | 要点                  | 检查项                      | 状态 |
  |------|----------------------|-----------------------------|------|
  | P    | 目标明确？方法可行？   | ☐ 目标 ☐ 指标 ☐ 资源 ☐ 时间 |      |
  | D    | 按计划执行？记录完整？ | ☐ 执行 ☐ 记录 ☐ 偏差说明    |      |
  | C    | 实际 vs 目标差距？    | ☐ 数据 ☐ 原因分析           |      |
  | A    | 固化/修正/下一轮？    | ☐ 标准化 ☐ 改进 ☐ 再循环    |      |
  ```
- **英文关键词**：PDCA cycle, Deming cycle, plan do check act

### ㊾ 业务盘点表（Business Inventory）
- **用途**：把部门/岗位的所有工作事项列清，便于盘活、合并、外包、自动化。
- **模板**：
  ```
  | 事项 | 频次 | 耗时 | 价值 | 难度 | 负责人 | 处置建议 |
  |------|------|------|------|------|--------|---------|
  |      | 日/周/月 | 小时 | 高/中/低 | 高/中/低 |  | 保留/合并/外包/自动化/砍掉 |
  ```
- **英文关键词**：business inventory, work audit, task audit

### ㊿ 业务流程图（Business Process Flowchart / BPMN）
- **用途**：把一条业务流程的步骤、判断、角色画出来。
- **基础符号**：
  - 圆角矩形 / 椭圆：开始 & 结束
  - 矩形：流程步骤
  - 菱形：判断分支
  - 箭头：流向
  - 泳道：按角色分区
- **模板**（泳道式）：
  ```
  角色 A │  [开始] → [步骤1] ─────────────→ [步骤4] → [结束]
         │                ↘              ↗
  角色 B │                 [步骤2] → ◇判断
         │                           ↓否
  角色 C │                         [步骤3] ↺
  ```
- **英文关键词**：flowchart, BPMN, swimlane, process map

### 51 PERT 图（Program Evaluation and Review Technique / CPM）
- **用途**：项目任务依赖网络 + 关键路径识别。
- **步骤**：
  1. 列出所有任务及其前置依赖
  2. 估计每个任务的乐观（O）/ 最可能（M）/ 悲观（P）时长
  3. 期望时长 = (O + 4M + P) / 6
  4. 画出网络图，找出最长路径 = **关键路径**
- **模板**：
  ```
  | 任务 | 前置 | O | M | P | 期望时长 | 是否关键路径 |
  |------|------|---|---|---|---------|-------------|
  ```
- **英文关键词**：PERT chart, CPM, critical path

### 52 RACI（职责分工矩阵）
- **用途**：明确每件事谁做、谁决策、谁支持、谁知情。
- **四角色**：
  - **R**esponsible 执行者（动手做）
  - **A**ccountable 负责人（最终拍板，每件事只能 1 人）
  - **C**onsulted 被咨询者（提供意见，双向沟通）
  - **I**nformed 被告知者（只接收结果，单向沟通）
- **模板**：
  ```
  | 任务 \ 角色 | 张 | 李 | 王 | 赵 |
  |-------------|----|----|----|----|
  | 任务 1      | R  | A  | C  | I  |
  | 任务 2      | A  | R  | I  | C  |
  ```
- **英文关键词**：RACI matrix, responsibility assignment

### 53 不足 / 过剩 / 不均（Muda / Mura / Muri，精益 3M）
- **用途**：从精益视角识别浪费。
- **三类**：
  - **Muda 不足/浪费**：无附加值的动作
  - **Mura 不均**：波动/起伏（需求忽高忽低、质量不稳）
  - **Muri 过剩/过载**：超负荷（人机设备超常运转）
- **丰田 7 大浪费（TIMWOOD）**：
  - **T**ransport 搬运
  - **I**nventory 库存
  - **M**otion 动作
  - **W**aiting 等待
  - **O**verproduction 过量生产
  - **O**ver-processing 过度加工
  - **D**efects 不良品
- **模板**：
  ```
  | 环节 | 是否有 Muda | 是否有 Mura | 是否有 Muri | 具体浪费类型 | 改善动作 |
  |------|-------------|-------------|-------------|-------------|----------|
  ```
- **英文关键词**：muda mura muri, 3M waste, lean 7 wastes, TIMWOOD, TPS

### 54 ECRS（Eliminate / Combine / Rearrange / Simplify）
- **用途**：对每个流程步骤做"四问"式改造。
- **四问**：
  1. **E**liminate 能否取消？（不做会怎样？）
  2. **C**ombine 能否合并？（与其他步骤一起做？）
  3. **R**earrange 能否重排？（换顺序或换人做？）
  4. **S**implify 能否简化？（用更省力的方式？）
- **使用顺序**：先 E（能去掉不花力气去优化），再 C/R（整合），最后 S（打磨）。
- **模板**：
  ```
  | 流程步骤 | E | C | R | S | 改造结果 |
  |---------|---|---|---|---|---------|
  ```
- **英文关键词**：ECRS, process improvement, work simplification, IE

### 55 业务改善提案表（Improvement Proposal Sheet）
- **用途**：把改善想法结构化提交，便于评审与追踪。
- **模板**：
  ```
  提案人：               部门：              日期：
  ────────────────────────────────────────
  【现状 As is】：
  【问题 / 浪费点】：
  【改善方案 To be】：
  【预期效果】（可量化）：省时 / 省钱 / 提质 / 增安
  【所需资源 & 成本】：
  【试点范围与周期】：
  【风险 & 应对】：
  ────────────────────────────────────────
  评审意见：             负责人：           预计上线：
  ```
- **英文关键词**：kaizen proposal, improvement suggestion

---

## 常用组合

- **快速复盘** → `KPT`㊻ 或 `YWT`㊼
- **结构化改进循环** → `PDCA`㊽ 贯穿全程
- **梳理业务** → `业务盘点表`㊾ → `业务流程图`㊿
- **项目排期** → `PERT 图`51 + 第 4 章 `甘特图`㊵
- **分工不清** → `RACI`52
- **流程优化深挖** → `不足/过剩/不均`53 → `ECRS`54 → `业务改善提案表`55

## 输出契约

完成本章后必须产出：
1. **现状流程图 + 问题清单**（`业务流程图`㊿ + `不足/过剩/不均`53）
2. **改进后的流程 + ECRS 对照表**（`ECRS`54）
3. **分工矩阵**（`RACI`52）
4. **改善提案**（`业务改善提案表`55）
5. **复盘机制**（`PDCA`㊽ / `KPT`㊻ / `YWT`㊼ 的周期约定）
6. **建议下一步**：
   - 人员问题浮现 → 转入 `ch6-org-management`
   - 需要向上汇报 → 转入 `ch7-communication-sharing`
   - 暴露出新问题 → 大循环回到 `ch1-problem-discovery`

---

## 扩展资源

- **改善样例**（售后退款流程案例，涵盖 PDCA / RACI / Muda-TIMWOOD / ECRS / KPT / YWT / PERT）：见 [references/examples.md](references/examples.md)
