---
name: my-project-management
description: >-
  AI 项目管理技能套件，覆盖项目全生命周期的七大能力：需求拆解、风险评估、进度管控、资源优化、会议纪要、绩效度量、过程观测。
  当用户需要以下操作时触发：(1) 拆解模糊需求为可执行任务清单（"帮我拆解需求"、"分析需求"、"WBS"）；
  (2) 评估项目风险并生成应对策略（"评估项目风险"、"风险预警"、"风险矩阵"）；
  (3) 跟踪项目进度并分析偏差（"跟踪进度"、"进度监控"、"进度偏差"）；
  (4) 优化人员任务分配与负载均衡（"分配任务"、"优化资源"、"负载均衡"）；
  (5) 将会议录音/文字/笔记转为结构化纪要（"记录会议"、"生成纪要"、"会议总结"）；
  (6) 设计指标体系、计算 EVM/挣值、出具绩效评估与验收结论（"评估项目绩效"、"KPI 设计"、"指标定义"、"挣值"、"EVM"、"验收标准"、"测试用例"）；
  (7) 持续监控项目运行状态、判定偏差级别并触发预警、生成分层状态报告（"监控项目"、"状态报告"、"偏差预警"、"告警"、"观测"）。
  基于 PMBOK 第八版（6 条原则 + 7 绩效域 + 5 聚焦领域 + 裁剪 + AI 增强 + 可持续发展）。
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

## AI 增强策略

| 策略层级 | 应用 |
|----------|------|
| Automation | 纪要结构化、EVM 计算、风险矩阵生成 |
| Assistance | WBS 拆解建议、风险清单生成、资源匹配 |
| Augmentation | 偏差根因分析、风险趋势预测、方案对比 |
