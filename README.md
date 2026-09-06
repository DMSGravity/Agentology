## Disclaimer, this project is nearly fully agentic-thus the programs name- I've kept the source private cause this is a hobby for me; I needed to talk to my local agent, and the other tools had too much friction for me to deal with. [[LM Studio for Copilot Chat](https://github.com/yoy123/lmstudio-copilot-provider)] worked, but the context window widget didn't work and I thought "I can just use Ai to fix this." little did I know what I was in for. Below is agent text, I've head it read my depo but you know how they go; if you have bugs or anything else, feel free to post them here however, please try to be concise and clear- I cannot just "figure out" bugs and asks like a trained coder can. 
```markdown
# Agentology for VS Code — Feedback & Issue Tracker

Welcome to the public issue tracker and feedback repository for **Agentology for VS Code** (LM Studio integration for VS Code & Copilot Chat).

Use this repository to report bugs, request features, or share feedback.

---

##  Features at a Glance

Agentology is an advanced, high-performance Language Model Provider and Autonomous Agent runtime connecting your local **LM Studio** models directly into VS Code Copilot and the VS Code Agents Window.

###  100% Local & Private
- **Zero Cloud Leakage**: Keep your code, prompts, and tokens entirely on your local machine.
- **No Surprise API Bills**: Closed subagent delegation prevents background tasks from secretly routing to paid cloud APIs (Claude/OpenAI).

###  Deep Tool & MCP Execution
- **Dynamic MCP Discovery**: Automatically discovers and forwards 100% of all registered workspace and MCP tools (including Jupyter notebook execution: `run_notebook_cell`, `execute_cell`, `read_notebook`).
- **Autonomous Multi-Turn Tool Loop**: Use `@agentology` in the Chat View to run autonomous reasoning, terminal commands, file edits, and tool executions in a single session.
- **Surgical Parameter Bridging**: Automatically normalizes open-weight model parameter variations (`file_path` $\to$ `filePath`, `old_string` $\to$ `oldString`).

###  Real-Time Context & Token Synchronization
- **Live VRAM Context Sync**: Dynamically mirrors your loaded LM Studio KV-cache window (up to 262k tokens) to VS Code using a 4-tier source-of-truth hierarchy.
- **Zero-Latency Token Estimator**: Sub-millisecond BPE approximation eliminates socket freezing and connection drops during heavy inference.
- **Automatic Budget Split**: Reserves 25% output headroom to prevent context window overflow truncation.

###  Native Custom Agents & Dynamic Subagents
- **`LocalAgent` Coordinator**: Use the `Local` session target in the Agents Window or Chat view with native delegation to specialized local subagents (`LocalResearcher`, `LocalCoder`, `LocalPlanner`).
- **Pure Dynamic Inheritance**: Automatically inherits whichever model you have loaded in LM Studio without requiring hardcoded configuration.

###  Multimodal & Architecture Support
- **Vision (Image Input)**: Full support for multimodal vision models (e.g. Qwen-VL, Pixtral, LLaVA).
- **Dynamic Model Families**: Automatically detects and maps `qwen`, `llama`, `deepseek`, `mistral`, `gemma`, `phi`, and `gpt-4o` architectures.

---

##  Quick Setup

1. **Start LM Studio**:
   - Open LM Studio and start the Local Server (default: `http://localhost:1234`).
   - Load your preferred model (e.g., Qwen 2.5 Coder 32B, Llama 3.3 70B, DeepSeek-Coder).
2. **Open VS Code**:
   - Install **Agentology for VS Code**.
   - In VS Code Copilot Chat (`Ctrl+Alt+I` / `Cmd+Alt+I`), select your loaded LM Studio model from the model picker.
   - Type `@agentology` to run autonomous tasks with full MCP and workspace tools.

---

##  How to Report Bugs

When opening an issue, please provide:
1. **Operating System**: (Windows / macOS / Linux)
2. **LM Studio Version & Model Name**: (e.g., `LM Studio v0.3.x`, `Qwen/Qwen2.5-Coder-32B-Instruct-GGUF`)
3. **Context Length Configured in LM Studio**: (e.g., `32,768` or `131,072`)
4. **Relevant Output Channel Logs**:
   - Open the **Output** panel in VS Code (`Ctrl+Shift+U` / `Cmd+Shift+U`).
   - Select **"LM Studio"** from the dropdown and paste the relevant log snippet.
5. **Steps to Reproduce**: Detailed description of what prompt or tool caused the issue.

---

## 📜 License
Agentology for VS Code is distributed under the [MIT License](LICENSE).
```

