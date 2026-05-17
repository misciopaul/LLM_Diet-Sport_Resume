# 🛠 Technical Setup Guide

This guide explains how to technically configure your AI assistant to manage the Diet & Sport Wiki.

## 1. Prerequisites
- **Obsidian:** Installed on your computer.
- **AI Assistant:** An assistant with file system access (e.g., **Gemini CLI**, **ChatGPT with Canvas/Advanced Data Analysis** - though Gemini CLI is recommended for its native integration).
- **Git (Optional):** To keep the repository updated.

## 2. Vault Initialization
1.  **Download the Repository:** Clone or download this project.
2.  **Open as Vault:** Open the folder in Obsidian.
3.  **Language Preference:** When you first start your assistant, it will ask for your language. It will then translate the core files to match your choice.

## 3. Configuring Gemini CLI
If you are using Gemini CLI, ensure the `GEMINI.md` file is present in the root. The CLI reads this file automatically as a "System Prompt" to understand the rules of your Wiki.

### Automated Workflow
The assistant follows these rules:
- **Weekly Logs:** Created automatically in `Diet/` and `Sport/`.
- **Calculations:** Done automatically using your `profile.md`.
- **Monthly Reports:** Proactively suggested at the start of each month.

## 4. Manual Configuration (Other LLMs)
If you are not using an automated CLI:
1. Copy the content of `GEMINI.md`.
2. Paste it as a "System Instructions" or "Custom Instructions" in your preferred LLM interface.
3. Manually upload your `profile.md` when you need accurate calculations.

---
*Ready to start? Ask your assistant: "How can I set up my profile?"*
