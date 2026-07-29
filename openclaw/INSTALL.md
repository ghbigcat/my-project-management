# OpenClaw 安装指南

## 方式一：ClawHub CLI 安装（推荐）

```bash
# 如果已安装 ClawHub
npx clawhub@latest install my-project-management

# 或通过 OpenClaw CLI
openclaw skills add my-project-management
```

## 方式二：手动安装

1. 下载本仓库的 `openclaw/` 目录
2. 将 `SKILL.md` 和 `references/` 复制到 OpenClaw skills 目录：

```bash
# 全局安装（所有项目可用）
mkdir -p ~/.openclaw/skills/my-project-management
cp openclaw/SKILL.md ~/.openclaw/skills/my-project-management/
cp -r openclaw/references/ ~/.openclaw/skills/my-project-management/

# 工作区安装（仅当前项目）
mkdir -p ./skills/my-project-management
cp openclaw/SKILL.md ./skills/my-project-management/
cp -r openclaw/references/ ./skills/my-project-management/
```

3. 重启 OpenClaw 网关使 skill 生效：

```bash
openclaw restart
```

## 安装验证

安装后在 OpenClaw 对话中输入触发词，若 skill 被激活则安装成功：

- "帮我拆解需求" → 需求拆解助手
- "评估项目风险" → 风险雷达
- "跟踪进度" → 进度管家
- "分配任务" → 资源优化器
- "记录会议" → 会议纪要大师

## 技能优先级

OpenClaw skill 优先级：工作区 > 本地 > 内置

- 工作区：`./skills/my-project-management/`
- 本地（全局）：`~/.openclaw/skills/my-project-management/`
- 内置：OpenClaw 自带技能

## 配置本地 LLM

本 skill 可配合本地 LLM 使用（如 Ollama + Llama 3.1）：

```json
{
  "llm": {
    "provider": "ollama",
    "model": "llama3.1:8b",
    "baseUrl": "http://localhost:11434"
  }
}
```

> 注意：本地小型模型（<8B 参数）在复杂项目管理任务上可能能力有限，建议使用 13B+ 模型或云模型获得最佳效果。
