# Cybersecurity Expert 快速启动指南

本指南帮助你在 5 分钟内完成 GitHub 发布。

---

## 📋 发布前检查

- [ ] 已安装 Git
- [ ] 已有 GitHub 账号
- [ ] 已准备好发布的项目副本

---

## 🚀 5 分钟发布步骤

### Step 1: 配置 Git (1 分钟)

```bash
# 替换为你的信息
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

### Step 2: 创建 GitHub 仓库 (1 分钟)

1. 访问 https://github.com/new
2. 填写：
   - Repository name: `cybersecurity-expert`
   - Description: `🛡️ World-class cybersecurity audit skill for Claude Code`
   - 选择 **Public**
   - License: **MIT License**
3. 点击 **Create repository**
4. 复制你的仓库 URL: `https://github.com/YOUR_USERNAME/cybersecurity-expert.git`

### Step 3: 推送代码 (2 分钟)

```bash
# 进入项目目录
cd "E:\智能体\github-publish\cybersecurity-expert"

# 初始化仓库
git init

# 添加所有文件
git add .

# 创建提交
git commit -m "Initial release: Cybersecurity Expert v1.2.0"

# 添加远程仓库（替换 YOUR_USERNAME）
git remote add origin https://github.com/YOUR_USERNAME/cybersecurity-expert.git

# 推送到 GitHub
git branch -M main
git push -u origin main
```

**如果推送时需要认证：**
1. 用户名：输入你的 GitHub 用户名
2. 密码：输入 Personal Access Token（不是 GitHub 密码）

**创建 Personal Access Token：**
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. "Generate new token (classic)"
3. 勾选 `repo` 权限
4. 生成并复制 token

### Step 4: 创建 GitHub Release (1 分钟)

1. 在仓库页面点击 **Releases** → **Create a new release**
2. 填写：
   - Tag version: `v1.2.0`
   - Target: `main`
   - Release title: `🛡️ Cybersecurity Expert v1.2.0`
   - Description: 复制以下内容

```markdown
## 首次发布

我们很高兴宣布 Cybersecurity Expert 首次发布！

## 核心特性

- 🔍 恶意提示词检测 - 识别越狱、注入、角色扮演攻击
- 🛡️ 代码安全审计 - 检测后门、数据窃取、权限提升
- 🔐 混淆代码识别 - Base64、十六进制、动态调用
- 🌐 威胁情报关联 - CVE 漏洞查询、恶意软件签名
- 🤖 智能体协作 - 支持复杂代码库的深度审计
- ⚠️ 零容忍政策 - 对所有安全风险严格审查

## 安装

```bash
git clone https://github.com/YOUR_USERNAME/cybersecurity-expert.git
cp cybersecurity-expert/skill.md ~/.claude/skills/cybersecurity-expert/
```

## 快速开始

在 Claude Code 中：
```
请审计这段代码的安全性：[你的代码]
```

## 许可证

MIT License

## 免责声明

仅用于授权安全测试、防御性安全、CTF 挑战和教育目的。
```

3. 勾选 **Set as the latest release**
4. 点击 **Publish release**

---

## 🎉 完成！

你的项目已成功发布到 GitHub！

---

## 📊 下一步

### 可选：配置仓库

1. **设置 Topics**：在仓库页面右侧添加以下 topics
   - `cybersecurity`
   - `security-audit`
   - `claude-code`
   - `ai-security`

2. **设置描述**：在 About 中填写
   ```
   🛡️ World-class cybersecurity audit skill for Claude Code
   ```

### 可选：社交媒体推广

参考 `docs/SOCIAL_MEDIA.md` 获取现成的推广文案。

---

## 🆘 常见问题

### Q: 推送时提示 "Permission denied"

**A:** 检查以下几点：
1. 确认仓库名称正确
2. 使用 Personal Access Token 作为密码
3. 确认你有仓库的写入权限

### Q: 如何创建 Personal Access Token？

**A:**
1. GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. "Generate new token (classic)"
3. 勾选 `repo` 权限
4. 生成并复制 token
5. 推送时用 token 作为密码

### Q: 如何更新 README 中的链接？

**A:** 使用查找替换功能，将所有 `YOUR_USERNAME` 替换为你的实际 GitHub 用户名。

---

## 📁 项目结构

```
cybersecurity-expert/
├── .github/
│   ├── ISSUE_TEMPLATE/      # Issue 模板
│   └── PULL_REQUEST_TEMPLATE.md  # PR 模板
├── docs/
│   ├── PUBLISHING_GUIDE.md  # 完整发布指南
│   ├── RELEASE_NOTES.md     # 发布素材
│   └── SOCIAL_MEDIA.md      # 社交媒体文案
├── skill.md                 # 核心 skill 文件
├── README.md                # 项目说明
├── LICENSE                  # MIT 许可证
├── CHANGELOG.md             # 变更日志
├── CONTRIBUTING.md          # 贡献指南
└── .gitignore               # Git 忽略规则
```

---

## 🔗 有用链接

- **GitHub 文档**: https://docs.github.com
- **Git 官方文档**: https://git-scm.com/doc
- **Markdown 指南**: https://guides.github.com/features/mastering-markdown/

---

**祝你发布顺利！** 🎉

如有问题，请参考 `docs/PUBLISHING_GUIDE.md` 获取详细指导。
