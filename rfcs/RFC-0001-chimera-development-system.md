# RFC-0001: Chimera Development System

## Status

Draft

## Context

Project Chimera requires a development process capable of coordinating human creators, AI agents, Codex sessions, auditors, and future Unreal implementation work.

The process must avoid common failure modes in AI-assisted development:

- Early self-approval
- Biased review prompts
- Hidden technical debt
- Softened quality gates
- Loss of context
- Repeated minor defects becoming downstream failures
- Metrics replacing real quality

## Proposal

Adopt the Chimera Development System (CDS) as the governing methodology for Project Chimera.

CDS is based on:

- Independent swarms
- Greenfield audits
- Evidence-backed findings
- Explicit technical debt tracking
- Fresh re-audits
- 10/10 loop exit requirement
- Meta-audits of the process itself

## Core Loop

```text
Specify -> Implement -> Audit -> Findings -> Fix -> Fresh Audit -> Repeat -> 10/10 -> Advance
```

## Key Rules

1. Auditors evaluate from scratch.
2. Prompts must be non-leading.
3. Findings must be itemized and evidence-backed.
4. Any unresolved finding blocks loop exit.
5. Severity affects priority, not completion.
6. All assigned auditors must independently reach 10/10.
7. The process itself must be audited.

## Alternatives Considered

### Standard Agile Workflow

Rejected as insufficient for adversarial AI-assisted development. Standard tickets and reviews do not prevent self-approval loops.

### Single-Agent Review

Rejected because one evaluator is too vulnerable to bias, context loss, and rubber-stamping.

### Accept Less Than 10/10

Rejected because tolerated minor findings can become hidden downstream failures.

## Risks

- Process overhead may be high.
- Auditors may become predictable.
- Poorly written rubrics may be gamed.
- Excessive looping may slow experimentation.

## Mitigations

- Scope tasks tightly.
- Use clear acceptance criteria.
- Rotate auditor prompts.
- Separate findings from scoring where practical.
- Use meta-audits.
- Allow prototypes to have explicit reduced scope, but not reduced audit honesty.

## Decision Needed

Should CDS become the required development methodology for Project Chimera?

## Current Recommendation

Accept as foundational governance, then improve through meta-audit.
