---
title: 开发配置存储项目 (dev-configs)
description: 结构化的项目信息说明，旨在辅助 AI Agent 理解本项目作为开发配置模板库的角色。
---

## 1. 项目背景 (Project Context)

- **核心目标**: 该项目主要用于保存项目开发中的配置文件（如 Cursor 规则、技能、IDE 配置等），提供一个最小化可执行方案，方便正式项目开发。
- **业务场景**: 作为新项目的启动模板或现有项目的配置参考。
- **当前状态**: 持续更新中。

## 2. 技术栈 (Tech Stack)

- **核心工具**: [Cursor IDE](https://cursor.com/)
- **配置格式**: Markdown (.md), JSON (.json)
- **领域专注**: AI Agent 开发、深度学习、Git 规范。

## 3. 项目架构与目录结构 (Architecture & Directory Structure)

- **`.cursor/`**: Cursor IDE 核心配置目录。
  - **`rules.md`**: 定义 Agent 的全局人设与代码风格。
  - **`context/`**: 存储项目上下文信息（如本文件）。
  - **`skills/`**: 场景化的 Agent 技能增强（智能体开发、深度学习、Git 提交）。
- **`.vscode/`**: 编辑器通用配置。

## 4. 开发规范 (Development Standards)

- **编码风格**: 配置文件遵循简洁、易读的 Markdown 规范。
- **技能配置**: 每个技能目录包含 `SKILL.md`，详细说明适用场景与核心能力。
- **Git 工作流**: 遵循 Conventional Commits + Emoji 规范（由 `gitAgent` 技能支持）。

## 5. 核心业务领域 (Domain Knowledge)

- **Agent Skill**: 指针对特定任务（如 RAG 系统开发）对 AI Agent 进行的能力增强配置。
- **Context Management**: 如何通过结构化文档（如本文件）提升 AI Agent 对项目的理解深度。

## 6. 开发与使用 (Getting Started)

- **环境要求**: 安装最新版本的 Cursor IDE。
- **使用方法**: 直接复制 `.cursor` 目录到新项目中，或参考其中的规则与技能配置。

## 7. 备忘录与未来规划 (Notes & Roadmap)

- **已知限制**: 当前系统存在的问题或待优化点。
- **短期规划**: 完善更多开发场景的 Skill 配置（如 Frontend Essentials, Backend Security）。
- **长期愿景**: 成为一套开箱即用的、高度智能化的 AI 协同开发配置标准。
