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

Quickstart (dev)
```bash
git clone git@github.com:nikajoyboy/Susano.git
cd Susano
make setup        # prepares the dev environment
make build-dev    # fast dev image build
./scripts/run-qemu.sh out/dev/susano-dev.img
```

Typical workflows
- Local development — iterate with `make build-dev` and `./scripts/run-qemu.sh`.
- CI integration — run `make build-dev` in Actions to produce and upload dev artifacts.
- Release — run reproducible `make build-release` in a pinned CI environment; sign artifacts and publish.

Security & responsible use
- Only test systems you own or explicitly have permission to test.
- PoCs and exploit-work are provided for research and validation; do not use them against third-party systems without permission.
- Follow the project SECURITY.md for disclosure and contact details.

Contributing
- Read CONTRIBUTING.md before opening PRs.
- Keep changes small and well-documented.
- Provide tests or reproducible steps for changes that affect builds or runtime behavior.

Releases & signing
- Release artifacts are signed with project GPG keys. Verify checksums and GPG signatures before trusting artifacts.
- Release flow (high level): build in isolated CI → generate checksums → sign artifacts → create GitHub Release with artifacts.

Directory layout
```
Susano/
├── boot/
├── configs/
├── docs/
├── kernel/
├── scripts/
├── src/
├── packages/
├── tools/
├── docker/
├── out/
├── Makefile
├── README.md
├── LICENSE
├── SECURITY.md
└── .gitignore
```

License
- MIT (see LICENSE)

Acknowledgements
Thanks to the open-source projects and maintainers whose work Susano builds on.

Contact
- Project: Susano OS
- Repository: https://github.com/nikajoyboy/Susano
- Security contact: open an issue with the `security` label or see SECURITY.md
