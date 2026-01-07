# 贡献指南 / Contributing Guidelines

感谢你对 Cybersecurity Expert 的关注！我们欢迎各种形式的贡献。

## 中文

### 如何贡献

1. **Fork 本仓库**
2. **创建特性分支** (`git checkout -b feature/AmazingFeature`)
3. **提交更改** (`git commit -m 'Add some AmazingFeature'`)
4. **推送到分支** (`git push origin feature/AmazingFeature`)
5. **开启 Pull Request**

### 开发指南

#### Skill 结构

```
cybersecurity-expert/
├── skill.md           # 核心 skill 定义文件
├── README.md          # 项目说明文档
├── LICENSE            # MIT 许可证
├── CONTRIBUTING.md    # 贡献指南（本文件）
└── CHANGELOG.md       # 版本更新日志
```

#### 修改 Skill

- 确保 `skill.md` 的 frontmatter 格式正确
- 测试所有修改后的功能
- 更新版本号和 CHANGELOG.md

#### 提交规范

提交信息格式：

```
<type>(<scope>): <subject>

<body>

<footer>
```

**类型 (type):**
- `feat`: 新功能
- `fix`: 修复bug
- `docs`: 文档更新
- `style`: 代码格式
- `refactor`: 重构
- `test`: 测试
- `chore`: 构建/工具

**示例:**
```
feat(detection): add support for detecting obfuscated PowerShell scripts

- Added new pattern recognition for Base64 encoded PowerShell
- Improved detection rate for encoded malicious commands

Closes #123
```

### 代码审查

所有 Pull Request 都需要通过代码审查。请确保：

- [ ] 代码符合项目风格
- [ ] 所有测试通过
- [ ] 文档已更新
- [ ] CHANGELOG.md 已更新

### 行为准则

- 尊重所有贡献者
- 建设性反馈
- 关注问题本身而非个人

---

## English

### How to Contribute

1. **Fork the repository**
2. **Create your feature branch** (`git checkout -b feature/AmazingFeature`)
3. **Commit your changes** (`git commit -m 'Add some AmazingFeature'`)
4. **Push to the branch** (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Development Guidelines

#### Skill Structure

```
cybersecurity-expert/
├── skill.md           # Core skill definition file
├── README.md          # Project documentation
├── LICENSE            # MIT License
├── CONTRIBUTING.md    # Contributing guidelines (this file)
└── CHANGELOG.md       # Version changelog
```

#### Modifying the Skill

- Ensure `skill.md` frontmatter format is correct
- Test all modified functionality
- Update version number and CHANGELOG.md

#### Commit Convention

Commit message format:

```
<type>(<scope>): <subject>

<body>

<footer>
```

**Types:**
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation update
- `style`: Code formatting
- `refactor`: Refactoring
- `test`: Testing
- `chore`: Build/tooling

**Example:**
```
feat(detection): add support for detecting obfuscated PowerShell scripts

- Added new pattern recognition for Base64 encoded PowerShell
- Improved detection rate for encoded malicious commands

Closes #123
```

### Code Review

All Pull Requests require code review. Please ensure:

- [ ] Code follows project style
- [ ] All tests pass
- [ ] Documentation is updated
- [ ] CHANGELOG.md is updated

### Code of Conduct

- Respect all contributors
- Provide constructive feedback
- Focus on issues, not personalities
