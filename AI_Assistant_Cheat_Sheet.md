# 🧠 Ultimate AI Prompt & Tool Cheat Sheet

### 📁 Local Prompt Vault Index  
A quick-reference index for all system prompts and tools you've collected for use with various AI assistant setups. Use this to stay organized and optimize your development environment.

---

## 🧑‍💻 Codex / Cursor Prompts
- **Filename:** `Cursor_Prompt.md`
- **Focus:** Full-featured agentic coding assistant prompt for pair programming, task planning, tool use, memory creation, safe command execution.
- **Notable Features:**
  - Workspace + file awareness
  - Tool schema for safe, modular command calls
  - Persistent memory
  - Strict "no surprise edits" communication style

### 🔧 Cursor Tools
- **Filename:** `Cursor_Tools.md`
- **Description:** Massive JSON block defining tool capabilities like `grep_search`, `run_command`, `view_file`, `browser_preview`, and more.
- **Power Use:** Designed for safe, modular codebase interaction within VSCode.

---

## 🌬️ Windsurf (Cascade / Codeium)
- **Prompt:** `Windsurf_Prompt.md`
- **Tools:** `Windsurf_Tools.md`
- **Focus:** Cascade (formerly Windsurf), a dev-focused AI with autonomous code editing, terminal use, and memory.
- **Best For:** Agentic pair programming in web-heavy or CLI-based workflows.

---

## 🤖 Claude 3.5 Sonnet
- **Prompt Location:** `Claude_Prompt.md` *(Pending Upload)*
- **Focus:** Lightweight, fast, great for reasoning-heavy tasks and intermediate development workflows.
- **Use Case:** Real-time code reviews, assistant-style chat, and context-rich Q&A.

---

## 🧠 Mistral / LeChat
- **Prompt:** `LeChat.md`
- **Focus:** French-style assistant derived from Mistral models.
- **Vibe:** Friendly, informal, precise.
- **Use Case:** Frontend help, creative projects, or when you want a casual dev partner.

---

## 🧰 Tips for Using These Prompts
1. 🔁 **Always back up** your prompt collection in your project folder under `/system-prompts/`.
2. 🧠 **Stick to one assistant** per workspace for consistent behavior.
3. ⚡ **Test compatibility** with different tools—e.g., Claude with `curl`, Windsurf in Cursor, Codex with `run_command`.

---