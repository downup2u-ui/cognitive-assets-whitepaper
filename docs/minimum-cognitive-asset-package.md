# Minimum Cognitive Asset Package {.unnumbered}

A cognitive asset does not need to begin as a complex database, graph system, or custom software platform. The minimum viable form can be a small, structured folder that preserves enough context, judgment, workflow, and failure memory for future reasoning to resume.

The purpose of a Minimum Cognitive Asset Package is not to document everything. It is to preserve the parts of reasoning that would be costly to reconstruct later.

A practical package can begin as a Markdown-first folder with the following files.

## 1. project-context.md {.unnumbered}

Purpose:
Defines what the project is, what it is not, its current state, constraints, audience, and active goals.

Contains:

- Project summary
- Current stage
- Target audience or user
- Scope boundaries
- Constraints
- Open questions
- What should not be assumed

Why it matters:
Without project context, future AI sessions and human collaborators tend to generalize. The project loses its actual situation and becomes generic.

## 2. glossary.md {.unnumbered}

Purpose:
Stabilizes important terms so future AI systems and human collaborators do not casually reinterpret them.

Contains:

- Core terms
- Working definitions
- Deprecated terms
- Terms that must not be used loosely
- Distinctions that must remain stable

Why it matters:
Long-term work often depends on precise internal language. If terms drift, reasoning drifts with them.

## 3. decision-log.md {.unnumbered}

Purpose:
Preserves major decisions and the reasoning behind them.

Contains:

- Decision
- Date
- Context
- Options considered
- Reason chosen
- Risks accepted
- Reopen condition
- Human owner of the decision

Why it matters:
A decision without its reasoning becomes fragile. A future user may know what was chosen but not why the choice made sense.

## 4. judgment-rules.md {.unnumbered}

Purpose:
Preserves the human-owned criteria used to evaluate outputs, decisions, and risks.

Contains:

- Standards
- Boundaries
- Risk thresholds
- Claims requiring verification
- Decisions requiring human approval
- Conditions that trigger escalation or exit

Why it matters:
Judgment rules prevent AI fluency from becoming synthetic authority. They keep responsibility visible.

## 5. failure-record.md {.unnumbered}

Purpose:
Preserves rejected paths, wrong assumptions, abandoned strategies, and costly lessons.

Contains:

- What was tried
- Why it seemed plausible
- Why it failed
- What should not be repeated
- Whether the failure is contextual or general
- What the failure clarified

Why it matters:
Failure memory is often the most expensive and reusable part of cognition. Without it, old mistakes return under new names.

## 6. workflow-map.md {.unnumbered}

Purpose:
Preserves how work should continue.

Contains:

- Repeatable process
- AI-assisted steps
- Human review steps
- Verification steps
- Handoff rules
- Stop / exit conditions

Why it matters:
A workflow map turns scattered experience into repeatable action. It helps future work continue without depending on improvisation.

## 7. source-and-evidence.md {.unnumbered}

Purpose:
Separates verified knowledge from assumptions, interpretations, and AI-generated claims.

Contains:

- Verified sources
- Unverified claims
- Assumptions
- Evidence gaps
- Claims requiring future review
- Notes on uncertainty

Why it matters:
Persistent cognition becomes dangerous when unsupported claims are preserved as if they were verified knowledge.

## 8. review-status.md {.unnumbered}

Purpose:
Prevents persistent memory from becoming persistent error.

Contains:

- Last reviewed date
- Items requiring review
- Outdated decisions
- Uncertainty markers
- Retired assumptions
- Human owner of final judgment

Why it matters:
A cognitive asset must remain correctable. Review status makes it possible to distinguish active judgment from stale memory.

## Minimal Folder Structure {.unnumbered}

Use this Markdown folder example:

```text
cognitive-asset-package/
|-- project-context.md
|-- glossary.md
|-- decision-log.md
|-- judgment-rules.md
|-- failure-record.md
|-- workflow-map.md
|-- source-and-evidence.md
`-- review-status.md
```

## Minimal Rule {.unnumbered}

The minimum package should answer eight questions:

- What is this project or domain?
- What do the key terms mean?
- What has already been decided?
- What judgment rules govern future work?
- What has already failed?
- How should work continue?
- What evidence supports the current understanding?
- What needs review before being trusted?

If a package can answer these questions, a future human or AI system has a better chance of re-entering the reasoning without restarting from zero.

## Example: decision-log.md Fragment {.unnumbered}

A minimum package becomes easier to understand when at least one file is shown in concrete form. The following fragment illustrates how a `decision-log.md` entry might preserve not only what was decided, but why the decision was made, what alternatives were rejected, what risks were accepted, and when the decision should be reopened.

```markdown
# decision-log.md

## DEC-2026-001 — Use Markdown-first package as the Level 1 format

**Date:** 2026-05-16
**Status:** Active
**Owner:** Xiaoqing Wang
**Authority status:** Human-approved
**Review required:** Yes

### Decision

Use a Markdown-first Cognitive Asset Package as the Level 1 implementation format.

### Context

The whitepaper defines cognitive assets as persistent, reusable, and evolving structures of judgment, reasoning, context, and workflow. A full technical protocol would be premature at this stage because the judgment structure should stabilize before heavier infrastructure is introduced.

### Options Considered

1. Define a formal JSON schema immediately.
2. Use a graph database model as the default structure.
3. Start with a Markdown-first folder structure.

### Reason Chosen

The Markdown-first package is readable by humans, easy to version with Git, portable across AI systems, and low-friction enough for individuals and small teams to maintain. It supports the first operational layer without forcing premature technical complexity.

### Risks Accepted

- Less machine validation than a structured schema.
- Possible inconsistency between files.
- Requires human discipline and periodic review.

### Reopen Condition

Reopen this decision if multiple projects require automated validation, cross-project retrieval, governed access control, or integration with organizational AI systems.
```

This example is intentionally small. A cognitive asset package should begin with the minimum structure needed to preserve judgment. More formal schemas, metadata, or database-backed infrastructure can be added later if reuse, migration, or governance requires it.
