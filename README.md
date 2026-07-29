# 我的项目管理 — 跨平台 AI 项目管理技能套件

> 基于 **PMBOK Guide 第八版（2024）** 的 AI 项目管理技能套件，覆盖项目全生命周期的五大能力。
> 以**价值交付**为核心，以**非规定性裁剪**为方法论，以 **AI 三级增强**为执行策略。

[![PMBOK](https://img.shields.io/badge/PMBOK-8th%20Edition-blue)](https://www.pmi.org/standards/pmbok)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![WorkBuddy](https://img.shields.io/badge/WorkBuddy-Skill-orange)](https://www.codebuddy.ai)
[![Claude Code](https://img.shields.io/badge/Claude%20Code-compatible-purple)](https://claude.com)
[![Codex](https://img.shields.io/badge/Codex-AGENTS.md-black)](https://developers.openai.com/codex)
[![OpenClaw](https://img.shields.io/badge/OpenClaw-compatible-red)](https://openclaw.ai)

---

## 目录

- [功能特性](#功能特性)
- [PMBOK 第八版对齐](#pmbok-第八版对齐)
- [安装方式](#安装方式)
  - [WorkBuddy](#方式一workbuddy-推荐)
  - [Claude Code](#方式二claude-code)
  - [Codex CLI](#方式三codex-cli)
  - [OpenClaw](#方式四openclaw)
- [使用方法](#使用方法)
- [能力总览](#能力总览)
- [目录结构](#目录结构)
- [裁剪指南](#裁剪指南)
- [AI 增强策略](#ai-增强策略)
- [版本历史](#版本历史)
- [贡献指南](#贡献指南)
- [许可证](#许可证)

---

## 功能特性

| # | 能力 | 核心方法 | 项目阶段 |
|---|------|----------|----------|
| 1 | **需求拆解助手** | WBS 100% 原则 + INVEST 验证 + MoSCoW 优先级 + 价值映射 | Initiating |
| 2 | **资源优化器** | 技能匹配度计算 + 负载均衡系数 + 赋能文化建设 + 可持续资源评估 | Planning |
| 3 | **进度管家** | EVM 挣值管理（SV/CV/SPI/CPI/EAC）+ 价值实现偏差（VV/VPI）+ 根因分析 | Executing |
| 4 | **风险雷达** | 概率-影响矩阵 + 5 种应对策略 + 可持续性风险 + AI 辅助识别 | Monitoring |
| 5 | **会议纪要大师** | 7 种会议类型 + 5W 行动项 + 价值评审 + 相关方参与评估矩阵 | Closing |

### 核心亮点

- **PMBOK 第八版全对齐**：6 条原则 + 7 绩效域 + 5 聚焦领域 + 裁剪 + AI 增强 + 可持续发展
- **渐进式加载**：SKILL.md 仅含路由逻辑，6 个 reference 文件按需加载，不占上下文
- **统一 Markdown 输出**：所有能力输出结构化 Markdown，含元信息头、价值检查、行动项跟踪
- **裁剪意识内置**：执行任何能力前自动判断项目类型（预测型/适应型/混合型），调整执行方式
- **零依赖即装即用**：纯 Markdown 内容，不依赖任何脚本、API 密钥或外部服务

---

## PMBOK 第八版对齐

### 6 条原则映射

| # | 原则 | 英文 | 体现 |
|---|------|------|------|
| 1 | 采用全局视角 | Adopt a Holistic Approach | 需求拆解时考虑范围/进度/成本/风险/资源的相互影响 |
| 2 | 聚焦价值 | Focus on Value | 所有能力输出均含"价值实现检查" |
| 3 | 将质量融入过程和交付物 | Embed Quality into Process and Deliverables | 验收标准前置，偏差分析含质量维度 |
| 4 | 成为负责任的领导者 | Be an Accountable Leader | 行动项明确单一负责人，风险应对明确责任人 |
| 5 | 在所有项目领域融入可持续发展 | Integrate Sustainability in All Project Areas | 各能力含可持续性影响评估（社会/环境/经济） |
| 6 | 建设赋能文化 | Build an Empowered Culture | 资源优化含能力建设维度，会议纪要含团队反馈闭环 |

### 7 绩效域覆盖

| 绩效域 | 对应能力 |
|--------|---------|
| Governance（治理） | 会议纪要大师 |
| Scope（范围） | 需求拆解助手 |
| Schedule（进度） | 进度管家 |
| Finance（财务） | 进度管家 |
| Stakeholders（相关方） | 会议纪要大师 |
| Resources（资源） | 资源优化器 |
| Risk（风险） | 风险雷达 |

---

## 安装方式

本技能套件支持 4 大平台，一次下载，多平台使用。

### 平台兼容性总览

| 平台 | 安装方式 | 格式 | 位置 |
|------|----------|------|------|
| **WorkBuddy** | .skill 导入 / 手动复制 | SKILL.md + references/ | `~/.workbuddy/skills/` |
| **Claude Code** | 复制 .claude/ 目录 | .claude/skills/ + .claude/commands/ | 项目根目录或 `~/.claude/` |
| **Codex CLI** | AGENTS.md 自动读取 | AGENTS.md | 仓库根目录或 `~/.codex/` |
| **OpenClaw** | ClawHub CLI / 手动复制 | SKILL.md + references/ | `~/.openclaw/skills/` |

---

### 方式一：WorkBuddy（推荐）

#### A. 直接安装 .skill 文件

1. 下载本仓库中的 `my-project-management.skill` 文件
2. 在 WorkBuddy 中打开 Skill 管理页面
3. 导入 `.skill` 文件，系统会自动触发安全审计
4. 审计通过后即可使用

#### B. 手动安装（从源码）

```bash
git clone https://github.com/ghbigcat/my-project-management.git
mkdir -p ~/.workbuddy/skills/my-project-management
cp my-project-management/SKILL.md ~/.workbuddy/skills/my-project-management/
cp -r my-project-management/references/ ~/.workbuddy/skills/my-project-management/
```

重启 WorkBuddy，skill 自动加载。

---

### 方式二：Claude Code

Claude Code 支持两种方式：Skill 自动激活 + Slash 命令手动调用。

#### A. 安装 Skill（自动激活）

```bash
git clone https://github.com/ghbigcat/my-project-management.git

# 项目级安装（团队共享）
cp -r my-project-management/.claude/ .claude/

# 或全局安装（个人使用）
cp -r my-project-management/.claude/skills/ ~/.claude/skills/
```

安装后 Claude Code 在检测到项目管理相关请求时自动激活 skill。

#### B. Slash 命令（手动调用）

本仓库提供 5 个 slash 命令，复制 `.claude/commands/` 到项目后可用：

| 命令 | 功能 | 示例 |
|------|------|------|
| `/pm-req` | 拆解需求为 WBS | `/pm-req PSP患者服务项目` |
| `/pm-risk` | 评估项目风险 | `/pm-risk 患者服务项目` |
| `/pm-progress` | 跟踪进度与偏差 | `/pm-progress 项目周报数据` |
| `/pm-resource` | 优化资源分配 | `/pm-resource 团队5人` |
| `/pm-meeting` | 生成会议纪要 | `/pm-meeting 站会记录` |

---

### 方式三：Codex CLI

Codex 自动读取仓库根目录的 `AGENTS.md` 文件。

#### A. 项目级安装

```bash
git clone https://github.com/ghbigcat/my-project-management.git
cd my-project-management
# Codex 启动时自动读取 ./AGENTS.md
codex "帮我拆解需求"
```

#### B. 全局安装

```bash
cp my-project-management/AGENTS.md ~/.codex/AGENTS.md
cp -r my-project-management/references/ ~/.codex/references/
# 所有项目中 Codex 自动加载
```

> Codex 的 AGENTS.md 限制 32KB，本文件已控制在限制内。支持嵌套覆盖：子目录可放置额外 AGENTS.override.md。

---

### 方式四：OpenClaw

详见 [`openclaw/INSTALL.md`](openclaw/INSTALL.md)。

```bash
# ClawHub CLI 安装
npx clawhub@latest install my-project-management

# 或手动安装
git clone https://github.com/ghbigcat/my-project-management.git
mkdir -p ~/.openclaw/skills/my-project-management
cp my-project-management/openclaw/SKILL.md ~/.openclaw/skills/my-project-management/
cp -r my-project-management/openclaw/references/ ~/.openclaw/skills/my-project-management/
openclaw restart
```

可配合本地 LLM（Ollama + Llama 3.1）使用，详见安装指南。

---

### 安装验证

安装后在对话中输入以下任一触发词，若 skill 被激活则安装成功：

| 触发词 | 预期能力 |
|--------|---------|
| "帮我拆解需求" | 需求拆解助手 |
| "评估项目风险" | 风险雷达 |
| "跟踪进度" | 进度管家 |
| "分配任务" | 资源优化器 |
| "记录会议" | 会议纪要大师 |

---

## 使用方法

### 基本用法

在 AI 对话中直接说出需求，skill 会根据意图自动路由到对应能力（Claude Code 也可用 slash 命令手动触发）：

```
用户：帮我拆解 PSP 患者服务项目的需求
→ 触发"需求拆解助手"，读取 req-decomposer.md 执行

用户：评估这个项目的风险
→ 触发"风险雷达"，读取 risk-radar.md 执行

用户：这个月的进度偏差是多少
→ 触发"进度管家"，读取 progress-manager.md 执行
```

### 多能力组合

```
用户：拆解需求并分配任务给团队
→ 先执行"需求拆解助手"，再执行"资源优化器"
```

### 裁剪提示

若未说明项目类型，skill 会主动询问：

```
Skill：请确认项目类型（预测型/适应型/混合型），以便调整执行方式。
用户：混合型
→ 参考 tailoring-guide.md 调整 WBS 深度、进度跟踪方式、风险审查频率
```

### 输出格式

所有能力统一输出 Markdown 文件到工作目录：

```
{能力简称}_{项目名}_{YYYYMMDD}.md

示例：req-decomposer_PSP患者服务_20260727.md
```

每个输出文件包含：
1. 元信息头（项目名称、日期、能力名称、项目类型）
2. 主体内容（按能力模板结构）
3. 价值实现检查
4. 可持续性影响评估（可选）
5. 行动项跟踪表

---

## 能力总览

| 聚焦领域 | 能力 | 触发词 | Reference 文件 |
|----------|------|--------|---------------|
| Initiating | 需求拆解助手 | "拆解需求"、"分析需求"、"WBS" | `references/req-decomposer.md` |
| Planning | 资源优化器 | "分配任务"、"优化资源"、"负载均衡" | `references/resource-optimizer.md` |
| Executing | 进度管家 | "跟踪进度"、"进度监控"、"进度偏差" | `references/progress-manager.md` |
| Monitoring & Controlling | 风险雷达 | "评估风险"、"风险预警"、"风险矩阵" | `references/risk-radar.md` |
| Closing | 会议纪要大师 | "记录会议"、"生成纪要"、"会议总结" | `references/meeting-minutes.md` |
| 全周期 | 裁剪指南 | "裁剪"、"适配"、"定制方法" | `references/tailoring-guide.md` |

---

## 目录结构

```
my-project-management-git/
├── README.md                              # 本文件（多平台安装指南）
├── LICENSE                                 # MIT 许可证
├── .gitignore
├── CHANGELOG.md                            # 版本历史
├── AGENTS.md                               # Codex CLI 指令文件
├── my-project-management.skill            # WorkBuddy 打包文件
├── SKILL.md                                # WorkBuddy 主文件（路由+规范+PMBOK对齐）
├── references/                             # WorkBuddy 能力文件
│   ├── req-decomposer.md                   # 需求拆解助手
│   ├── risk-radar.md                       # 风险雷达
│   ├── progress-manager.md                 # 进度管家
│   ├── resource-optimizer.md               # 资源优化器
│   ├── meeting-minutes.md                  # 会议纪要大师
│   └── tailoring-guide.md                  # 裁剪指南
├── .claude/                                # Claude Code 格式
│   ├── skills/my-project-management/       # Skill（自动激活）
│   │   ├── SKILL.md
│   │   └── references/
│   └── commands/                           # Slash 命令（手动触发）
│       ├── pm-req.md                       # /pm-req
│       ├── pm-risk.md                      # /pm-risk
│       ├── pm-progress.md                  # /pm-progress
│       ├── pm-resource.md                  # /pm-resource
│       └── pm-meeting.md                   # /pm-meeting
└── openclaw/                               # OpenClaw 格式
    ├── INSTALL.md                          # 安装指南
    ├── SKILL.md
    └── references/
```

---

## 裁剪指南

PMBOK 第八版强调"非规定性"——过程和实践应根据项目特征裁剪。本 skill 内置裁剪意识，支持以下维度：

| 裁剪维度 | 选项 | 影响 |
|----------|------|------|
| 开发方法 | 预测型 / 适应型（敏捷/看板） / 混合型 | WBS 分解深度、进度跟踪方式、风险审查频率 |
| 项目规模 | 小型 / 中型 / 大型 / 超大型 | 流程正式程度、文档详细度、治理层级 |
| 行业 | 通用 / 医疗健康 / IT / 制造 / 金融 | 合规要求、风险类别、质量标准 |
| 团队分布 | 同地 / 分布式 / 全远程 | 沟通频率、会议类型、工具选择 |

详见 `references/tailoring-guide.md`。

---

## AI 增强策略

基于 PMBOK 第八版附录 X3，本 skill 按三级策略增强项目管理实践：

| 策略层级 | 定义 | 应用 |
|----------|------|------|
| **Automation（自动化）** | 替代人工执行重复性任务 | 会议纪要自动结构化、EVM 指标自动计算、风险矩阵自动生成 |
| **Assistance（辅助）** | 辅助人工完成复杂任务 | WBS 拆解建议、风险识别清单生成、资源匹配度计算 |
| **Augmentation（增强）** | 增强人类决策能力 | 偏差根因分析、风险趋势预测、资源优化方案对比 |

---

## 版本历史

详见 [CHANGELOG.md](CHANGELOG.md)。

| 版本 | 日期 | 主要变更 |
|------|------|----------|
| 1.2.0 | 2026-07-29 | 跨平台支持：新增 Claude Code、Codex CLI、OpenClaw 适配 |
| 1.1.0 | 2026-07-27 | PMBOK 第八版全量更新（6 原则 + 7 绩效域 + 裁剪 + AI 增强 + 可持续发展） |
| 1.0.0 | 2026-07-27 | 初始版本，基于 PMBOK 第六/七版，5 大能力套件 |

---

## 贡献指南

欢迎提交 Issue 和 Pull Request。

### 贡献方向

- 新增行业裁剪模板（医疗/IT/制造/金融/教育）
- 补充 PMBOK 第八版其他附录内容
- 各能力的模板优化和边界用例
- 多语言支持（英文版 reference 文件）

### 提交规范

1. Fork 本仓库
2. 创建特性分支：`git checkout -b feature/your-feature`
3. 提交变更：`git commit -m 'feat: add your feature'`
4. 推送分支：`git push origin feature/your-feature`
5. 提交 Pull Request

---

## 许可证

[MIT License](LICENSE) — 自由使用、修改、分发。

---

> **参考标准**：PMI, *A Guide to the Project Management Body of Knowledge (PMBOK Guide) — Eighth Edition*, Project Management Institute, 2024.
