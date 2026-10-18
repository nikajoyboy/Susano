# Susano OS

[![Status](https://img.shields.io/badge/status-active-blue)]() [![License](https://img.shields.io/badge/license-MIT-3b82f6)]()

Susano OS is a security-first, modular operating system and tooling platform for reproducible testing, automation, and hardened deployments. Susano provides a minimal, auditable base with curated tooling for security research, CI integration, and deterministic builds.

Highlights
- Hardened base system with secure defaults
- Deterministic build pipeline for images and ISOs
- Sandboxed runtime for safe PoC validation and tooling
- CI-driven validation and signed release artifacts

Project goals
- Provide a minimal, auditable OS image for research and testing
- Enable reproducible builds and deterministic packaging
- Keep default attack surface small; enable components explicitly
- Provide tooling for safe, sandboxed exploit validation and triage

Supported platforms
- x86_64 (primary)
- ARM64 (experimental)
- QEMU / VirtualBox / VMware for testing
- Containerized toolchain for CI builds

Requirements (developer)
- Linux host (Ubuntu/Debian recommended)
- Docker
- QEMU (for VM testing)
- Python 3.10+
- 8–16 GB RAM recommended
