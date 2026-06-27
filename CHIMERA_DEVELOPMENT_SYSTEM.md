# Chimera Development System (CDS)

## Purpose

The Chimera Development System is the AI-native engineering and design methodology used to build Project Chimera. It is designed to resist approval bias, metric gaming, lazy completion, hidden technical debt, and downstream time bombs.

CDS is not a loose workflow. It is a disciplined loop system for turning ideas into verified, audited, evidence-backed work products.

## Core Philosophy

Do not ask an AI to prove that it is right. Build a system where independent agents continuously try to prove each other wrong, and only advance when no evidence of failure remains within the current scope.

## Key Concepts

### 1. Swarms

Swarms are groups of specialized agents that independently propose, analyze, design, or implement work.

Examples:

- Combat Swarm
- Humor Swarm
- Quest Swarm
- Economy Swarm
- Multiplayer Swarm
- AI Architecture Swarm
- Technical Debt Swarm

Swarm members should have distinct perspectives and responsibilities.

### 2. Greenfield Auditors

Auditors evaluate the current artifact from scratch.

They must not see:

- Previous scores
- Previous audit findings
- Previous reviewer comments
- Desired score
- Implementation history
- Prior fixes
- The identity or intent of the implementation agent when avoidable

They should receive only:

- Current specification
- Current artifact or implementation
- Domain-specific evaluation instructions
- Non-leading rubric constraints

### 3. Findings Before Scores

Auditors should primarily produce evidence-backed findings. Scoring may be performed by a separate scoring engine when practical.

This reduces incentive for auditors to inflate or manipulate scores.

### 4. Evidence-Based Evaluation

Every finding must include evidence. Vague criticism is not allowed.

Bad finding:

> Dialogue is repetitive.

Good finding:

> Finding DIA-017: Three merchant NPCs use the same greeting structure in six sampled encounters. This violates Dialogue Variety Standard section 3.2 and reduces perceived NPC individuality.

### 5. Technical Debt Queue

Every finding becomes explicit debt until resolved.

Each item should include:

- ID
- Source audit
- Category
- Severity
- Evidence
- Required fix
- Owner
- Verification method
- Status

### 6. 10/10 Loop Gate

No meaningful task exits its loop until every assigned auditor independently reaches 10/10 under the current scope, with no unresolved findings.

Severity only controls priority. It does not decide whether an issue blocks completion. Any unresolved finding blocks completion.

### 7. Anti-Goodhart Design

CDS must resist Goodhart's Law: when a measure becomes a target, it ceases to be a good measure.

Therefore:

- Do not optimize for score.
- Optimize for reality.
- Hide scoring mechanics where practical.
- Separate auditing from scoring where practical.
- Use greenfield audits.
- Rotate auditor prompts and perspectives.
- Audit the auditors.

## Standard Work Loop

1. Define scope.
2. Write specification.
3. Generate proposal or implementation.
4. Run independent greenfield audits.
5. Convert findings into work items.
6. Fix findings.
7. Re-run fresh audits from scratch.
8. Repeat until every assigned auditor returns 10/10.
9. Record final decision, evidence, and residual risks.
10. Move to next task.

## Loop Exit Rule

A loop exits only when:

- All assigned auditors independently return 10/10.
- All findings are closed.
- All tests pass.
- All acceptance criteria are satisfied.
- All assumptions are documented.
- All known risks are logged or explicitly accepted through governance.
- No hidden TODOs remain inside the current scope.

## Meta-Audit

The development process itself must be audited.

Meta-auditors ask:

- Are auditors becoming predictable?
- Are prompts leading or biased?
- Are agents gaming rubrics?
- Are findings being softened to escape loops?
- Are repeated low-severity findings creating downstream risk?
- Are scoring thresholds being weakened over time?
- Are blind spots recurring?

## CDS Motto

A score below 10 is not failure. It is the map to the next fix.
