# ai-refactor-demo
这是一个我在日常开发中探索 AI Agent 能力的测试仓库，包含基于 OpenClaw + Claude Code 的代码重构试验。目前已实现巨型组件的自动化拆分和单元测试闭环验证。
# AI Refactor Agent Demo

本项目演示了基于 OpenClaw + Claude Code 实现的代码自动化重构 Agent 原型。

## 架构设计

- 编排层：OpenClaw
- 语义理解层：Claude Code
- 静态分析层：本地 LSP + AST

## 核心流程

1. **审计阶段**：扫描 src 目录，用 AST 识别耦合度高的文件和循环依赖
2. **重构阶段**：子 Agent 协作切分巨型组件，搭配测试闭环验证
3. **文档阶段**：自动生成带调用示例的 README 和 Storybook 文档

## 运行截图

见 /screenshots 目录
