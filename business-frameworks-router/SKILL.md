---
name: business-frameworks-router
description: 'Business & management problem router over 70+ thinking frameworks from the MAP book. Auto-triages any request involving problem discovery, market analysis, ideation, strategy, business improvement, team management, or reporting, and orchestrates 1-3 frameworks into a structured answer. Use proactively when the user mentions business frameworks, consulting-style analysis, SWOT/PEST/STP/BMC/OKR/KPI/RACI/PDCA/GROW, or asks "how should I analyze / plan / improve / pitch X". 关键词：business framework, problem solving, strategy planning, market analysis, brainstorming, process improvement, team management, presentation, consulting toolkit, 商业框架, 思维模型, 问题解决, 分析方法, 策略规划, 管理工具, 汇报模板, 咨询工具箱。'
---

# 商业框架路由器 · business-frameworks-router

本 skill 是 70+ 商业思维框架的**总入口**，负责理解用户问题 → 分诊到合适的子 skill → 按"小循环/大循环"组合多个框架 → 产出结构化结论。

---

## 一、何时触发本 skill

当用户提出以下类型的问题时，**立即激活**：

- "帮我分析一下 XX 市场 / 公司 / 产品"
- "这个问题该怎么解决 / 从哪入手"
- "帮我做一份策略 / 方案 / 规划"
- "团队 / 组织 / 绩效出了问题"
- "帮我优化这个流程 / 业务"
- "把这个想法整理成汇报 / 提案"
- 任何包含 "框架 / 模型 / 矩阵 / 分析方法 / 画布 / 模板" 字眼的请求

**意图 → 子 skill 速查表**：

| 用户话术里出现 | 优先进入 |
|---|---|
| 问题模糊 / 搞不清楚 / 怎么拆 / 根因 / 差距 | `ch1-problem-discovery` |
| 市场 / 竞争 / 用户 / 行业 / 画像 / 旅程 | `ch2-market-analysis` |
| 点子 / 创意 / 脑暴 / 发散 / 方案 | `ch3-solution-ideation` |
| 战略 / 定位 / 商业模式 / 路线图 / KPI / 北极星 | `ch4-strategy-formulation` |
| 流程 / 效率 / 浪费 / 复盘 / 分工 | `ch5-business-improvement` |
| 团队 / 下属 / 激励 / 辅导 / 绩效 / 干系人 | `ch6-org-management` |
| 汇报 / 演讲 / 提案 / 方案书 / 一页纸 | `ch7-communication-sharing` |

---

## 二、子 skill 目录

| 子 skill | 对应章节 | 核心用途 | 框架编号 | 数量 |
|---|---|---|---|---|
| `ch1-problem-discovery` | 第 1 章 发现问题、课题 | 识别 & 定义问题 | 01–08 | 8 |
| `ch2-market-analysis` | 第 2 章 分析市场 | 市场 / 竞争 / 客户洞察 | 09–21 | 13 |
| `ch3-solution-ideation` | 第 3 章 思索课题的解决方法 | 创意发散与初筛 | 22–31 | 10 |
| `ch4-strategy-formulation` | 第 4 章 制订策略 | 战略规划与落地 | 32–45 | 14 |
| `ch5-business-improvement` | 第 5 章 改善业务 | 流程 / 效率 / 复盘 | 46–55 | 10 |
| `ch6-org-management` | 第 6 章 管理组织 | 团队 / 激励 / 辅导 | 56–66 | 11 |
| `ch7-communication-sharing` | 第 7 章 传达与共享 | 沟通与汇报 | 67–70 | 4 |

---

## 三、自动路由决策树（基于 MAP 的小循环 / 大循环）

```
用户问题进入
│
├─ ① 问题是否清晰？
│   └─ 否 → 进入【小循环①：深究问题】
│            ch1-problem-discovery ⇄ ch2-market-analysis
│            （边发现边分析，直到问题被精确定义）
│
├─ ② 是否已经有清晰的问题，需要找方案？
│   └─ 是 → 进入【小循环②：拟定策略】
│            ch3-solution-ideation ⇄ ch4-strategy-formulation
│            （创意发散 → 策略收敛，来回迭代）
│
├─ ③ 问题是"内部运作"类（流程 / 团队）？
│   ├─ 流程/业务改善 → ch5-business-improvement
│   └─ 团队/人员管理 → ch6-org-management
│
├─ ④ 需要把结果讲给别人？
│   └─ 是 → ch7-communication-sharing
│
└─ ⑤ 执行后得到新结果 → 【大循环】回到 ① 处理下一个问题
```

