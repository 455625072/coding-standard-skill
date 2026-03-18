# AI 开发通用规范 (AI Development Standards)

本项目是一套为 AI 助手（Agent）量身定制的通用开发规范，旨在提升代码质量、统一沟通语言并规范 Git 提交行为。我们针对主流的 5 种 AI 工具和 3 种操作系统（Windows, macOS, Linux）进行了排列组合，提供了总计 15 个针对性的 Agent Skill。

## 核心准则

1.  **语言与沟通**：强制要求使用**中文**进行技术分析、方案制定和代码解释。
2.  **环境适配**：针对不同操作系统提供原生指令支持（如 Windows 的 PowerShell 与 macOS/Linux 的 Shell）及路径规范。
3.  **开发“八荣八耻”**：一套严苛的编码哲学，强调复用、验证、诚实与谨慎。
4.  **详尽注释**：要求代码逻辑透明，严禁产出“天书”代码。
5.  **Git 提交规范**：严格的结构化 Commit 格式，确保版本历史清晰可追溯。

## 可用 Skill 矩阵

你可以根据当前使用的工具和环境，在相应的文件夹中找到对应的 `SKILL.md`。

| 开发工具 | Windows | macOS | Linux |
| :--- | :--- | :--- | :--- |
| **Anti Gravity** | [Skill](antigravity-windows/SKILL.md) | [Skill](antigravity-mac/SKILL.md) | [Skill](antigravity-linux/SKILL.md) |
| **Codex** | [Skill](codex-windows/SKILL.md) | [Skill](codex-mac/SKILL.md) | [Skill](codex-linux/SKILL.md) |
| **Claude Code** | [Skill](claudecode-windows/SKILL.md) | [Skill](claudecode-mac/SKILL.md) | [Skill](claudecode-linux/SKILL.md) |
| **Cursor** | [Skill](cursor-windows/SKILL.md) | [Skill](cursor-mac/SKILL.md) | [Skill](cursor-linux/SKILL.md) |
| **VSCode** | [Skill](vscode-windows/SKILL.md) | [Skill](vscode-mac/SKILL.md) | [Skill](vscode-linux/SKILL.md) |

## 安装与使用 (Installation & Usage)

### 1. 克隆仓库
```bash
git clone https://github.com/455625072/coding-standard-skill.git
```

### 2. 安装 Skill
根据您的工具和环境，选择对应的 Skill 文件夹并安装：

#### A. 直接拷贝 (推荐)
将目标 Skill 文件夹（例如 `antigravity-windows`）直接拷贝到您 AI 工具的技能目录中。
- **Antigravity**: `%APPDATA%\.gemini\antigravity\skills\`
- **Codex**: 查阅对应工具的 `SKILLS_PATH` 环境变量或文档。

#### B. 创建符号链接 (开发者推荐)
如果您希望保持仓库代码更新，可以使用符号链接：
- **Windows (PowerShell/Cmd - 需要管理员模式)**:
  ```powershell
  # 示例：将本项目中的 skill 链接到 Antigravity 目录
  mklink /D "%APPDATA%\.gemini\antigravity\skills\my-skill" "D:\path\to\coding-standard-skill\antigravity-windows"
  ```
- **macOS/Linux**:
  ```bash
  ln -s /path/to/coding-standard-skill/cursor-mac ~/.cursor/skills/my-skill
  ```

### 3. 加载与验证
重启您的 AI 助手或执行“刷新技能”指令，AI 将自动加载并严格遵循其中的开发规范。

---
[English Version (英文版)](README_EN.md)
