# Agentology for VS Code

> High-performance, LM Studio provider & autonomous agent runtime for VS Code and Copilot Chat.

[![GitHub Discussions](https://img.shields.io/badge/Community-Discussions-green.svg)](https://github.com/DMSGravity/Agentology/discussions)

---

## 📖 About Agentology

**Agentology for VS Code** bridges your local [LM Studio](https://lmstudio.ai/) models directly into VS Code Copilot Chat. 

Built specifically for developers who want a seamless, air-gapped, zero-cost coding assistant, Agentology provides native multi-turn tool execution, full Model Context Protocol (MCP) tool forwarding, dynamic contexta budgeting, and closed local subagent orchestration.

---

## ✨ Key Capabilities

- ⚡ **Full MCP & Workspace Forwarding**: Discovers and runs 100% of registered workspace and MCP tools.
- 🧠 **Live Context Sync**: Dynamically reports your loaded LM Studio KV-cache window to VS Code via a 4-tier source-of-truth hierarchy with low-latency BPE token estimation (`chars / 3.65`).
- 🤖 **Closed Subagent Delegation**: Native `LocalAgent` custom coordinator with pure dynamic model inheritance, strictly preventing background tasks from escaping to paid cloud APIs.
- 👁️ **Multimodal Vision & Multi-Family**: Out-of-the-box support for vision models (`imageInput: isVision`) and dynamic architecture detection (`qwen`, `llama`, `deepseek`, `mistral`, `gemma`, `phi`, `gpt-4o`).

---

## 💬 Discussions & Bug Reports

This repository serves as the official community feedback hub, discussion forum, and issue tracker for Agentology:

- **Ask Questions & Share Setups**: Join our [GitHub Discussions](https://github.com/DMSGravity/Agentology/discussions) to share recommended model quants, GPU settings, and workflows.
- **Report Bugs**: If you encounter an issue with tool calls or model compatibility, please [open an Issue](https://github.com/DMSGravity/Agentology/issues) with your OS, LM Studio model name, and relevant VS Code output channel logs.

---

## 📜 Acknowledgements & Upstream Attribution

Agentology originated as a hard fork of the open-source MIT-licensed project [LM Studio for Copilot Chat](https://github.com/yoy123/lmstudio-copilot-provider) by `@yoy123`.

While the codebase has been substantially refactored and re-engineered with an autonomous multi-turn MCP runtime, custom subagent architecture, and dynamic VRAM context synchronization, we gratefully acknowledge and preserve the foundational contributions of the original project under the terms of the MIT License.

---

## 📄 License

Agentology for VS Code is licensed under the [Proprietary License](LICENSE, see LICENSE file and Notice for details).
