# Decision Framework

## Purpose

This framework defines how Project Chimera evaluates proposals, features, systems, designs, and implementations.

The goal is to prevent weak ideas, hidden assumptions, untested work, and biased approvals from entering the project.

## Decision Inputs

A decision should include:

- Problem statement
- Proposed solution
- Alternatives considered
- Scope
- Acceptance criteria
- Dependencies
- Risks
- Test plan
- Audit plan
- Exit criteria

## Proposal Review Structure

1. Proposal owner drafts the idea.
2. Relevant swarm members independently review.
3. Auditors evaluate from a clean starting point.
4. Findings become work items.
5. Proposal is revised.
6. Re-audit runs from scratch.
7. Loop continues until the required standard is met.
8. Decision is recorded.

## Scoring Philosophy

Scores are measurements, not the mission.

Project Chimera uses 10/10 as the gate, but the work must be judged by evidence, tests, coherence, player trust, fun, maintainability, and clear acceptance criteria.

## Suggested Evaluation Categories

Category weights may vary by domain.

- Fun
- Story Tell Value
- Player Trust
- Originality
- Technical Feasibility
- Maintainability
- Scalability
- Replayability
- Production Cost
- Performance Risk
- AI Synergy
- Accessibility
- Live Ops Potential
- Lore Consistency
- Economy Impact
- Testability

## Finding-Derived Scoring

Where practical, auditors produce findings and a separate scoring step computes the resulting score.

Example model:

```text
10.0 minus unresolved finding penalties
```

The gate remains simple:

```text
Any unresolved finding means the loop continues.
All assigned auditors return 10/10 means the item is eligible to advance.
```

## Required Decision Record

Every accepted decision should record:

- Decision ID
- Date
- Owner
- Scope
- Decision
- Rationale
- Alternatives rejected
- Final audit state
- Known risks
- Follow-up tasks

## Explicit Rejection

A decision can be rejected for any of the following:

- Violates the constitution
- Weakens player trust
- Lacks meaningful player agency
- Creates unbounded technical debt
- Cannot be tested
- Cannot be explained
- Creates contradictions
- Treats the score as more important than the result
- Fails to reach 10/10 after revision attempts

## Defer Rule

A decision may be deferred when:

- Scope is premature
- Required information is missing
- Prototype is needed
- Dependencies are unresolved

Deferred decisions must be tracked. They may not silently disappear.

## Decision Motto

A good decision is not one everyone likes. A good decision is one future contributors can understand, test, and challenge.
