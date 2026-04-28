# Contributing

Thanks for your interest. This is a personal cloud-architecture learning portfolio: a slow-moving collection of designs from a 2022 classic 3-tier through a 2026 hybrid reference. Issues, corrections, and discussion are welcome.

## What's helpful

### 1. Diagram corrections
The whole point is being technically accurate. If you spot:

- A wrong service name, icon, or arrow direction
- A missing dependency (e.g., a private subnet that needs NAT but the diagram doesn't show it)
- An outdated AWS service (deprecated, renamed)

Please open an [Issue](https://github.com/byeongkicho/AWS_Architecture001/issues) with:

- Diagram name / file
- The specific element that's wrong
- What it should be (with reference if possible)

### 2. Suggestions for new architectures
The repo is intended to grow alongside my career — new diagrams as I work on new domains. If you have an idea (e.g., "show a serverless data pipeline pattern"), open an issue with the use-case and the constraints (small business? regulated? cost-sensitive?).

### 3. Learning questions
Honestly OK to open an issue if a diagram doesn't make sense or you want me to elaborate. I treat this repo as a teaching resource for myself first; questions help me clarify.

## Editing diagrams

- All diagrams are draw.io (`.drawio` files) — open with [diagrams.net](https://app.diagrams.net) (free, no signup)
- Keep both the editable `.drawio` source and an exported PNG/SVG when possible
- Mermaid diagrams in README are encouraged for simple flows — GitHub renders them natively

## What this repo isn't

- Not a deployment kit (no Terraform / CloudFormation here — see [smallbiz-cloud-platform](https://github.com/byeongkicho/smallbiz-cloud-platform) for a deployable counterpart)
- Not a comprehensive AWS reference (AWS Well-Architected Framework is the source of truth for that)
- Not opinionated about specific tools beyond what's drawn

## Disclosure

Diagrams are curated by the human author. AI tools (primarily Claude Code) are used for technical writing and consistency checks; the architectural decisions and final correctness are mine.
