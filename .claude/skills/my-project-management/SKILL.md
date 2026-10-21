---
description: "AI 项目管理技能套件 — 基于 PMBOK 第八版，覆盖需求拆解、风险评估、进度管控、资源优化、会议纪要、绩效度量、过程观测七大能力。当用户需要拆解需求(WBS)、评估风险、跟踪进度、优化资源分配、生成会议纪要、设计指标与 EVM 绩效评估、或监控项目状态并触发预警时自动激活。"
---

# 我的项目管理

> 基于 PMBOK Guide 第八版（2024），以**价值交付**为核心，覆盖项目全生命周期。

## 能力路由

根据用户意图选择对应能力，读取相应 reference 文件后执行：

| 触发关键词 | 能力 | Reference 文件 |
|------------|------|----------------|
| 拆解/分析需求/WBS | 需求拆解助手 | references/req-decomposer.md |
| 分配/优化资源/负载 | 资源优化器 | references/resource-optimizer.md |
| 进度/跟踪/偏差/延期 | 进度管家 | references/progress-manager.md |
| 风险/预警/应对/矩阵 | 风险雷达 | references/risk-radar.md |
| 绩效/度量/KPI/指标定义/挣值/EVM/验收/测试用例 | 绩效度量器 | references/evaluation.md |
| 监控/状态报告/偏差预警/告警/观测/趋势 | 过程观测器 | references/observability.md |
| 会议/纪要/记录会议 | 会议纪要大师 | references/meeting-minutes.md |
| 裁剪/适配/定制方法 | 裁剪指南 | references/tailoring-guide.md |

多能力请求按聚焦领域顺序（Initiating → Planning → Executing → Monitoring → Closing）依次执行。

## 边界：升级到项目群

以下信号属**项目群层级**，应转交 `my-programme-management` 技能（依据 GB/T 41246-2022 / ISO 21503）：

| 信号 | 判据 |
|------|------|
| 项目群 / programme / 多项目统筹 | 41246 §3.1 |
| 收益管理 / 收益登记册 / 收益实现 | 41246 §6.6 |
| 组件依赖 / 组件接口 / 跨项目资源冲突 | 41246 §6.3、§6.5 |
| 项目群治理 / 决策关口 / 治理主体 | 41245 §7 |

不转交：单个项目内部的 WBS、EVM、单项目风险、单项目纪要。

**绩效度量器与过程观测器的分工**：前者回答"这一期做得够不够好"（周期性、结论导向）；后者回答"现在有没有偏离，要不要报警"（持续性、预警导向）。二者共用同一套指标定义卡口径，不得各自定义。

**触发词歧义消解**：单独出现"评估"时按宾语判定 —— 评估**风险** → 风险雷达；评估**绩效/验收** → 绩效度量器；评估**状态/趋势** → 过程观测器。

## 统一输出规范

所有能力输出 Markdown 文件，命名：`{能力简称}_{项目名}_{YYYYMMDD}.md`

每个输出含：元信息头 → 主体内容 → 价值实现检查 → 可持续性影响评估（可选）→ 行动项跟踪表

行动项表必须含单一负责人，不可填"团队"或"全员"。

## PMBOK 第八版 6 条原则

1. 采用全局视角（Adopt a Holistic Approach）
2. 聚焦价值（Focus on Value）
3. 将质量融入过程和交付物（Embed Quality into Process and Deliverables）
4. 成为负责任的领导者（Be an Accountable Leader）
5. 在所有项目领域融入可持续发展（Integrate Sustainability in All Project Areas）
6. 建设赋能文化（Build an Empowered Culture）

## 裁剪意识

执行任何能力前判断项目类型（预测型/适应型/混合型），参考 references/tailoring-guide.md 调整执行方式。
