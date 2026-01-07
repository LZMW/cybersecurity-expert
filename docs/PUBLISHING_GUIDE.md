# Cybersecurity Expert GitHub 发布完整指南

本指南将一步步引导你完成 GitHub 发布全过程。

---

## 第一步：准备工作

### 1.1 检查 Git 安装

```bash
git --version
```

如果未安装，请从 [git-scm.com](https://git-scm.com/) 下载安装。

### 1.2 配置 Git 用户信息

```bash
# 配置你的用户名（替换为你的 GitHub 用户名）
git config --global user.name "Your Name"

# 配置你的邮箱（替换为你的 GitHub 邮箱）
git config --global user.email "your.email@example.com"
```

### 1.3 准备 GitHub 账号

如果还没有 GitHub 账号：
1. 访问 [github.com](https://github.com)
2. 点击 "Sign up" 注册
3. 验证邮箱

---

## 第二步：创建 GitHub 仓库

### 2.1 在 GitHub 创建新仓库

1. 登录 GitHub
2. 点击右上角 "+" → "New repository"
3. 填写仓库信息：
   - **Repository name**: `cybersecurity-expert`
   - **Description**: `🛡️ World-class cybersecurity audit skill for Claude Code`
   - **Public** ☑️（选择公开）
   - **不要**勾选 "Add a README file"（我们已经有了）
   - **不要**勾选 "Add .gitignore"
   - **License**: 选择 "MIT License"

4. 点击 "Create repository"

### 2.2 记录仓库 URL

创建后 GitHub 会显示你的仓库 URL：
- HTTPS: `https://github.com/YOUR_USERNAME/cybersecurity-expert.git`
- SSH: `git@github.com:YOUR_USERNAME/cybersecurity-expert.git`

---

## 第三步：推送代码到 GitHub

### 3.1 进入项目目录

```bash
cd "E:\智能体\github-publish\cybersecurity-expert"
```

### 3.2 初始化 Git 仓库（如果还没初始化）

```bash
git init
```

### 3.3 添加所有文件

```bash
git add .
```

### 3.4 创建初始提交

```bash
git commit -m "Initial release: Cybersecurity Expert v1.2.0

🛡️ World-class cybersecurity audit skill for Claude Code

Features:
- Malicious prompt detection
- Code security audit
- Obfuscation recognition
- Threat intelligence correlation
- Agent collaboration
- Zero-tolerance security policy

License: MIT"
```

### 3.5 添加远程仓库

**使用 HTTPS（推荐，更简单）：**
```bash
git remote add origin https://github.com/YOUR_USERNAME/cybersecurity-expert.git
```

**使用 SSH（需要配置 SSH 密钥）：**
```bash
git remote add origin git@github.com:YOUR_USERNAME/cybersecurity-expert.git
```

### 3.6 推送到 GitHub

```bash
# 推送到 main 分支
git branch -M main
git push -u origin main
```

**如果使用 HTTPS**，GitHub 会提示输入用户名和密码（或 Personal Access Token）。

**如果使用 SSH**，确保已配置 SSH 密钥。

---

## 第四步：创建 GitHub Release

### 4.1 进入 Releases 页面

1. 在 GitHub 仓库页面
2. 点击右上角 "Releases"
3. 点击 "Create a new release"

### 4.2 填写 Release 信息

**Tag version**: `v1.2.0`

**Target**: `main`

**Release title**:
```
🛡️ Cybersecurity Expert v1.2.0
```

**Description**:
```markdown
## 首次发布 / First Release

我们很高兴宣布 Cybersecurity Expert 首次发布！这是一个为 Claude Code 设计的专业网络安全审计 skill。

## 核心特性 / Key Features

- 🔍 **恶意提示词检测** - 识别越狱、注入、角色扮演攻击
- 🛡️ **代码安全审计** - 检测后门、数据窃取、权限提升
- 🔐 **混淆代码识别** - Base64、十六进制、动态调用
- 🌐 **威胁情报关联** - CVE 漏洞查询、恶意软件签名
- 🤖 **智能体协作** - 支持复杂代码库的深度审计
- ⚠️ **零容忍政策** - 对所有安全风险严格审查

## 安装 / Installation

```bash
git clone https://github.com/YOUR_USERNAME/cybersecurity-expert.git
cp cybersecurity-expert/skill.md ~/.claude/skills/cybersecurity-expert/
```

## 快速开始 / Quick Start

在 Claude Code 中：
```
请审计这段代码的安全性：[你的代码]
```

## 文档 / Documentation

- [完整文档](https://github.com/YOUR_USERNAME/cybersecurity-expert#readme)
- [贡献指南](https://github.com/YOUR_USERNAME/cybersecurity-expert/blob/main/CONTRIBUTING.md)
- [变更日志](https://github.com/YOUR_USERNAME/cybersecurity-expert/blob/main/CHANGELOG.md)

## 许可证 / License

MIT License

## 免责声明 / Disclaimer

仅用于授权安全测试、防御性安全、CTF 挑战和教育目的。
```

### 4.3 发布

- 勾选 "Set as the latest release"
- 点击 "Publish release"

---

## 第五步：配置仓库

### 5.1 设置仓库 Topics

1. 在仓库页面，点击右侧 "About" 下的齿轮图标
2. 添加以下 Topics：
   - `cybersecurity`
   - `security-audit`
   - `claude-code`
   - `ai-security`
   - `prompt-injection`
   - `malware-detection`
   - `threat-intelligence`
   - `security-tools`

### 5.2 设置仓库描述

在 About 中填写：
```
🛡️ World-class cybersecurity audit skill for Claude Code. Detect malicious prompts, backdoors, data theft, privilege escalation, and obfuscation techniques with zero-tolerance policy.
```

### 5.3 添加网站链接（如果有）

- Website:（你的个人网站或项目文档站点）
- Documentation: `https://github.com/YOUR_USERNAME/cybersecurity-expert/blob/main/docs/RELEASE_NOTES.md`

---

## 第六步：社交媒体推广

### 6.1 Twitter/X

发布素材位于：`docs/RELEASE_NOTES.md`

### 6.2 LinkedIn

发布素材位于：`docs/RELEASE_NOTES.md`

### 6.3 Reddit

推荐发布到：
- r/programming
- r/cybersecurity
- r/ArtificialIntelligence
- r/MachineLearning

### 6.4 技术社区

- V2EX: https://www.v2ex.com/go/opensource
- 掘金: 发布标签选择 "开源"
- SegmentFault: 发布到开源板块

---

## 第七步：提交到目录和聚合站

### 7.1 Awesome Lists

搜索相关的 awesome lists 并提交 PR：
- Awesome AI Security
- Awesome Claude
- Awesome Cybersecurity

### 7.2 Product Hunt

如果想在 Product Hunt 发布，需要：
1. 准备产品页面
2. 准备发布当天的推广计划
3. 联系社区支持

### 7.3 Hacker News

选择合适的发布时间（美国东部时间上午 9-11 点）

---

## 第八步：持续维护

### 8.1 监控 Issues

定期查看和回复 GitHub Issues

### 8.2 审查 Pull Requests

及时审查社区贡献的代码

### 8.3 发布新版本

当有重要更新时：
1. 更新 `CHANGELOG.md`
2. 更新 `skill.md` 中的版本号
3. 创建新的 git tag
4. 创建新的 GitHub Release

---

## 常见问题

### Q1: 推送时提示 "Permission denied"

**A:** 检查以下几点：
1. 确认仓库名称正确
2. 确认你有推送权限
3. 如果使用 HTTPS，可能需要 Personal Access Token

### Q2: 如何创建 Personal Access Token？

**A:**
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. "Generate new token (classic)"
3. 勾选 `repo` 权限
4. 生成并复制 token
5. 推送时用 token 作为密码

### Q3: 如何配置 SSH 密钥？

**A:**
```bash
# 生成 SSH 密钥
ssh-keygen -t ed25519 -C "your.email@example.com"

# 复制公钥
cat ~/.ssh/id_ed25519.pub

# 添加到 GitHub：
# GitHub → Settings → SSH and GPG keys → New SSH key
# 粘贴公钥

# 测试连接
ssh -T git@github.com
```

### Q4: 如何更新 README.md 中的链接？

**A:** 使用查找替换功能，将 `YOUR_USERNAME` 替换为你的实际 GitHub 用户名。

---

## 发布清单

完成以下检查后，即可正式发布：

- [ ] Git 已安装并配置
- [ ] GitHub 账号已创建
- [ ] GitHub 仓库已创建
- [ ] README.md 中的链接已更新
- [ ] Git 仓库已初始化
- [ ] 初始提交已创建
- [ ] 远程仓库已添加
- [ ] 代码已推送到 GitHub
- [ ] GitHub Release 已创建
- [ ] 仓库 Topics 已设置
- [ ] 仓库描述已填写
- [ ] 社交媒体文案已发布
- [ ] 相关目录已提交

---

## 需要帮助？

如果在发布过程中遇到问题：

1. 查看 [GitHub 文档](https://docs.github.com)
2. 搜索类似问题的解决方案
3. 在 GitHub Issues 中提问

---

**祝发布顺利！** 🎉

---

## 附录：项目文件结构

```
cybersecurity-expert/
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── PULL_REQUEST_TEMPLATE.md
├── docs/
│   └── RELEASE_NOTES.md          # 发布素材
├── skill.md                       # 核心 skill 文件
├── README.md                      # 项目说明
├── LICENSE                        # MIT 许可证
├── CHANGELOG.md                   # 变更日志
├── CONTRIBUTING.md                # 贡献指南
├── .gitignore                     # Git 忽略规则
└── PUBLISHING_GUIDE.md            # 本发布指南
```
