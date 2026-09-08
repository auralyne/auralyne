# Contributing to Auralyne

Thank you for your interest in contributing to Auralyne!

Auralyne is an open-source project focused on making local AI simple, fast, and accessible. Contributions of all kinds are welcome, including bug fixes, improvements, documentation, testing, and new features.

## Before You Start

Before making a change, please check:

* Existing Issues to see whether the problem or feature has already been reported.
* Existing Pull Requests to avoid duplicated work.
* The documentation and README for project-specific information.

For large changes or new features, opening an Issue first is recommended so the approach can be discussed before significant development work begins.

## How to Contribute

The recommended contribution workflow is:

1. Fork the repository.
2. Clone your fork locally.
3. Create a new branch from `main`.
4. Make your changes.
5. Test your changes locally.
6. Commit your changes with a clear commit message.
7. Push your branch to your fork.
8. Open a Pull Request against the Auralyne `main` branch.

Do not work directly on the `main` branch.

## Development

Auralyne is currently under active development.

Before submitting a Pull Request, make sure your changes:

* Build successfully.
* Do not introduce avoidable warnings or errors.
* Do not break existing functionality.
* Follow the existing project structure and coding style.
* Include appropriate tests when practical.
* Update documentation when your change affects user-facing behavior.

## Pull Requests

Pull Requests should be focused on a single change whenever possible.

A good Pull Request should explain:

* What was changed.
* Why the change was necessary.
* How the change was tested.
* Any limitations or known issues.

Please keep Pull Requests reasonably small and easy to review.

Large architectural changes should generally be discussed in an Issue before implementation.

## Bug Reports

Before opening a bug report, please search existing Issues to make sure the problem has not already been reported.

When reporting a bug, please provide:

* A clear description of the problem.
* Steps to reproduce it.
* Expected behavior.
* Actual behavior.
* Auralyne version or commit.
* Operating system.
* Relevant hardware information.
* Relevant logs or screenshots when useful.

Do not include passwords, API keys, tokens, private credentials, or other sensitive information in Issues or Pull Requests.

## Feature Requests

Feature requests are welcome.

Please explain:

* What problem the feature would solve.
* Why it would be useful.
* How you expect it to work.
* Any relevant examples or use cases.

For major features or architectural changes, opening an Issue before implementation is strongly recommended.

## Commit Messages

Use clear and descriptive commit messages.

Examples:

```text
fix: resolve llama-server startup issue
feat: add runtime detection
docs: improve installation instructions
refactor: simplify model discovery
```

Avoid vague messages such as:

```text
update
changes
fix stuff
test
```

## Code Quality

Please prefer simple, readable, and maintainable code over unnecessary complexity.

Avoid introducing dependencies unless they provide a clear benefit.

When modifying existing functionality, preserve current behavior unless the change intentionally requires it.

Contributors should follow the existing architecture and conventions of the project rather than introducing unrelated patterns or abstractions.

## Testing

Please test your changes before submitting a Pull Request.

Depending on the change, this may include:

* Building the project successfully.
* Running automated tests.
* Verifying the affected functionality manually.
* Checking for TypeScript, Rust, build, and runtime errors.
* Testing platform-specific behavior when relevant.

Do not submit changes that have not been tested when the affected functionality can reasonably be tested locally.

## Documentation

Documentation improvements are welcome.

When a change affects user-facing behavior, installation, configuration, APIs, or development workflows, update the relevant documentation whenever practical.

## Security

Please do not report security vulnerabilities through public Issues or Pull Requests.

For security vulnerabilities, please follow the instructions in [`SECURITY.md`](SECURITY.md).

Do not include sensitive credentials, API keys, authentication tokens, or other secrets in Issues or Pull Requests.

## Third-Party Software

Auralyne uses third-party libraries, frameworks, runtimes, and other software.

Contributions must respect the licenses of all third-party components used by the project.

Do not submit:

* Code that you do not have permission to redistribute.
* Assets that you do not have permission to use.
* Proprietary software or content without appropriate authorization.
* Dependencies with incompatible licensing requirements.

When adding a dependency, make sure it is properly declared in the appropriate project configuration.

## Code of Conduct

Please be respectful and constructive when interacting with other contributors.

Harassment, discrimination, personal attacks, intimidation, spam, or intentionally disruptive behavior are not welcome.

Technical disagreements are normal. They should be handled professionally and respectfully.

The goal of Auralyne is to build useful software collaboratively.

## License

By contributing to Auralyne, you agree that your contributions may be distributed as part of the project under the project's MIT License.

Unless otherwise stated, contributions must be compatible with the project's licensing requirements.

## Questions and Discussions

For general questions, ideas, and project discussions, please use GitHub Issues or Discussions where appropriate.

Thank you for contributing to Auralyne.
