# Project Chimera Rulebook

## Purpose

The rulebook records the laws of the game world and the development system. It exists so designers, engineers, writers, AI agents, and auditors can reason from shared rules instead of memory.

## Rule Categories

### Physical Laws

Rules that almost never change.

Examples:

- Time behavior
- Collision principles
- Damage resolution order
- Movement constraints
- Networking authority

### World Laws

Rules that define the fiction and systems.

Examples:

- Dungeon structure
- Sponsor mechanics
- Faction rules
- Item rarity
- Safe room behavior
- Memory and reputation

### Narrative Laws

Rules that can evolve through story.

Examples:

- Faction alliances
- Audience preferences
- Sponsor politics
- Floor events
- Character relationships

### Development Laws

Rules that govern how work is designed, implemented, audited, and approved.

Examples:

- Greenfield audit requirement
- 10/10 loop gate
- Evidence-based findings
- No silent standard weakening

## Rule Template

```text
Rule ID:
Name:
Category:
Statement:
Rationale:
Examples:
Exceptions:
How Exceptions Are Explained:
Validation Method:
Related Rules:
Last Modified:
```

## Exception Rule

An exception is allowed only when it has an explicit reason.

Valid exception reasons include:

- Narrative reveal
- Joke payoff
- Sponsor interference
- Buff or debuff
- Player-caused consequence
- Systemic interaction
- Faction action
- Lore-backed anomaly
- Tutorialized special case

Invalid exception reasons include:

- Because it seemed cool
- Because it was random
- Because implementation was easier
- Because the system forgot
- Because the rule was inconvenient

## Surprise Ledger

Every major apparent rule break should be tracked.

```text
Surprise ID:
Description:
Rule Appears Broken:
Actual Reason:
Player Discoverability:
Payoff Plan:
Status:
```

## Narrative Debt

Every unexplained weird event creates debt. Debt must eventually be paid through explanation, consequence, joke, discovery, or revelation.

## Initial Development Rules

### DEV-001: Greenfield Audits Required

Every meaningful review must evaluate the current artifact from scratch.

### DEV-002: Findings Must Be Evidence-Based

Every audit finding must include evidence and a verification method.

### DEV-003: 10/10 Required To Exit Loop

No meaningful task exits until all assigned auditors independently return 10/10.

### DEV-004: Any Unresolved Finding Blocks Exit

Severity determines priority, not whether a finding blocks completion.

### DEV-005: Re-Audits Are Fresh Audits

A re-audit evaluates the full current artifact, not merely whether previous fixes were attempted.

### DEV-006: No Silent Standard Weakening

Any change to quality gates, scoring rules, or audit rigor must be explicitly documented and approved.

## Rulebook Motto

The rules can be strange. They cannot be meaningless.
