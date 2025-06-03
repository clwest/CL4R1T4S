# 🧠 Cursor Prompt Engineering Cheat Sheet

Welcome to the underground vault of Codex/Cursor system prompts. This cheat sheet breaks down the key prompts used by Cursor AI for editing, navigation, memory, testing, and tool usage. Perfect for remixing with Claude 3.7, Replicate, or even VS Code integrations.

---

## ✍️ File Editing Prompt (`edit_file.md`)

**Purpose:** Edit a file based on natural language instructions.

**Key Behaviors:**

- Identifies target lines to change
- Handles multi-line refactors
- Inserts/removes functions, docstrings, or imports

**Use It For:**

- Replacing blocks of logic
- Generating new routes or views
- Renaming vars/functions across large files

```plaintext
“You are editing a code file given a diff-like instruction.”
```

---

## 🔍 Ask About Codebase (`ask_codebase.md`)

**Purpose:** Answer questions about the repo or code structure.

**Key Behaviors:**

- Searches for matching symbols/files
- Summarizes usage across files
- Traces function/variable logic

**Use It For:**

- "Where is `generate_prompt` used?"
- "What does `prompt_placement.py` do?"
- "What’s the model structure for StoryImage?"

```plaintext
“You are answering a question about a codebase...”
```

---

## ⚙️ Tool Executor (`tool_executor.md`)

**Purpose:** Execute dev commands via CLI or API wrappers.

**Key Behaviors:**

- Routes user intent to defined tools
- Returns structured result

**Use It For:**

- Custom shell commands (e.g. lint, migrate, push)
- AI agent orchestration
- File search → edit → commit pipelines

```plaintext
“You are executing a user’s command using available tools...”
```

---

## 🧪 Test Generator (`test_generation.md`)

**Purpose:** Write tests using framework already in use.

**Key Behaviors:**

- Detects test type (unit, integration)
- Adds coverage based on code paths
- Respects Pytest, Unittest, or Jest patterns

**Use It For:**

- Writing tests for views, models, utils
- Snapshot testing for frontend
- Auto-validating new routes after edit

```plaintext
“Write tests for this file using the testing framework in use.”
```

---

## 🧩 Memory + Chunking Prompt (Experimental)

**Purpose:** Auto-summarize and semantically chunk files for long-term memory.

**Key Behaviors:**

- Reads all files in a repo or folder
- Splits into summaries + embeddings
- Routes chunks into prompts as needed

**Use It For:**

- Long-term repo Q&A memory
- Searchable RAG-style assistant
- Claude or GPT agents with memory recall

```plaintext
“Summarize this code file into its core responsibilities...”
```

---

## 🧠 Bonus Prompt Ideas

- `navigation.md`: Jump to file/symbol quickly
- `tools.md`: Defines what tools Codex can access
- `file_explorer.md`: Understand file tree structure
- `codemod.md`: Automate code rewrites across repo

---

## 🔧 Plug-and-Play: Claude + VS Code + Replicate

With these prompts, you can:

- Use Claude 3.7 as a file-aware dev assistant
- Build your own Cursor-style VS Code plugin
- Use Replicate for media + model routing

Let me know if you want a Claude-ready template to start remapping these!

---

> "Cursor isn’t just a tool. It’s a pattern. And now it’s yours to remix."

🚀 Built for Donkey Betz by ChatGPT
