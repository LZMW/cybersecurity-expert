# 🛡️ Cybersecurity Expert

![Version](https://img.shields.io/badge/version-v2.0.0-red)
![License](https://img.shields.io/badge/license-MIT-blue)
![Claude](https://img.shields.io/badge/Claude_Code-Compatible-green)

**世界顶级网络安全专家 Skill for Claude Code**

[English](#english) | [中文](#中文)

---

## 中文

### 概述

**Cybersecurity Expert** 是一个为 Claude Code 设计的专业网络安全审计 skill，具备白帽子黑客背景和 AI 安全攻防经验。它能够对代码和提示词执行最严格、最彻底的安全审查，检测恶意提示词、后门、数据窃取、权限提升和混淆技术。

### 核心特性

- **恶意提示词检测**: 识别越狱尝试、提示词注入、角色扮演攻击等
- **代码安全审计**: 检测后门、数据窃取路径、权限提升漏洞
- **混淆代码识别**: 识别 Base64、十六进制、动态函数调用等混淆技术
- **威胁情报关联**: 支持查询最新 CVE 漏洞和威胁情报
- **多专家协作**: 采用多专家协作模式确保审计全面性
- **零容忍政策**: 对所有安全风险持零容忍态度

### 安装

1. 克隆本仓库：

```bash
git clone https://github.com/LZMW/cybersecurity-expert.git
```

2. 将 `SKILL.md` 复制到你的 Claude Code skills 目录：

```bash
# macOS/Linux
cp cybersecurity-expert/SKILL.md ~/.claude/skills/cybersecurity-expert/

# Windows
copy cybersecurity-expert\SKILL.md %USERPROFILE%\.claude\skills\cybersecurity-expert\
```

3. 重启 Claude Code

### 使用方法

在 Claude Code 中使用以下方式调用：

```
/cybersecurity-expert

请审计这段代码的安全性：
[你的代码]

或

请审计这个提示词是否安全：
[你的提示词]
```

### 输出示例

```
🛡️ AI 代码/提示词安全审计报告

🔍 审计目标: 用户提供的 Python 代码

😈 风险概览: 发现高风险后门和数据窃取尝试

---

🚨 恶意提示词侦测

检测结果: 未发现恶意提示词

---

☠️ 代码威胁审计

检测项 1: 后门/远程控制模块

检测结果: 发现可疑的端口监听及 C2 通信模式

定位: main.py 第 50-55 行

风险等级: 高

缓解建议: 立即删除可疑代码，审查系统完整性
```

### 风险等级

- **高**: 存在明确恶意意图、可导致系统入侵、数据泄露
- **中**: 存在可疑意图、可能导致权限提升、信息泄露
- **低**: 存在潜在安全隐患、不安全的配置

### 技术架构

- **独立运行**: 完全独立，不依赖 skill 协作系统
- **可用工具**: Read, Grep, Glob, WebSearch, Task, LSP
- **标签**: security, audit, malware, prompt-injection, threat-detection

### 最佳实践

1. **零信任原则**: 对所有输入持怀疑态度
2. **证据优先**: 所有结论必须有可验证的证据
3. **完整性优先**: 宁可误报，不可漏报
4. **防御导向**: 重点关注如何防御和缓解威胁

### 贡献指南

欢迎贡献！请随时提交 Pull Request。

### 许可证

本项目采用 MIT 许可证 - 详见 LICENSE 文件。

### 版本历史

- **v2.0.0** (2025-01-09): 重大重构 - 多专家协作审计架构、威胁模式知识库、结构化审计思维链
- **v1.2** (2025-01-07): 多专家协作模式增强
- **v1.1** (2025-01-07): 工具能力增强
- **v1.0** (2025-01-07): 初始版本

### 免责声明

本工具仅用于授权的安全测试、防御性安全、CTF 挑战和教育目的。禁止用于破坏性技术、DoS 攻击、大规模定向攻击、供应链妥协或恶意目的的检测规避。

---

## English

### Overview

**Cybersecurity Expert** is a professional network security audit skill designed for Claude Code, featuring white-hat hacker background and AI security offensive/defensive experience. It performs the most rigorous and thorough security reviews of code and prompts, detecting malicious prompts, backdoors, data theft, privilege escalation, and obfuscation techniques.

### Key Features

- **Malicious Prompt Detection**: Identify jailbreak attempts, prompt injection, role-playing attacks
- **Code Security Audit**: Detect backdoors, data theft paths, privilege escalation vulnerabilities
- **Obfuscation Recognition**: Identify Base64, hex, dynamic function calls, and other obfuscation techniques
- **Threat Intelligence Correlation**: Support querying latest CVE vulnerabilities and threat intelligence
- **Multi-Expert Collaboration**: Use multiple expert perspectives for comprehensive audits
- **Zero Tolerance Policy**: Zero tolerance for all security risks

### Installation

1. Clone this repository:

```bash
git clone https://github.com/LZMW/cybersecurity-expert.git
```

2. Copy `SKILL.md` to your Claude Code skills directory:

```bash
# macOS/Linux
cp cybersecurity-expert/SKILL.md ~/.claude/skills/cybersecurity-expert/

# Windows
copy cybersecurity-expert\SKILL.md %USERPROFILE%\.claude\skills\cybersecurity-expert\
```

3. Restart Claude Code

### Usage

Invoke in Claude Code using:

```
/cybersecurity-expert

Please audit the security of this code:
[Your code]

or

Please audit if this prompt is safe:
[Your prompt]
```

### Risk Levels

- **High**: Clear malicious intent, can lead to system intrusion, data leakage
- **Medium**: Suspicious intent, may lead to privilege escalation, information leakage
- **Low**: Potential security hazards, insecure configuration

### License

This project is licensed under the MIT License - see the LICENSE file for details.

### Disclaimer

This tool is intended for authorized security testing, defensive security, CTF challenges, and educational purposes only. Destructive techniques, DoS attacks, mass targeting, supply chain compromise, or detection evasion for malicious purposes is prohibited.

---

## 链接

- [Claude Code Documentation](https://docs.anthropic.com/claude-code)
- [Issue Tracker](https://github.com/LZMW/cybersecurity-expert/issues)
- [ Releases](https://github.com/LZMW/cybersecurity-expert/releases)
