<p align="center">
  <img src="https://github.com/user-attachments/assets/260ce434-1501-42d1-a944-c75fbffcbf7c" alt="Auralyne" width="240"/>
</p>

<h1>Auralyne</h1>

<p>
  <strong>Local AI. Autonomous embedded coding. Full control.</strong>
</p>

<p>
  Build, modify, compile, debug, and deploy Arduino and ESP32 projects using autonomous AI agents.
</p>

## Download

### Windows

~~~shell
not yet available
~~~

or [download manually (not yet available)](https://github.com/auralyne-systems/auralyne/releases/latest/download/Auralyne-Setup.exe)

# What is Auralyne?

**Auralyne is a local-first autonomous vibe coding environment specialized in Arduino and ESP32 development.**

Auralyne combines local LLM inference, project context, web research, documentation, libraries, development tools, compilation, debugging, hardware information, schematics, and autonomous agent execution in a single desktop application.

Instead of only generating code, Auralyne is designed to understand an embedded project, inspect its files, research the required information, find and use the appropriate libraries, modify the code, compile it, analyze errors, debug problems, and iterate until the task is completed.

Auralyne can work with **local GGUF models**, models downloaded through **Hugging Face**, or external AI providers using the user's own **API key**.

The local coding workflow runs using **llama.cpp** and local GGUF models.

# Current Features

### Local GGUF inference

Run compatible `.gguf` models directly on your machine using **llama.cpp**.

Auralyne manages the local inference runtime and provides the model layer required by the coding agent.

Models can be:

- Installed manually
- Downloaded through Auralyne
- Downloaded from Hugging Face
- Managed locally
- Selected directly from the application
- Configured for different hardware and use cases

Auralyne can also connect to external AI providers using a user-provided API key.

### Local chat

Auralyne provides a local AI interface with:

- Local model execution
- Model discovery
- Model selection
- Model management
- Persistent conversations
- Conversation history
- Streaming responses
- Markdown rendering
- Code blocks
- Local inference
- External API model support

### Arduino and ESP32 development

Auralyne is specifically designed around embedded development workflows.

The agent can work with:

- Arduino projects
- ESP32 projects
- Arduino sketches
- C/C++ source code
- PlatformIO projects
- Project configuration
- Libraries
- GPIO and peripheral configuration
- Hardware-specific code
- Firmware
- Sensors
- Displays
- Motors
- Communication modules

### Autonomous coding

The coding agent is designed to execute multi-step embedded development tasks.

This includes:

- Reading project files
- Creating files
- Modifying existing code
- Understanding project structure
- Installing or using libraries
- Running development commands
- Compiling firmware
- Inspecting compiler output
- Analyzing errors
- Applying fixes
- Recompiling
- Iterating on tasks
- Verifying the result

### Compilation and debugging

Auralyne can use development tools to validate generated code instead of relying only on the model's assumptions.

The agent can:

- Compile projects
- Inspect compiler errors
- Analyze warnings
- Identify incompatible APIs
- Detect missing libraries
- Apply fixes
- Recompile the project
- Analyze build failures
- Iterate until the code builds correctly

### Web research

Auralyne can research information required to complete a development task.

The agent can use web research to find:

- Arduino documentation
- ESP32 documentation
- Library documentation
- API references
- Hardware specifications
- Examples
- GitHub repositories
- Technical solutions
- Community information

This allows the agent to verify information instead of relying exclusively on its internal knowledge.

### Documentation and library research

Auralyne is designed to work with the documentation required for embedded development.

The agent can search and read:

- Arduino documentation
- ESP32 documentation
- Library documentation
- API references
- GitHub repositories
- Project documentation
- Datasheets
- Technical documents
- Code examples

This is particularly important for Arduino and ESP32 development, where library APIs, board variants, GPIO capabilities, peripheral implementations, and hardware limitations can differ between platforms.

### Hardware-aware development

Auralyne can reason about the hardware context of an embedded project.

The agent can work with:

- GPIO configuration
- Sensors
- Displays
- Motors
- Communication modules
- Wi-Fi
- Bluetooth
- I2C
- SPI
- UART
- PWM
- ADC
- DAC
- ESP32 peripherals
- Arduino peripherals

The objective is to connect the software implementation with the actual hardware requirements of the project.

### Schematics and wiring

Auralyne can create and work with hardware schematics and wiring information.

The agent can help determine:

- Component connections
- GPIO assignments
- Power connections
- Communication buses
- Sensor wiring
- Module connections
- Arduino pin mappings
- ESP32 pin mappings
- Peripheral connections

This allows software and hardware development to be handled together rather than as separate workflows.

### Project-aware development

Auralyne works directly with the user's development projects.

The agent can work with:

- Project files
- Source code
- Directories
- Project configuration
- Libraries
- Build systems
- Local development environments
- Hardware configuration
- Documentation
- Development tools

The project itself becomes part of the AI's context.

# Model Support

Auralyne supports multiple ways of using AI models.

### Local models

Run compatible GGUF models directly on the user's hardware using **llama.cpp**.

Users can:

- Install GGUF models manually
- Download models from Hugging Face
- Download models through the Auralyne marketplace
- Manage installed models
- Select models for their projects
- Configure local inference
- Use different models depending on their hardware

This allows users to run AI locally without sending their source code or project context to an external provider.

### API models

Auralyne can also connect to external AI providers using the user's own API key.

This allows users to choose between:

- Local inference
- External API models
- Different models for different tasks
- Different providers depending on their needs

Users remain in control of which provider and model they use.

# Backend

Auralyne uses a native architecture designed around local inference, autonomous agents, embedded development, and system-level integration.

### Core technologies

- **Rust** — Native backend and system integration
- **llama.cpp** — Local LLM inference
- **GGUF** — Local model format
- **Tauri** — Desktop application framework
- **TypeScript** — Application logic
- **React** — User interface
- **Vite** — Frontend tooling
- **MCP** — Tool and context integration

The architecture separates the user interface from the agent, local inference, development tools, and system layers:

~~~text
React / Tauri
      │
      ▼
 Agent Runtime
      │
 ┌────┴─────────────────────────────┐
 ▼                                  ▼
llama.cpp                        Local Tools
 ▼                                  │
GGUF Models             Files / Shell / Build Tools
                                       │
                         ┌─────────────┴─────────────┐
                         ▼                           ▼
                  Web / Documentation         Arduino / ESP32
                  Libraries / GitHub           Toolchains
                         │                           │
                         └─────────────┬─────────────┘
                                       ▼
                                Compile / Debug
                                       │
                                       ▼
                              Firmware / Schematics
~~~

# Coming Soon

Auralyne is actively under development.

The platform is being expanded into a complete autonomous embedded development environment.

### Vision

Auralyne will support local vision-capable models for tasks such as:

- Screenshot analysis
- Visual debugging
- Hardware setup analysis
- Diagram interpretation
- Image-based development workflows
- Hardware and wiring analysis

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
- Arduino toolchains
- ESP32 toolchains
- Documentation
- Web research
- Libraries
- MCP servers
- APIs
- Git repositories
- Hardware projects
- Schematics
- Multi-step tasks
- Automated workflows

The objective is to provide a **complete embedded vibe coding environment**, rather than a traditional AI chat application.

# Roadmap

~~~text
Current
  │
  ├── GGUF inference
  ├── Local chat
  ├── Model discovery
  ├── Model management
  ├── Hugging Face models
  ├── Manual GGUF installation
  ├── API model support
  ├── Project context
  ├── Arduino / ESP32 development
  ├── Web research
  ├── Documentation research
  ├── Library research
  ├── File operations
  ├── Code generation
  ├── Compilation
  ├── Error analysis
  ├── Debugging
  └── Hardware-aware development
       │
       ▼
Next
  │
  ├── Advanced autonomous agents
  ├── Hardware-aware workflows
  ├── Automated firmware workflows
  ├── Advanced schematics
  ├── MCP
  ├── Git integration
  └── Extended embedded tool ecosystem
       │
       ▼
Future
  │
  ├── Vision
  ├── Voice
  ├── Advanced agent memory
  ├── Multi-step autonomous workflows
  └── Extended local embedded tool ecosystem
~~~

# Philosophy

**Local.**

Run AI directly on the user's hardware whenever possible.

**Autonomous.**

AI should be able to execute complete development tasks rather than only generate code.

**Embedded-first.**

Auralyne is designed specifically around Arduino, ESP32, and embedded development workflows.

**Private.**

Source code, project context, and agent execution should remain local by default.

**Verified.**

AI should be able to research documentation, inspect libraries, compile code, and analyze errors instead of blindly assuming that generated code is correct.

**Flexible.**

Users can choose between local GGUF models, Hugging Face models, and external AI providers using their own API keys.

**Simple.**

Embedded AI development should not require users to manually manage complex inference configuration.

**Powerful.**

Advanced users should be able to control models, tools, runtimes, APIs, MCP servers, and agent behavior.

# Status

> 🚧 Auralyne is currently in active development.

Auralyne is evolving from a local AI coding interface into a **complete autonomous vibe coding environment for Arduino, ESP32, and embedded development**.

Features described in the roadmap are under development and may change as the platform evolves.
