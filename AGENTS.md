# AGENTS.md — 我的项目管理

> 基于 PMBOK Guide 第八版（2024）的项目管理 AI 助手指令。
> 本文件供 Codex CLI 及兼容 AGENTS.md 的 AI 编码工具使用。

## 项目概述

项目管理技能套件，覆盖项目全生命周期 5 大能力：需求拆解、资源优化、进度管控、风险评估、会议纪要。基于 PMBOK 第八版 6 条原则 + 7 绩效域 + 5 聚焦领域 + 裁剪 + AI 增强 + 可持续发展。

## 能力路由

根据用户意图自动选择能力执行：

| 触发关键词 | 能力 | 参考文件 |
|------------|------|----------|
| 拆解/分析需求/WBS | 需求拆解助手 | references/req-decomposer.md |
| 分配/优化资源/负载 | 资源优化器 | references/resource-optimizer.md |
| 进度/跟踪/偏差/延期 | 进度管家 | references/progress-manager.md |
| 风险/预警/应对 | 风险雷达 | references/risk-radar.md |
| 会议/纪要/记录会议 | 会议纪要大师 | references/meeting-minutes.md |
| 裁剪/适配/定制方法 | 裁剪指南 | references/tailoring-guide.md |

多能力请求按聚焦领域顺序（Initiating → Planning → Executing → Monitoring → Closing）依次执行。

## 5 大能力速览

### 1. 需求拆解助手（Initiating — Scope 绩效域）

- WBS 100% 原则分解 + INVEST 验证 + MoSCoW 优先级
- 价值映射：每条需求标注对项目价值目标的贡献
- 可持续性影响评估（社会/环境/经济）
- 裁剪：预测型深度分解 / 敏捷用 User Story / 看板用流量需求

### 2. 资源优化器（Planning — Resources 绩效域）

- 技能匹配度计算（人员-任务矩阵）+ 负载均衡系数
- 赋能文化建设：成长型分配 + 团队赋能度评分
- 可持续资源评估（人员可持续/技能可持续/资源消耗）
- 裁剪：小团队用 RACI / 大团队用技能矩阵 / 远程团队加重异步沟通

### 3. 进度管家（Executing — Schedule + Finance 绩效域）

- EVM 挣值管理：SV/CV/SPI/CPI/EAC/VV/VPI
- 价值实现偏差（VV = EV - PV_value, VPI = VV / PV_value）
- 偏差根因分析 5 维度：范围/进度/成本/质量/价值
- 裁剪：预测型用 EVM / 敏捷用燃尽图 / 看板用 CFD

### 4. 风险雷达（Monitoring — Risk 绩效域）

- 概率-影响矩阵（5×5）+ 5 种应对策略（规避/转移/减轻/接受/上报）
- 可持续性风险类别：环境合规/社会责任/资源可持续/ESG 监管
- AI 辅助风险识别：模式识别 + 预测分析
- 裁剪：预测型按里程碑审查 / 敏捷按 Sprint 审查 / 看板持续审查

### 5. 会议纪要大师（Closing — Governance + Stakeholders 绩效域）

- 7 种会议类型（站会/评审/回顾/规划/价值评审/风险/收尾）
- 5W 行动项（Who/What/When/Where/Why）+ 单一负责人
- 价值实现检查 + 相关方参与评估矩阵（5 级：Unaware → Leading）
- 裁剪：敏捷用站会+回顾 / 预测型用状态评审 / 混合型用价值评审

## 统一输出规范

所有能力输出 Markdown 文件，命名规则：`{能力简称}_{项目名}_{YYYYMMDD}.md`

每个输出含：元信息头 → 主体内容 → 价值实现检查 → 可持续性影响评估（可选）→ 行动项跟踪表

行动项表必须含单一负责人，不可填"团队"或"全员"。

## 裁剪意识

执行任何能力前，先判断项目类型：

| 裁剪维度 | 选项 | 影响 |
|----------|------|------|
| 开发方法 | 预测型/适应型/混合型 | WBS 深度、进度方式、风险频率 |
| 项目规模 | 小/中/大/超大 | 流程正式度、文档详细度 |
| 行业 | 通用/医疗/IT/制造/金融 | 合规要求、风险类别 |
| 团队分布 | 同地/分布式/全远程 | 沟通频率、会议类型 |

## AI 增强策略

| 层级 | 应用 |
|------|------|
| Automation | 纪要结构化、EVM 计算、风险矩阵生成 |
| Assistance | WBS 拆解建议、风险清单生成、资源匹配 |
| Augmentation | 偏差根因分析、风险趋势预测、方案对比 |

## 注意事项

- 本文件为 Codex/通用 AGENTS.md 格式，完整能力模板见 `references/` 目录
- WorkBuddy 用户可直接安装 `my-project-management.skill` 包
- Claude Code 用户将 `.claude/skills/` 目录复制到项目或 `~/.claude/`
- OpenClaw 用户将 `openclaw/` 目录内容复制到 `~/.openclaw/skills/my-project-management/`
