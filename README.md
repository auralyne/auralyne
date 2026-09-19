<p align="center">
  <img src="https://github.com/user-attachments/assets/260ce434-1501-42d1-a944-c75fbffcbf7c" alt="Auralyne" width="240"/>
</p>

<h1>Auralyne</h1>

<p>
  <strong>Local AI. Autonomous coding. Full control.</strong>
</p>

<p>
  Build, modify, run, and debug software using autonomous AI agents running entirely on your machine.
</p>

## Download

### Windows

```shell
not yet available
```

or [download manually (not yet available)](https://github.com/auralyne-systems/auralyne/releases/latest/download/Auralyne-Setup.exe)

# What is Auralyne?

**Auralyne is a local autonomous vibe coding environment designed to let AI directly work on software projects.**

Auralyne combines local LLM inference, project context, development tools, and autonomous agent execution in a single desktop application.

Instead of only generating code, Auralyne is designed to understand a project, modify it, execute commands, analyze results, and iterate until a task is completed.

The core coding workflow runs locally using **llama.cpp** and local **GGUF** models.

# Current Features

### Local GGUF inference

Run compatible `.gguf` models directly on your machine using **llama.cpp**.

Auralyne manages the local inference runtime and provides the model layer required by the coding agent.


### Local chat

Auralyne currently provides a local AI interface with:

- Local model execution
- Model discovery
- Model selection
- Persistent conversations
- Conversation history
- Streaming responses
- Markdown rendering
- Code blocks
- Local inference


### Project-aware development

Auralyne is being built around direct interaction with software projects.

The agent can work with:

- Project files
- Source code
- Directories
- Project configuration
- Local development environments


### Autonomous coding

The coding agent is designed to execute multi-step development tasks.

This includes:

- Reading and creating files
- Modifying existing code
- Running commands
- Inspecting command output
- Analyzing errors
- Applying fixes
- Iterating on tasks


# Backend

Auralyne uses a native architecture designed around local inference, autonomous agents, and system-level integration.

### Core technologies

- **Rust** — Native backend and system integration
- **llama.cpp** — Local LLM inference
- **GGUF** — Model format
- **Tauri** — Desktop application framework
- **TypeScript** — Application logic
- **React** — User interface
- **Vite** — Frontend tooling
- **MCP** — Tool and context integration

The architecture separates the user interface from the agent, local inference, and system layers:

```text
React / Tauri
      │
      ▼
 Agent Runtime
      │
 ┌────┴───────────────┐
 ▼                    ▼
llama.cpp          Local Tools
 ▼                    │
GGUF Models       Files / Shell / MCP
```

# Coming Soon

Auralyne is actively under development.

The platform is being expanded into a complete local autonomous coding environment.

### Vision

Auralyne will support local vision-capable models for tasks such as screenshot analysis, visual debugging, and image-based development workflows.

### Voice

Local voice interaction is planned, including speech recognition and voice-based interaction with the coding agent.

### MCP

Auralyne will support **Model Context Protocol (MCP)** connections.

This will allow agents to access additional tools and services through a standardized interface.


### Advanced local agents

Auralyne is being developed toward an autonomous local agent system capable of interacting directly with the user's development environment.

Agents will be designed to work with:

- Local files
- Applications
- Commands
- Development tools
- MCP servers
- APIs
- Git repositories
- Multi-step tasks
- Automated workflows

The objective is to provide a **complete local vibe coding environment**, rather than a traditional AI chat application.

# Roadmap

```text
Current
  │
  ├── GGUF inference
  ├── Local chat
  ├── Model discovery
  ├── Hardware detection
  ├── Model management
  └── Streaming responses
       │
       ▼
Next
  │
  ├── Project-aware agents
  ├── File operations
  ├── Shell execution
  ├── Autonomous coding
  ├── Error analysis
  ├── MCP
  └── Git integration
       │
       ▼
Future
  │
  ├── Vision
  ├── Voice
  ├── Advanced agent memory
  ├── Multi-step autonomous workflows
  └── Extended local tool ecosystem
```

# Philosophy

**Local.**

Run AI directly on the user's hardware whenever possible.

**Autonomous.**

AI should be able to execute complete development tasks rather than only generate code.

**Private.**

Source code, project context, and agent execution should remain local by default.

**Simple.**

Local AI coding should not require users to manually manage complex inference configuration.

**Powerful.**

Advanced users should be able to control models, tools, runtimes, MCP servers, and agent behavior.

# Status

> 🚧 Auralyne is currently in active development.

Auralyne is transitioning from a local AI interface into a **complete autonomous local vibe coding environment**.

Features described in the roadmap are under development and may change as the platform evolves.
