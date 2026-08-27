<p align="center">
  <img src="https://github.com/user-attachments/assets/260ce434-1501-42d1-a944-c75fbffcbf7c" alt="Auralyne" width="180"/>
</p>

<h1>Auralyne</h1>

<p>
  <strong>Local AI. One interface. Full control.</strong>
</p>

<p>
  Run models locally, automatically install models adapted to your system, connect external tools, and deploy advanced AI agents directly on your machine.
</p>

## Download

### Windows

```shell
curl -fsSL https://auralyne.com/install.sh | sh
```

or [download manually](https://github.com/auralyne-systems/auralyne/releases/latest/download/Auralyne-Setup.exe)

# What is Auralyne?

**Auralyne is a local AI platform designed to make running AI models as simple as possible.**

During installation, Auralyne automatically downloads models adapted to the user's machine, making local AI accessible without requiring manual model configuration.

Auralyne is built around local **GGUF inference**, automatic model management, and a unified interface for different types of AI workloads.

```text
                    Auralyne
                       │
          ┌────────────┼────────────┐
          │            │            │
          ▼            ▼            ▼
        Chat         Vision        Voice
          │            │            │
          ▼            ▼            ▼
       Best model   Best model   Best model
          │            │            │
          └────────────┼────────────┘
                       ▼
                  Local Runtime
                       │
                       ▼
                  Your Hardware
```

# Current Features

### Local GGUF inference

Run compatible `.gguf` models directly on your machine.

Auralyne handles the local runtime and exposes the model through a simple desktop interface.

### Automatic model management

Auralyne detects the available hardware and can download models adapted to the system.

The goal is to remove unnecessary complexity from local AI:

```text
Your hardware
      │
      ▼
Hardware detection
      │
      ▼
Model compatibility
      │
      ▼
Automatic model selection
      │
      ▼
Local inference
```

### Local chat

Auralyne currently provides a complete local chat experience with:

- Local model execution
- Model discovery
- Model selection
- Persistent conversations
- Conversation history
- Streaming responses
- Markdown rendering
- Code blocks
- Local inference

# Backend

Auralyne uses a native architecture designed around local inference and system-level integration.

### Core technologies

- **Rust** — Native backend and system integration
- **llama.cpp** — Local LLM inference
- **GGUF** — Model format
- **Tauri** — Desktop application framework
- **TypeScript** — Application logic
- **React** — User interface
- **Vite** — Frontend tooling

The architecture separates the user interface from the local inference and system layers:

```text
                    Auralyne
                       │
                ┌──────┴──────┐
                │   React UI  │
                │ TypeScript  │
                └──────┬──────┘
                       │
                ┌──────┴──────┐
                │    Tauri    │
                └──────┬──────┘
                       │
                ┌──────┴──────┐
                │    Rust     │
                │   Backend   │
                └──────┬──────┘
                       │
                ┌──────┴──────┐
                │  llama.cpp  │
                └──────┬──────┘
                       │
                       ▼
                  GGUF Models
                       │
                       ▼
                  Your Hardware
```

# Coming Soon

Auralyne is actively under development.

The platform is being expanded from local chat into a complete local AI environment.

### Vision

Auralyne will support vision-capable models and automatically select an appropriate model when an image-based task requires one.

### Voice

Local voice interaction is planned, including speech recognition and voice-based interaction with local models.

### MCP

Auralyne will support **Model Context Protocol (MCP)** connections.

This will allow models to access external tools through a standardized interface.

```text
Auralyne
    │
    ▼
Local Model
    │
    ▼
MCP
    │
    ├── Tools
    ├── Services
    └── External systems
```

### API connections

Auralyne will support connections to external APIs, allowing local models to interact with external services when required.

### Advanced local agents

Auralyne is being developed toward an advanced local agent system capable of interacting directly with the user's machine.

Agents will be designed to work with:

- Local files
- Applications
- Commands
- External tools
- MCP servers
- APIs
- Multi-step tasks
- Automated workflows

The long-term objective is to turn Auralyne into a **local AI agent runtime**, not simply a chat application.

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
  ├── Automatic model selection
  ├── Vision
  ├── Voice
  ├── MCP
  └── API connections
       │
       ▼
Future
  │
  └── Advanced local agents
       │
       ├── Files
       ├── Applications
       ├── Commands
       ├── Tools
       ├── APIs
       └── Automation
```

# Philosophy

**Local.**

Run AI directly on your hardware whenever possible.

**Simple.**

Local AI should not require users to understand inference runtimes, quantization, or model configuration.

**Powerful.**

Advanced users should be able to connect models, tools, APIs, MCP servers, and agents.

# Status

> 🚧 Auralyne is currently in active development.

Features described in the roadmap are under development and may change as the platform evolves.
