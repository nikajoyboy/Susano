<div align="center">

# ⬡ SUSANO OS ⬡
### Local-first AI-assisted security tooling — project concept and interface previews

**Status: early-stage / implementation not yet verified**

</div>

---

## About

Susano OS is a project concept for a local-first security research and defensive testing environment. The intended direction includes a terminal operator interface, local AI assistance, a report library, and integrations with security tools. This repository currently contains the README and visual SVG previews; it does **not** currently contain a runnable console, OS image, or the implementation described in some draft materials.

Capabilities and commands mentioned in design material should be treated as proposals until implemented, tested, and documented against the actual code. No release artifacts or reproducible build instructions are available here yet.

## Interface previews

These are visual concepts, not screenshots of a running build:

| Companion concept | Boot-screen concept | Interactive-console concept |
| --- | --- | --- |
| ![Susano-chi companion interface](assets/companion-interface.svg) | ![Susano OS boot screen](assets/boot-screen.svg) | ![Susano OS interactive AI mode](assets/interactive-mode.svg) |

See [all interface previews](assets/README.md).

## Documentation

- [Step-by-step operator guide](docs/STEP_BY_STEP_GUIDE.md) — current project status, intended workflow, safety boundaries, and a release-readiness checklist.

## Responsible use and safety

The intended use is authorized security work, defensive research, and education. Only test systems you own or have explicit permission to assess. Before presenting any feature as available, verify it in the source and a reproducible test environment. Any future scanning or request-replay functionality should have clear authorization prompts, scope controls, auditability, and safe defaults.

## Contributing and feedback

Feedback on the interface concepts, user needs, and release priorities is welcome through GitHub Issues. Contributions should include a clear description and reproducible evidence for implemented behavior. Do not submit real credentials, private tokens, or sensitive target data.

## Current milestone

The immediate milestone is to establish a working, testable implementation that matches the documented scope, then add CI, reproducible packaging, a threat model, and a signed preview release. Hardware upgrades are not a prerequisite for this documentation and design-preview stage; first identify a tested workload that requires additional GPU capacity.

---

<div align="center">
<sub>Susano OS · Early-stage project · Interface previews are illustrative</sub>
</div>
