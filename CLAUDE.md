# Agent Reach

给 AI Agent 一键装上互联网能力的工具。

## 项目结构

```
Agent-Reach/
├── agent_reach/     # Python主包 (不能改为src/)
│   ├── channels/    # 渠道模块 (twitter, youtube, bilibili, github等)
│   ├── guides/      # 各平台配置指南
│   ├── integrations/# MCP集成
│   ├── cli.py       # CLI入口
│   ├── config.py    # 配置管理
│   ├── core.py      # 核心逻辑
│   └── doctor.py    # 状态检查
├── skills/          # 技能定义 (SKILL.md)
├── memory/          # 持久化记忆
├── config/         # 配置文件
├── docs/           # 文档
├── tests/          # 测试
└── pyproject.toml
```

## 重要说明

- Python包名必须是 `agent_reach`，这是 pyproject.toml 中定义的
- 不要将 `agent_reach/` 重命名为 `src/`，否则会破坏包导入

## 常用命令

- `agent-reach install --env=auto` - 自动安装
- `agent-reach doctor` - 检查状态
- `agent-reach configure twitter-cookies "..."` - 配置Twitter

## 开发

- Python 3.10+
- 使用 pytest 进行测试
