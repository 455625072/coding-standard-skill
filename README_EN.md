# AI Development Standards

This project is a set of universal development standards tailored for AI assistants (Agents), aimed at improving code quality, unifying communication languages, and standardizing Git commit behaviors. We have created 15 specific Agent Skills by combining 5 mainstream AI tools with 3 operating systems (Windows, macOS, Linux).

## Core Principles

1.  **Language & Communication**: Mandatory use of **Chinese** for technical analysis, implementation planning, and code explanation (as per user preference for learning Chinese).
2.  **Environment Adaptation**: Native command support for different operating systems (e.g., PowerShell for Windows, Shell for macOS/Linux) and path standards.
3.  **Development "8 Honors & 8 Shames"**: A strict coding philosophy emphasizing reuse, verification, honesty, and caution.
4.  **Detailed Comments**: Strict requirement for transparent code logic, forbidding "unreadable" code.
5.  **Git Commit Standards**: Structured Commit format to ensure clear and traceable version history.

## Available Skill Matrix

You can find the corresponding `SKILL.md` in the folder matching your tool and environment.

| AI Tool | Windows | macOS | Linux |
| :--- | :--- | :--- | :--- |
| **Anti Gravity** | [Skill](antigravity-windows/SKILL.md) | [Skill](antigravity-mac/SKILL.md) | [Skill](antigravity-linux/SKILL.md) |
| **Codex** | [Skill](codex-windows/SKILL.md) | [Skill](codex-mac/SKILL.md) | [Skill](codex-linux/SKILL.md) |
| **Claude Code** | [Skill](claudecode-windows/SKILL.md) | [Skill](claudecode-mac/SKILL.md) | [Skill](claudecode-linux/SKILL.md) |
| **Cursor** | [Skill](cursor-windows/SKILL.md) | [Skill](cursor-mac/SKILL.md) | [Skill](cursor-linux/SKILL.md) |
| **VSCode** | [Skill](vscode-windows/SKILL.md) | [Skill](vscode-mac/SKILL.md) | [Skill](vscode-linux/SKILL.md) |

## Installation & Usage

### 1. Clone the Repository
```bash
git clone https://github.com/455625072/coding-standard-skill.git
```

### 2. Install the Skill
Choose the corresponding Skill folder based on your tool and environment and install it:

#### A. Direct Copy (Recommended)
Copy the target Skill folder (e.g., `antigravity-windows`) directly into your AI tool's skills directory.
- **Antigravity**: `%APPDATA%\.gemini\antigravity\skills\`
- **Codex**: Check the tool's `SKILLS_PATH` environment variable or documentation.

#### B. Create a Symbolic Link (Recommended for Developers)
If you want to keep the repository code updated, use a symbolic link:
- **Windows (PowerShell/Cmd - Admin Mode required)**:
  ```powershell
  # Example: Link a skill from this repo to the Antigravity directory
  mklink /D "%APPDATA%\.gemini\antigravity\skills\my-skill" "D:\path\to\coding-standard-skill\antigravity-windows"
  ```
- **macOS/Linux**:
  ```bash
  ln -s /path/to/coding-standard-skill/cursor-mac ~/.cursor/skills/my-skill
  ```

### 3. Load & Verify
Restart your AI assistant or execute a "Refresh Skills" command. The AI will automatically load and strictly follow the development standards.

---
[中文版 (Chinese Version)](README.md)
