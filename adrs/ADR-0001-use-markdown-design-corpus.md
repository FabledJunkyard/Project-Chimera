# ADR-0001: Use Markdown Design Corpus

## Status

Accepted

## Context

Project Chimera needs a durable, version-controlled source of truth that can be read and modified by humans, Codex, AI agents, and future automation.

The project will include game design, technical architecture, AI prompts, audit reports, RFCs, ADRs, production plans, and future Unreal implementation notes.

## Decision

Use a Markdown-first repository structure for the initial design corpus.

Markdown will be used for:

- Constitution
- Governance
- Development system
- Rulebook
- RFCs
- ADRs
- GDD sections
- Technical specs
- AI specs
- Audit templates
- Production plans

## Consequences

### Benefits

- Human-readable
- Git-friendly
- Easy for Codex and LLMs to edit
- Diffable
- Portable
- Compatible with documentation generators
- Suitable for long-term institutional memory

### Tradeoffs

- Diagrams may require separate formats.
- Large specs may need indexing.
- Future structured data may require JSON, YAML, CSV, or database-backed tools.

## Follow-Up

Future ADRs should decide:

- Diagram format
- Structured schema format
- Unreal project layout
- CI documentation validation
- Audit report schema
