# Susano OS — Step-by-Step Operator Guide

> **Status:** Planning and visual-preview stage; no runnable operator console or release image is currently present in this repository.  
> **Platform direction:** Linux; target platforms and requirements remain to be validated.  
> **Purpose:** Explain the project direction and what must be verified before an operator guide can describe actual commands.

---

## Contents

1. [What is Susano OS?](#1-what-is-susano-os)
2. [What is in this repository now?](#2-what-is-in-this-repository-now)
3. [Intended capabilities](#3-intended-capabilities)
4. [How to evaluate the project today](#4-how-to-evaluate-the-project-today)
5. [Safety and authorization](#5-safety-and-authorization)
6. [Release-readiness checklist](#6-release-readiness-checklist)
7. [Demo and funding preparation](#7-demo-and-funding-preparation)

---

## 1. What is Susano OS?

Susano OS is an early-stage concept for a local-first, AI-assisted security research and defensive testing environment. Its proposed direction is to bring an operator interface, local AI assistance, selected security-tool integrations, and report organization into a coherent workflow.

Those are project goals—not claims that these capabilities are already implemented. The repository should be treated as a visual and planning preview until source code, tests, and reproducible setup instructions are available.

## 2. What is in this repository now?

The repository currently contains a README and SVG interface concepts under `assets/`:

- [Companion interface](../assets/companion-interface.svg)
- [Boot screen](../assets/boot-screen.svg)
- [Interactive-mode screen](../assets/interactive-mode.svg)

The images are illustrations, not captures from a running program. There is currently no verified console executable, installer, OS image, model manager, scan implementation, or release package in this repository. Commands and file paths from draft guides should not be assumed to work.

## 3. Intended capabilities

The project may explore these capabilities as implementation and testing progress:

- A terminal interface for organizing security work.
- Optional local-model assistance, with clearly documented network and data behavior.
- A library for organizing operator notes and reports.
- Integrations for authorized, scoped defensive assessments.
- Build, packaging, and release automation.

Each feature should be labeled **implemented**, **experimental**, or **planned**, and supported by tests or a reproducible demonstration before being advertised as available. Local inference by itself does not guarantee that all project data stays on the device; verify network behavior before making privacy claims.

## 4. How to evaluate the project today

There is no runnable setup procedure yet. To review the project, inspect the README and the SVG previews. Do not follow unverified commands from draft documentation, and do not treat mock interface text as evidence that a feature exists.

When a runnable preview is published, its release instructions should identify supported distributions, prerequisites, installation steps, uninstall steps, model requirements, and known limitations. A first demonstration should use a deliberately local, controlled training environment and avoid real accounts, production services, or out-of-scope targets.

## 5. Safety and authorization

Any future security-testing feature should be designed for systems the operator owns or is explicitly authorized to assess. Before a feature can send requests or run probes, the project should document its behavior, obtain clear operator confirmation, provide a way to constrain the authorized scope, and keep an auditable record of actions.

A result should be described as a lead requiring human verification—not a confirmed vulnerability—until it has been checked safely and manually. Do not publish real credentials, session tokens, personal information, or sensitive target details in demos, issue reports, or logs.

## 6. Release-readiness checklist

Before calling the project a usable release, work through these milestones:

- [ ] Add the actual application source and document what is implemented versus planned.
- [ ] Make setup and removal reproducible on a supported Linux distribution.
- [ ] Add automated tests and CI for the supported workflows.
- [ ] Document data flows, local storage, outbound network connections, and model behavior.
- [ ] Define safe defaults, authorization prompts, scope handling, and audit logging for any assessment features.
- [ ] Add a threat model, vulnerability-reporting contact, and responsible-use policy.
- [ ] Produce a demo using a controlled local lab and explain its limitations.
- [ ] Package a preview release with checksums; add signing when release infrastructure is ready.
- [ ] Verify every README and guide command against the release artifact.

## 7. Demo and funding preparation

A short screen recording is useful once there is a real, reproducible workflow to show. Keep it focused: introduce the project and its current status, demonstrate one task in a controlled local environment, show the resulting output, and state what is experimental or not implemented. Do not stage fabricated output as a live feature.

Before recording, hide notifications and unrelated windows; use dummy accounts and data; check terminal history and environment variables for secrets; and avoid showing private IPs, tokens, customer data, or third-party targets. Add captions or narration and provide a text-based reproduction path where possible.

For funding, connect a specific request to verifiable milestones—such as testing, packaging, independent review, documentation, or a defined local-model workload. Explain why existing hardware or CI is insufficient and what a GPU upgrade would enable. Do not make a GPU purchase a release prerequisite until a measured workload demonstrates the need.