---

## 四、标准工作流（SOP）

每次接到任务，按如下步骤执行：

### Step 1：问题分诊（Triage）
输出一段"问题画像"，明确：
- **问题类型**：问题发现 / 市场分析 / 方案构思 / 战略制定 / 业务改善 / 组织管理 / 对外沟通
- **处于循环的哪个环节**：小循环① / 小循环② / 大循环 / 内部支援 / 对外共享
- **建议进入的子 skill**（可 1 个或多个）

### Step 2：框架选型（Framework Selection）
在对应子 skill 中挑选 **1–3 个最合适的框架**，说明为什么选它们。

### Step 3：引导式应用（Guided Application）
逐个框架：
1. 简述框架是什么 & 为什么适用当前场景
2. 列出**提问清单**引导用户填写（或基于已有信息直接填充）
3. 用框架标准**模板**（表格 / 矩阵 / 画布）输出结果
4. 给出**解读与建议**

### Step 4：串联与跃迁（Chaining）
若当前循环未闭环，主动提示下一步：
- 小循环①未闭环 → "要不要再用 `SWOT` 交叉验证一下问题定义？"
- 小循环②未闭环 → "方案已出，要不要用 `商业模式图` 做落地检验？"
- 大循环触发 → "执行一段时间后，建议用 `KPT` 或 `PDCA` 回顾"

### Step 5：产出归档（Deliverable）
最终统一输出：
- **问题定义**（1 句话）
- **使用框架清单**（带编号）
- **关键结论**（3–5 条）
- **下一步行动**（含负责人 / 期限建议）

---

## 五、常见场景快捷组合（Recipes）

| 场景 | 推荐组合 |
|---|---|
| 新产品立项 | `6W2H`② → `PEST`⑨ → `SWOT`⑫ → `STP`㉟ → `商业模式图`㊲ → `产品策划书`67 |
| 老产品下滑 | `As is/To be`① → `帕雷托`⑬ → `逻辑树状图`⑤ → `头脑风暴`㉒ → `决策矩阵`⑧ |
| 市场进入决策 | `PEST`⑨ → `五力分析`⑩ → `VRIO`⑪ → `安索夫矩阵`㉝ → `定位图`㊱ |
| 客户洞察 | `人物画像`⑮ → `同理心地图`⑯ → `客户体验旅程图`⑰ |
| 创意发散 | `头脑风暴`㉒ → `曼陀罗`㉓ → `奥斯本核验表`㉖ → `报酬矩阵`㉛ |
| 团队绩效差 | `任务愿景价值`56 → `Will/Can/Must`57 → `Will/Skill`65 → `GROW`66 → `KPT`㊻ |
| 流程低效 | `业务流程图`㊿ → `不足/过剩/不均`53 → `ECRS`54 → `PDCA`㊽ → `RACI`52 |
| 项目排期 | `PERT`51 → `甘特图`㊵ → `RACI`52 → `SMART`㊺ |
| 汇报方案 | `PREP`69（结论先行） / `TAPS`70（问题汇报） |
| 复盘 | `KPT`㊻ / `YWT`㊼ / `PDCA`㊽ |

---

## 六、调用约定

- **默认语言**：中文输出，框架名保留英文/缩写（如 `SWOT`、`PDCA`、`GROW`）
- **统一编号**：每个框架用 MAP 图编号（01–70），便于追溯
- **输出格式**：Markdown，表格/矩阵优先
- **循环提示**：每产出一版结论，追问"是否进入下一循环"

---

## 七、子 skill 索引（详细用法见各自的 SKILL.md）

- [发现问题、课题](../ch1-problem-discovery/SKILL.md)
- [分析市场](../ch2-market-analysis/SKILL.md)
- [思索解决方法](../ch3-solution-ideation/SKILL.md)
- [制订策略](../ch4-strategy-formulation/SKILL.md)
- [改善业务](../ch5-business-improvement/SKILL.md)
- [管理组织](../ch6-org-management/SKILL.md)
- [传达与共享](../ch7-communication-sharing/SKILL.md)

---

## 扩展资源

- **30+ 场景组合库**（跨章节套餐推荐）：见 [references/recipes.md](references/recipes.md)
