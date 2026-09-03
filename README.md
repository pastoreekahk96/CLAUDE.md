# CLAUDE.md - Coding Agent Working Contract

This repository contains a reusable `CLAUDE.md` working contract for coding agents. It defines how an agent should reason about work, search before building, test before shipping, handle security, and communicate completion.

## Purpose

The contract is designed to push coding-agent sessions toward complete, testable, understandable results instead of quick code generation. It emphasizes:

- Understanding before implementation
- Deterministic code for deterministic work
- Tests and regression coverage
- Security and secret hygiene
- Simple technology choices
- Clear service boundaries for larger systems
- Explicit completion and blocking states
- Honest communication about failure modes

## Using it

Copy `CLAUDE.md` into the root of a project where Claude Code should follow these instructions. Review the project-specific rules before using it, especially the sections covering LLM access, architecture, deployment, and tooling.

If another coding agent supports its own instruction filename, adapt the file name or copy the contract according to that tool's documented conventions. Avoid maintaining multiple independently edited copies when a single source of truth can be used.

## Customize it first

Before adopting this contract, replace project-specific assumptions with rules that match your environment. In particular, review:

- The human/project name used in the instructions
- LLM access requirements
- Framework and architecture preferences
- Available agent skills and tools
- Testing and evaluation requirements
- Deployment and restart procedures
- Security constraints

The contract is intentionally opinionated. Keep the rules that improve your workflow and remove rules that do not apply.

## Repository contents

```text
CLAUDE.md   # The coding-agent working contract
README.md   # This guide
```

The source contract is kept as a single file so it can be copied into other projects without bringing along unrelated application code.
