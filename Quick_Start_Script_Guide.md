# 🚀 Quick Start Script Guide

To make using Gemini CLI with your Wiki even faster, you can create a shortcut script.

## For Linux/macOS (`start_wiki.sh`)
1. Create a file named `start_wiki.sh` in the root.
2. Paste the following:
   ```bash
   #!/bin/bash
   # Navigate to the Wiki directory
   cd "/path/to/your/LLM_Diet-Sport_Resume"
   # Start Gemini CLI in interactive mode
   gemini chat
   ```
3. Make it executable: `chmod +x start_wiki.sh`.

## For Windows (`start_wiki.bat`)
1. Create a file named `start_wiki.bat`.
2. Paste the following:
   ```batch
   @echo off
   cd "C:\path\to\your\LLM_Diet-Sport_Resume"
   gemini chat
   ```

## Why use a script?
- **Automatic Context:** The assistant will immediately "see" your `GEMINI.md` and your data logs.
- **Speed:** No need to navigate the file system every time.
