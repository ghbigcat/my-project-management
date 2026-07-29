# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.2.0] - 2026-07-29

### Added

- **跨平台支持**：新增 Claude Code、Codex CLI、OpenClaw 三大平台适配
- **AGENTS.md**：Codex CLI 兼容指令文件（<150 行，自动读取）
- **Claude Code Skill**：`.claude/skills/my-project-management/` 目录含适配 frontmatter 的 SKILL.md + references
- **Claude Code Slash 命令**：5 个命令（`/pm-req`、`/pm-risk`、`/pm-progress`、`/pm-resource`、`/pm-meeting`）
- **OpenClaw 适配**：`openclaw/` 目录含 SKILL.md、references、INSTALL.md 安装指南
- **多平台安装指南**：README.md 新增 4 平台安装方式对比表和详细步骤

### Changed

- README.md 标题更新为"跨平台 AI 项目管理技能套件"
- 新增 Claude Code、Codex、OpenClaw 兼容性徽章
- 目录结构更新，展示完整多平台文件布局

## [1.1.0] - 2026-07-27

### Added

- **PMBOK 第八版全量对齐**：6 条原则映射表、7 绩效域覆盖表、5 聚焦领域映射
- **裁剪指南**（`references/tailoring-guide.md`）：3 大裁剪维度 × 5 大能力矩阵 + 快速决策表
- **AI 增强策略**（PMBOK 第八版附录 X3）：Automation / Assistance / Augmentation 三级策略映射
- **可持续发展维度**：各能力新增可持续性影响评估（社会/环境/经济三维度）
- **价值导向**：需求拆解新增价值映射表，进度管家新增价值实现偏差指标（VV/VPI），会议纪要新增价值评审板块
- **相关方参与评估矩阵**：会议纪要大师新增 5 级参与度评估（Unaware → Leading）

### Changed

- PMBOK 对齐表从第六版十大知识领域 → 第八版 7 绩效域
- 阶段命名从"需求阶段/规划阶段/..." → 第八版 Focus Areas 术语（Initiating/Planning/...）
- 风险分类新增"可持续性风险"类别（环境合规/社会责任/资源可持续/ESG 监管）
- 资源优化器新增"建设赋能文化"维度（成长型分配 + 团队赋能度评分）
- 偏差原因分析从 4 维度扩展到 5 维度（新增"价值"维度）

### Updated

- SKILL.md：新增原则映射段落、价值导向声明、裁剪指导段落、AI 三级策略表
- req-decomposer.md：WBS 定义更新为价值导向，新增裁剪指导（预测型/敏捷/看板/混合型差异）
- risk-radar.md：新增 AI 辅助风险识别（模式识别 + 预测分析），新增裁剪指导
- progress-manager.md：新增 EVM 适用性矩阵（敏捷用燃尽图/看板用 CFD），新增裁剪指导
- resource-optimizer.md：新增资源可持续性评估，新增裁剪指导
- meeting-minutes.md：新增价值评审会类型，新增裁剪指导

## [1.0.0] - 2026-07-27

### Added

- 初始版本发布
- 5 大能力套件：需求拆解助手、资源优化器、进度管家、风险雷达、会议纪要大师
- 基于 PMBOK 第六/七版知识体系和过程组
- 统一 Markdown 输出规范（元信息头 + 主体 + 行动项跟踪表）
- 渐进式加载架构（SKILL.md 路由 + 5 个 reference 按需加载）
- 打包为 `.skill` 文件支持 WorkBuddy 直接安装
