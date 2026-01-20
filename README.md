# Gemini-CLI-in-WSL
Your Automated Assistant: Gemini-CLI in WSL
Step-by-step Guide:
**Install WSL:** Ensure Windows Subsystem for Linux is installed on your Windows machine. You can do this by running `wsl --install` in PowerShell (as Administrator).
**Choose a Linux Distribution:** Install your preferred Linux distribution (e.g., Ubuntu) from the Microsoft Store or via `wsl --install -d `.
**Update & Upgrade:** Once in your WSL terminal, update and upgrade your packages: `sudo apt update && sudo apt upgrade`.
**Install Node.js (if not present):** `gemini-cli` is often a Node.js application. Install Node Version Manager (nvm) and then Node.js:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
source ~/.bashrc
nvm install node
**Install Gemini CLI:** Install the `gemini-cli` globally:
npm install -g gemini-cli
**Configure Gemini CLI (API Key):** Follow the `gemini-cli` setup instructions to configure your API key. This typically involves running `gemini configure` or setting an environment variable.
**Start Using:** You can now interact with `gemini-cli` directly from your WSL terminal! For example, `gemini "Explain cron jobs"` or `gemini -y "$(cat my-prompt.txt)"` for automated tasks.
