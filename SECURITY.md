# Security Policy

## Supported Versions

Auralyne is currently under active development. Security updates are provided for the latest stable release.

| Version                            | Supported          |
| ---------------------------------- | ------------------ |
| Latest stable release              | :white_check_mark: |
| Older releases                     | :x:                |
| Development / pre-release versions | :x:                |

## Reporting a Vulnerability

If you discover a security vulnerability in Auralyne, please report it privately rather than opening a public GitHub issue.

Please use GitHub's **Private Vulnerability Reporting** feature if it is available for this repository.

When reporting a vulnerability, please include:

* A clear description of the vulnerability.
* The affected version of Auralyne.
* Steps to reproduce the issue.
* The potential impact.
* Any relevant logs, screenshots, or proof-of-concept information that can safely be shared.

We will review legitimate security reports and provide an acknowledgement as soon as reasonably possible.

Please do not publicly disclose the vulnerability before a fix or mitigation is available.

## Scope

This policy applies to security vulnerabilities affecting Auralyne itself, including:

* The Auralyne application.
* Auralyne's backend and local services.
* Runtime management and runtime installation.
* Model handling where it creates a security vulnerability.
* Update and download mechanisms.
* Security-sensitive interactions between the application and external services.

Third-party software and runtimes, including llama.cpp and its dependencies, may have their own security policies and should also be reported to their respective maintainers when appropriate.

## Out of Scope

The following are generally not considered security vulnerabilities:

* General bugs that do not create a security impact.
* Feature requests.
* Performance issues.
* Issues limited to unsupported or modified builds.
* Vulnerabilities in third-party software that do not originate from Auralyne's integration.

## Responsible Disclosure

Please allow reasonable time for the issue to be investigated and, when applicable, fixed before publicly disclosing details.

Security researchers who report vulnerabilities responsibly will be credited for their contribution when appropriate and with their consent.
