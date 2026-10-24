
<p align="center">
  <img src="https://github.com/user-attachments/assets/260ce434-1501-42d1-a944-c75fbffcbf7c" alt="Auralyne logo" width="240"/>
</p>
<h1 align="center">Auralyne</h1>
<p align="center">
  <strong> Autonomous coding application</strong>
</p>
<p align="center">
  Build, modify, compile, and debug projects with AI agents
</p>

## What is Auralyne?

**Auralyne is a desktop coding environment built around autonomous AI agents.** It is designed to do more than generate snippets: the agent can inspect a project, research technical information, edit files, run available development tools, analyze errors, and work through multi-step tasks.

Auralyne combines AI model management, project context, documentation research, library workflows, compilation, and debugging in one application. Its key differentiator is a dedicated focus on **Arduino, ESP32, and embedded development**, alongside general software coding.

## Key features

### Autonomous coding agent

Depending on the model, available tools, permissions, and project setup, the agent can:

- Inspect project files and understand their structure.
- Create and modify source files.
- Research documentation, APIs, and code examples.
- Find relevant libraries and investigate dependencies.
- Run available development commands.
- Compile projects and inspect build output.
- Analyze errors, apply fixes, and repeat validation.

The goal is to connect research, code changes, and build checks in one workflow rather than making users switch constantly between a chatbot, editor, terminal, and documentation.

### Arduino and ESP32 development

Auralyne is designed for embedded projects as well as conventional software. It can work with:

- Arduino sketches and ESP32 firmware.
- C and C++ source code.
- PlatformIO projects and configuration.
- GPIO and peripheral code.
- Sensors, displays, motors, and communication modules.
- Wi-Fi, Bluetooth, I²C, SPI, UART, PWM, ADC, and DAC use cases.
- Board-specific documentation, libraries, and build requirements.

When the relevant toolchains and dependencies are configured, the agent can help modify firmware, compile projects, and investigate build failures. Check hardware specifications, pin assignments, voltage levels, and power requirements before connecting or powering components.

### Local AI models

Run compatible `.gguf` models on your own computer using **`llama.cpp`**.

- Download supported models through Auralyne or from Hugging Face, where available.
- Import compatible local model files manually.
- Manage and select installed models.
- Choose models based on your hardware and task.
- Run inference locally without sending project context to an external AI provider.

Performance and compatibility depend on the model, quantization, context size, runtime, and available hardware.

### External AI through API keys

Auralyne can connect to supported external AI providers using your own API key. This gives you the flexibility to choose between local inference and hosted models, depending on your needs.

API availability and pricing depend on the provider. Requests sent to an external provider are subject to its service terms and privacy policy.

### Documentation and library research

The agent can research information relevant to a project, including:

- Official Arduino and ESP32 documentation.
- Library documentation and API references.
- GitHub repositories and code examples.
- Datasheets and hardware specifications.
- Project configuration and dependency requirements.

Research results should be checked for relevance and compatibility with the versions used by your project.

### Compilation and debugging

Where the required development tools are available, Auralyne can use real build output to help validate code. Workflows can include compiling a project, inspecting warnings and errors, investigating missing libraries or incompatible APIs, changing source code or configuration, and compiling again.

A successful build does not guarantee that firmware will behave correctly on physical hardware, so testing on the target board remains important.

### Project-aware development

The agent is designed to work with the context of a project, including its files, directories, source code, configuration, libraries, build systems, documentation, and available development tools. This helps connect research and code changes to the actual project instead of treating every request as an isolated prompt.

## Model support

### Local models

Auralyne supports compatible GGUF models through `llama.cpp`. Models can be obtained through supported downloads or imported manually. Local inference offers control over model selection and can keep project context on your machine.

### API models

Supported external AI providers can be used with a user-supplied API key. Model availability, costs, and data handling depend on the selected provider and the current Auralyne integration.

## Architecture and technology

Auralyne uses a desktop architecture that connects the user interface, agent runtime, model inference, and development tools.

### Core technologies

- **Rust** — native backend and system integration.
- **Tauri** — desktop application framework.
- **React** — user interface.
- **Vite** — frontend tooling.
- **llama.cpp** — local language-model inference.
- **GGUF** — supported local model format.
- **MCP** — planned tool and context integration.


## Roadmap

Auralyne is actively evolving. The following are development directions and may not be available in the current build:

- More advanced autonomous agent workflows.
- More complete embedded build and firmware workflows.
- Expanded hardware and schematic support.
- MCP tool integrations and Git integration.
- Local vision-capable models for screenshot, image, and diagram analysis.
- Local voice interaction and speech recognition.
- Improved agent memory and longer multi-step tasks.
- A broader ecosystem of local embedded development tools.

## Philosophy

- **Autonomous** — Help users complete development tasks, not just generate snippets.
- **Embedded-first** — Treat Arduino, ESP32, and microcontroller workflows as core use cases.
- **Local-first** — Support running compatible models directly on the user's hardware.
- **Flexible** — Offer a choice between compatible local models and supported API providers.
- **Verified** — Encourage research, compilation, and error analysis instead of blindly trusting generated code.
- **User-controlled** — Keep model selection and development decisions visible.

## Download

### Windows

**Prebuilt releases are coming soon.** Watch the repository for release announcements, or build Auralyne from source in the meantime.

- [View the GitHub repository](https://github.com/auralyne-systems/auralyne)
- [Check GitHub Releases](https://github.com/auralyne-systems/auralyne/releases)

## Project status

> Auralyne is currently in active development.

Auralyne aims to provide a complete autonomous coding environment for general software development, with a particular focus on Arduino, ESP32, and embedded systems. Available features may vary by build, model, configured toolchain, and connected provider; roadmap items may change as development progresses.
