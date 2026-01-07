# 变更日志 / Changelog

本文件记录了 Cybersecurity Expert skill 的所有重要变更。

格式基于 [Keep a Changelog](https://keepachangelog.com/zh-CN/1.0.0/)，
版本号遵循 [语义化版本](https://semver.org/lang/zh-CN/)。

## [Unreleased]

### 计划中
- 支持更多编程语言的特定模式检测
- 增强对抗性样本检测能力
- 添加更多威胁情报数据源

## [1.2.0] - 2025-01-07

### 新增
- 新增 `Task` 工具支持，可调用 general-purpose 智能体
- 新增 `Explore` 智能体支持，快速探索代码库结构
- 新增 `AgentOutputTool` 获取智能体分析结果
- 添加智能体使用指南和组合示例
- 添加多步骤复杂审计工作流示例

### 改进
- 优化了大型代码库的审计流程
- 增强了跨文件关联分析能力

### 文档
- 更新了工具使用说明
- 添加了智能体协作最佳实践

## [1.1.0] - 2025-01-07

### 新增
- 新增 `WebSearch` 工具用于威胁情报查询
- 添加 CVE 漏洞查询能力
- 添加已知恶意软件签名搜索
- 添加可疑域名/IP信誉查询

### 改进
- 增强了威胁情报关联分析
- 优化了检测报告格式

### 文档
- 添加了详细的工具使用指南
- 明确了工具使用原则和禁止事项
- 添加了工具组合使用示例

## [1.0.0] - 2025-01-07

### 新增
- 初始版本发布
- 恶意提示词检测能力
- 代码安全审计功能
- 后门/远程控制检测
- 数据窃取路径识别
- 权限提升漏洞分析
- 代码混淆技术识别
- 依赖链安全审查
- 风险等级评估（高/中/低）
- 完整的安全审计报告输出

### 特性
- 完全独立运行，不依赖 skill 协作系统
- 零容忍安全政策
- 支持中英文双语输出
- 专业的取证导向分析报告

---

## 版本说明

### 版本号格式
- **主版本号**：不兼容的 API 修改
- **次版本号**：向下兼容的功能新增
- **修订号**：向下兼容的问题修正

### 风险等级说明
- **高风险 (High)**：存在明确恶意意图，可直接导致系统被入侵
- **中风险 (Medium)**：存在可疑意图，可能导致权限提升或信息泄露
- **低风险 (Low)**：存在潜在安全隐患，不直接导致安全事件

---

## [Unreleased]: https://github.com/YOUR_USERNAME/cybersecurity-expert/compare/v1.2.0...HEAD
## [1.2.0]: https://github.com/YOUR_USERNAME/cybersecurity-expert/compare/v1.1.0...v1.2.0
## [1.1.0]: https://github.com/YOUR_USERNAME/cybersecurity-expert/compare/v1.0.0...v1.1.0
## [1.0.0]: https://github.com/YOUR_USERNAME/cybersecurity-expert/releases/tag/v1.0.0
