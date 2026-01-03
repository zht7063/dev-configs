# 配置存储项目

该项目主要用于保存项目开发中的配置文件，提供一个最小化可执行方案，方便正式项目开发。

## 项目结构

```
d:\neo-projs\configs\
├── .cursor/              # Cursor IDE 配置目录
│   ├── rules.md          # Agent 全局规则
│   ├── context/          # 项目上下文信息
│   │   └── project-info.md
│   └── skills/           # 专业领域技能配置
│       ├── agentDevCoder/
│       │   └── SKILL.md
│       ├── deepLearningCoder/
│       │   └── SKILL.md
│       └── gitAgent/
│           └── SKILL.md
├── .vscode/              # VS Code 配置
│   └── settings.json
└── readme.md             # 项目文档
```

## 配置内容介绍

### 目录：`.cursor`

该目录用于存储 Cursor IDE 的配置文件。

#### `rules.md` - Agent 规则提示词

该文件用于存储 Cursor Agent 的系统提示词信息，常用于为 Agent 定义人设、代码风格、基本规则等。

#### `context/` - 项目上下文

该目录用于存储项目相关上下文内容，如项目整体目标、项目结构等信息。

#### `skills/` - 专业技能配置

该目录包含针对不同开发场景的专业技能配置，用于在特定场景下增强 Agent 的能力：

- **agentDevCoder**: 智能体应用开发技能

  - 适用场景：多智能体架构设计、工具调用、RAG、工作流编排
  - 核心能力：工具系统、状态管理、评测与可观测性

- **deepLearningCoder**: 深度学习编程技能

  - 适用场景：PyTorch/Lightning 训练脚本、模型实现、实验复现
  - 核心能力：数据管线、分布式训练、性能优化、调试

- **gitAgent**: Git 提交规范技能
  - 适用场景：编写规范的 Git 提交信息
  - 核心能力：Conventional Commits + Emoji、可追溯性、可检索性

### 目录：`.vscode`

该目录用于存储 VS Code 编辑器的配置文件。

---

# 其他内容

## 关于最高效使用 cursor 不同模型的方案

- 默认模型：Gemini 3 Flash（写大多数代码、做小改动）
- 卡住了再切：GPT-5.1 Codex Max / Composer 1（复杂 bug、跨模块重构）
- 最后兜底：Sonnet 4.5（你明确感觉“需要更强的长链路规划/更稳的 agent 执行”时再上）
