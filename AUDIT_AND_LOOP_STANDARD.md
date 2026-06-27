# Audit And Loop Standard

## Purpose

This standard defines how Project Chimera evaluates work products, code, design documents, quests, dialogue, mechanics, technical architecture, and AI-generated artifacts.

The standard exists to prevent early loop exits, lazy approval, hidden technical debt, and downstream failures caused by tolerated minor defects.

## Prime Directive

Every audit must attempt to discover evidence that the artifact fails to satisfy its specification.

Audits are not approval rituals. They are falsification attempts.

## Greenfield Audit Requirement

Every audit must be greenfield.

A greenfield auditor receives:

- The current artifact
- The current specification
- The relevant domain checklist
- Any required acceptance criteria

A greenfield auditor does not receive:

- Previous audit scores
- Previous findings
- Previous fixes
- Desired score
- Expected conclusion
- Implementation agent notes
- Other auditor opinions

## Non-Leading Prompt Rule

Audit prompts must avoid wording that implies the artifact should pass.

Avoid:

- "Confirm this is complete."
- "Check that the fixes worked."
- "Verify this is now 10/10."
- "Make sure this passes."

Prefer:

- "Evaluate the current artifact against the specification. Identify all evidence of deficiency, ambiguity, inconsistency, missing behavior, hidden assumptions, or verification gaps."
- "Attempt to falsify the claim that this artifact satisfies its current scope."

## Auditor Output Format

Each audit must return:

```text
Audit ID:
Artifact:
Scope:
Auditor Type:
Inputs Reviewed:
Areas Examined:
Findings:
Score Recommendation or Finding Summary:
Confidence:
Open Questions:
Required Retest Areas:
```

Each finding must include:

```text
Finding ID:
Category:
Severity:
Evidence:
Violated Requirement:
Impact:
Required Fix:
Verification Method:
Retest Instruction:
Score Impact If Scoring Is Used:
Status:
```

## Finding Severity

Severity communicates priority, not completion status.

All unresolved findings block loop exit.

Severity levels:

- Critical
- Major
- Medium
- Minor
- Nit
- Unknown / Question

A Nit still blocks completion until fixed, rejected through explicit governance, or converted into a documented out-of-scope item.

## 10/10 Gate

No meaningful task exits its loop unless all assigned auditors independently return 10/10.

10/10 means:

- No unresolved findings remain within the current scope.
- No known requirement deviations remain.
- No skipped required tests remain.
- No undocumented assumptions remain.
- No hidden TODOs remain.
- No open verification gaps remain.
- No unresolved ambiguities remain.

## Score Gaming Protections

To reduce rubric gaming:

1. Auditors should not know target score requirements when practical.
2. Auditors should focus on findings rather than scores.
3. Scoring should be derived from findings where practical.
4. Implementation agents should not receive hidden scoring weights.
5. Re-audits must be fresh evaluations, not fix confirmations.
6. Auditor prompts should rotate over time.
7. Meta-audits should inspect whether the process is being gamed.

## Loop Pattern

```text
Specify -> Implement -> Greenfield Audit -> Findings -> Fix -> Fresh Greenfield Audit -> Repeat -> 10/10 -> Advance
```

## Required Loop Exit Evidence

Before exit, the task record must contain:

- Final artifact version
- Scope statement
- Auditor list
- Final audit reports
- Evidence that all findings are closed
- Test results
- Open risks, if any
- Explicit approval decision

## Important Distinction

10/10 does not mean perfect forever.

It means no known deficiency remains under the current declared scope, specification, rubric, and verification standard.

If scope expands later, the loop reopens.
