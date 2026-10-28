# Auralyne

<p align="center">
  <img src="https://github.com/user-attachments/assets/260ce434-1501-42d1-a944-c75fbffcbf7c" alt="Auralyne logo" width="100" />
</p>

<h3 align="center">Local AI. Real hardware. Your ideas.</h3>

<p align="center">
  An AI-powered development environment for Arduino, ESP32, and embedded systems.
  <br />
  Write code, explore solutions, and develop firmware with AI running on your own hardware.
</p>

<p align="center">
  <a href="#the-vision">The vision</a> ·
  <a href="#see-it-in-action">Demo</a> ·
  <a href="#features">Features</a> ·
  <a href="#architecture--technology">Architecture</a> ·
  <a href="#roadmap">Roadmap</a>
</p>

---

## The vision

**Embedded development should feel more accessible, without taking control away from the developer.**

Auralyne is a local-first AI development environment built around the intersection of AI-assisted coding, microcontrollers, and electronics.

The goal is to bring AI assistance closer to the hardware development workflow — from understanding an existing project to writing firmware and investigating errors.

Designed with local AI at its core, Auralyne aims to give developers greater control over their models, their configuration, and their projects.

## See it in action

<p align="center">
  <img
    src="./assets/auralyne-demo.gif"
    alt="Auralyne — local AI coding assistant demonstration"
    width="900"
  />
</p>

<p align="center">
  <em>From an idea to code, with AI as your development partner.</em>
</p>

## Features

### AI-assisted development

- **AI coding agent** — Generate, explain, and modify code with AI assistance.
- **Project-aware workflows** — Work with existing project files and code.
- **Debugging assistance** — Investigate errors and explore possible solutions.

### Built for embedded systems

- **Arduino and ESP32** — Focused on microcontroller development.
- **Libraries and pin guidance** — Get assistance with board-specific details and hardware integration.
- **Hardware-oriented workflows** — A foundation for connecting firmware development with electronics and wiring.

### Local-first AI

- **Local model inference** — Run compatible GGUF models through [`llama.cpp`](https://github.com/ggml-org/llama.cpp).
- **Configurable inference** — Adjust supported model settings to suit your hardware and workflow.
- **Greater control** — Keep local inference on your own machine when using local models.

*Capabilities and hardware support are actively evolving.*

## Architecture & technology

Auralyne combines a desktop application, a web-based user interface, a native backend, local model inference, and persistent data storage.

### Technology stack

| Layer | Technology | Official documentation |
|---|---|---|
| Desktop framework | [Tauri](https://tauri.app/) | [Architecture](https://tauri.app/concept/architecture/) · [Process model](https://tauri.app/concept/process-model/) |
| Frontend | [React](https://react.dev/) | [Learn React](https://react.dev/learn) · [API reference](https://react.dev/reference/react) |
| Build tooling | [Vite](https://vite.dev/) | [Getting started](https://vite.dev/guide/) · [Configuration](https://vite.dev/config/) |
| Native backend | [Rust](https://www.rust-lang.org/) | [The Rust Book](https://doc.rust-lang.org/book/) · [Standard library](https://doc.rust-lang.org/std/) |
| Local inference | [llama.cpp](https://github.com/ggml-org/llama.cpp) | [Repository](https://github.com/ggml-org/llama.cpp) · [Build instructions](https://github.com/ggml-org/llama.cpp/blob/master/docs/build.md) |
| Model format | [GGUF](https://github.com/ggml-org/llama.cpp/wiki) | [llama.cpp documentation and wiki](https://github.com/ggml-org/llama.cpp/wiki) |
| Database | [SQLite](https://sqlite.org/) | [Documentation](https://sqlite.org/docs.html) · [SQL language](https://sqlite.org/lang.html) |
| Web technologies | [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML) · [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS) · [JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) | [MDN Web Docs](https://developer.mozilla.org/) |

### How the architecture fits together

- **Desktop layer:** Tauri connects the desktop application to its native capabilities through a WebView and a Rust-based core.
- **Interface layer:** React handles the component-based user interface, while Vite provides the development server and build tooling.
- **Backend layer:** Rust provides native application functionality and access to system-level operations.
- **AI layer:** `llama.cpp` provides local inference for compatible GGUF models.
- **Persistence layer:** SQLite stores application data locally.


## Local AI & model ecosystem

Auralyne is designed to work with compatible local GGUF models through `llama.cpp`.

Actual performance depends on the model architecture, quantization, context size, available memory, and hardware acceleration.

### Model and inference references

| Resource | Description |
|---|---|
| [`llama.cpp`](https://github.com/ggml-org/llama.cpp) | C/C++ inference engine for supported language models |
| [GGUF format documentation](https://github.com/ggml-org/llama.cpp/wiki) | References for the model file format and ecosystem |
| [Hugging Face Hub](https://huggingface.co/models) | Discover publicly available models |
| [Hugging Face GGUF documentation](https://huggingface.co/docs/hub/gguf) | Learn about GGUF model files |
| [Hugging Face Transformers documentation](https://huggingface.co/docs/transformers/index) | Reference for model architectures and machine learning workflows |

These are ecosystem references, not a guarantee that every model, format, or external service is supported directly by Auralyne.

## Embedded development resources

Auralyne focuses on the workflow around microcontrollers and firmware development.

| Resource | What it covers |
|---|---|
| [Arduino documentation](https://docs.arduino.cc/) | Boards, programming, libraries, and development tools |
| [Arduino language reference](https://docs.arduino.cc/language-reference/) | Core language functions and syntax |
| [Arduino libraries](https://docs.arduino.cc/libraries/) | Library discovery and documentation |
| [Espressif documentation](https://docs.espressif.com/) | Official ESP32 and Espressif technical documentation |
| [ESP-IDF programming guide](https://docs.espressif.com/projects/esp-idf/en/stable/esp32/) | Espressif's development framework for ESP32 |
| [ESP32 technical documents](https://www.espressif.com/en/support/documents/technical-documents/esp32-) | Hardware manuals and technical references |
| [PlatformIO documentation](https://docs.platformio.org/) | An additional reference for embedded development workflows |

The availability of a reference does not imply that its associated toolchain is fully integrated into Auralyne.

## Roadmap

Auralyne is under active development. This roadmap describes areas of work, not guaranteed release dates.

- [x] Desktop application foundation
- [x] Local-first architecture
- [x] Initial GGUF model integration
- [ ] Improve autonomous coding and multi-step workflows
- [ ] Strengthen compilation and debugging assistance
- [ ] Expand board and library support
- [ ] Improve model downloads and management
- [ ] Develop hardware and wiring visualization
- [ ] Refine the overall user experience

## Design principles

| Principle | What it means |
|---|---|
| **Local first** | Prioritize local inference and user control. |
| **Developer focused** | Keep the workflow centered on real projects. |
| **Hardware aware** | Build around the needs of embedded development. |
| **Configurable** | Make relevant model settings accessible. |
| **Iterative** | Develop, test, and improve through feedback. |

## Project status

Auralyne is an independent project in active development. Its features, supported models, and workflows may change as development continues.

The long-term goal is to create a cohesive environment where AI-assisted software development and embedded hardware projects work together naturally.

## Feedback & contributions

Ideas, feedback, and suggestions are welcome.

If you're interested in local AI, embedded development, or the intersection of software and hardware, follow the project's progress and share your thoughts.
