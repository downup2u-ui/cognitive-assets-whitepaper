# Cognitive Asset Package Specification v0.1

## Purpose

A Cognitive Asset Package is a structured preservation unit for human-AI collaboration.

Its purpose is to make human judgment, project context, decision history, failed paths, constraints, and AI collaboration protocols recoverable across time. It is designed for situations where AI-assisted work should not depend only on personal memory, platform-specific chat history, or scattered files.

A Cognitive Asset Package is not an ordinary folder and not a raw chat export. It is a deliberate structure for restoring the conditions of responsible cognition.

## Relationship to the Canonical MCAP Structure

This specification is based on the Minimum Cognitive Asset Package (MCAP) structure introduced in the whitepaper *Cognitive Assets: The Emergence of Persistent Human-AI Cognition*.

The whitepaper's MCAP structure is the canonical structure for this project. This specification explains that structure in a more formal and implementation-oriented way. The `template-repo/` directory is the practical implementation layer: it provides editable Markdown files that users can copy, adapt, and maintain.

Additional files may be added for specific domains, workflows, or publication contexts. However, the canonical MCAP files should not be missing from a package that claims alignment with this specification.

If a template uses alternative or supporting filenames, it should clearly explain how those files relate to the canonical structure.

## Normative Language

The following terms define the strength of requirements in this specification:

- `MUST` indicates a requirement for canonical MCAP alignment.
- `SHOULD` indicates a strong recommendation that may be adapted with justification.
- `MAY` indicates an optional practice or extension.
- `MUST NOT` indicates a prohibited practice that would undermine the purpose, safety, or integrity of the package.

## Scope

This specification defines a minimum structure for packaging cognitive assets in Markdown-based repositories or folders.

It applies to:

- individual research projects
- writing and editorial projects
- software and product projects
- organizational knowledge preservation
- long-term human-AI collaboration workflows
- AI-assisted decision support contexts
- portable restoration across AI systems

The specification is intentionally lightweight. It is designed to be understandable, editable, and usable without specialized software.

## Non-goals

This specification does not attempt to:

- preserve every AI interaction
- define a legal evidence standard
- replace formal records management systems
- replace version control, citation managers, or data repositories
- certify the truth of preserved claims
- grant AI systems decision authority
- require proprietary tools or platforms
- prescribe one universal workflow for all domains

A Cognitive Asset Package may support accountability, but it is not by itself an accountability regime.

## Core Concepts

### Cognitive Asset

A cognitive asset is a durable structure that preserves context, judgment, constraints, decisions, rejected paths, and continuity from human-AI collaboration.

### Cognitive Asset Package

A Cognitive Asset Package is a folder or repository organized according to this specification. It contains the minimum materials needed to help a human or AI system restore the relevant cognitive context of a project.

### Judgment

Judgment refers to the human evaluative structure behind decisions: what matters, what is acceptable, what is risky, what should be rejected, and what should remain under human authority.

### Continuity

Continuity is the ability to resume a line of work without reconstructing its background from memory or unstructured chat history.

### Authority Boundary

An authority boundary defines which decisions an AI system may assist with and which decisions must remain under human responsibility.

### Negative Knowledge

Negative knowledge includes rejected options, failed attempts, misleading framings, and known paths that should not be repeated without review.

## Minimum Cognitive Asset Package

A minimum Cognitive Asset Package should include enough material for a future reader, collaborator, or AI system to understand:

- who or what the package represents
- what project or domain it supports
- what principles guide judgment
- what decisions have already been made
- what paths were rejected and why
- how AI should assist
- what AI should not decide
- what risks or constraints remain active
- what must be reviewed before reuse

The minimum package should be human-readable and portable.

## Canonical File Structure

The canonical MCAP structure consists of eight files. A package that claims canonical MCAP alignment MUST include these files or a clearly documented equivalent mapping.

### project-context.md

Purpose:

Defines what the project is, what it is not, its current state, constraints, audience, scope boundaries, active goals, and open questions.

Why it matters:

Without project context, future AI sessions and human collaborators may generalize incorrectly. The project can lose its actual situation and become generic.

What should NOT go inside:

- credentials, private keys, or access tokens
- unnecessary personal identity details
- confidential client information unless explicitly required and protected
- raw chat transcripts that have not been reviewed
- obsolete context that is not clearly marked as archived or retired

### glossary.md

Purpose:

Stabilizes important terms, working definitions, deprecated terms, and distinctions that should not drift across future work.

Why it matters:

Long-term human-AI work often depends on precise internal language. If terms drift, reasoning drifts with them.

What should NOT go inside:

- invented definitions presented as established external standards
- terms copied from sources without attribution when attribution is required
- unresolved terminology disputes presented as settled definitions
- private or sensitive labels that are unnecessary for restoration

### decision-log.md

Purpose:

Preserves major decisions and the reasoning behind them, including context, options considered, chosen path, rejected paths, risks accepted, authority status, and reopen conditions.

Why it matters:

A decision without its reasoning becomes fragile. A future user may know what was chosen but not why the choice made sense.

What should NOT go inside:

- decisions attributed to AI as final authority
- unreviewed AI recommendations presented as approved decisions
- confidential deliberations that should be summarized or redacted
- decisions without owner, date, or review status when those fields are available

### judgment-rules.md

Purpose:

Preserves the human-owned criteria used to evaluate outputs, decisions, risks, claims, and AI assistance.

Why it matters:

Judgment rules prevent AI fluency from becoming synthetic authority. They keep responsibility visible and reviewable.

What should NOT go inside:

- rules that delegate final responsibility to AI
- vague preferences that cannot guide future review
- safety, legal, medical, or financial rules presented as expert advice without review
- instructions that conflict with privacy or confidentiality obligations

### failure-record.md

Purpose:

Preserves rejected paths, wrong assumptions, abandoned strategies, misleading outputs, and costly lessons in reusable form.

Why it matters:

Failure memory is often one of the most expensive and reusable parts of cognition. Without it, old mistakes may return under new names.

What should NOT go inside:

- blame-oriented personal records
- sensitive incident details that should be redacted or handled separately
- failures without context or lesson learned
- unverified accusations or claims about people, organizations, or systems

### workflow-map.md

Purpose:

Preserves how work should continue, including repeatable processes, AI-assisted steps, human review steps, verification steps, handoff rules, and stop conditions.

Why it matters:

A workflow map turns scattered experience into repeatable action. It helps future work continue without depending entirely on improvisation.

What should NOT go inside:

- credentials or operational secrets
- irreversible automation instructions without review gates
- workflows that bypass human authority for consequential decisions
- outdated procedures that are not marked as retired

### source-and-evidence.md

Purpose:

Separates verified knowledge from assumptions, interpretations, AI-generated claims, evidence gaps, and claims requiring review.

Why it matters:

Persistent cognition becomes dangerous when unsupported claims are preserved as if they were verified knowledge.

What should NOT go inside:

- fabricated citations
- unverifiable claims presented as verified evidence
- copyrighted source material copied beyond permitted use
- confidential sources that should be anonymized or protected

### review-status.md

Purpose:

Tracks last reviewed dates, items requiring review, outdated decisions, uncertainty markers, retired assumptions, and human ownership of final judgment.

Why it matters:

A cognitive asset must remain correctable. Review status helps distinguish active judgment from stale memory.

What should NOT go inside:

- false claims that material has been reviewed
- review dates without reviewers or responsible owners when those are known
- obsolete material left unmarked
- AI-generated status updates treated as human-approved without review

## Recommended Directory Structure

```text
cognitive-asset-package/
├── README.md
├── project-context.md
├── glossary.md
├── decision-log.md
├── judgment-rules.md
├── failure-record.md
├── workflow-map.md
├── source-and-evidence.md
├── review-status.md
├── STRUCTURE.md
└── support/
    ├── profile.md
    ├── judgment-principles.md
    ├── decision-history.md
    ├── ai-collaboration-protocol.md
    └── export-checklist.md
```

This structure may be adapted for specific domains, but the eight canonical MCAP files MUST remain present or explicitly mapped.

## Required Files

### README.md

Explains what the package is, who it is for, how it should be used, and what should not be placed inside it.

### project-context.md

Defines the project, domain, scope, constraints, audience, current stage, and open questions.

### glossary.md

Defines stable terms, working definitions, deprecated terms, and distinctions that should not drift.

### decision-log.md

Records important decisions in a structured format. Each entry should include date, context, options considered, chosen path, rejected paths, reasons, and review status.

### judgment-rules.md

Defines human-owned judgment criteria, authority boundaries, risk thresholds, escalation rules, and verification requirements.

### failure-record.md

Records failed paths, rejected assumptions, misleading outputs, and lessons that should inform future reasoning.

### workflow-map.md

Defines how work should continue, including repeatable processes, AI-assisted steps, human review steps, verification steps, and stop conditions.

### source-and-evidence.md

Separates verified sources, assumptions, interpretations, AI-generated claims, evidence gaps, and claims requiring review.

### review-status.md

Tracks review dates, uncertainty markers, outdated decisions, retired assumptions, and human ownership of final judgment.

## Optional Files

### profile.md

Describes the owner or project identifier, domain background, stable preferences, collaboration style, and assumptions that should not be made.

### judgment-principles.md

Provides a publication-facing or user-facing version of `judgment-rules.md`.

### decision-history.md

Provides a support format or extended narrative version of `decision-log.md`.

### ai-collaboration-protocol.md

Defines how AI systems should assist, what they should not decide, how uncertainty should be handled, and how context should be preserved.

### export-checklist.md

Defines what should be exported, removed, anonymized, verified, and restored when moving the package into another AI system or repository.

### restoration-notes.md

Provides instructions for reloading the package into a new AI system, including priority order and known limitations.

### review-log.md

Tracks package reviews, updates, obsolete entries, and unresolved issues.

## Metadata

A Cognitive Asset Package should include basic metadata in the `README.md` or a separate metadata file.

Recommended metadata:

- package title
- package owner or maintainer
- version
- creation date
- last reviewed date
- domain or project type
- review status
- confidentiality level
- intended restoration context
- license or reuse terms, if applicable

Example:

```yaml
title: Example Cognitive Asset Package
version: 0.1
owner: Example Owner
created: 2026-01-01
last_reviewed: 2026-01-15
domain: research-writing
review_status: draft
confidentiality: private
intended_restoration: AI-assisted research continuation
```

## Portability

A Cognitive Asset Package should be portable across systems.

Portability means:

- files are readable without proprietary software
- core materials are stored in plain text or Markdown
- package structure is understandable from the root `README.md`
- context is explicit enough to be restored in another AI environment
- sensitive information is removed or marked before transfer
- platform-specific exports are summarized or referenced rather than treated as the package itself

Portability does not require that every AI system interpret the package identically. It requires that the human context be recoverable enough for responsible continuation.

## Privacy and Classification

A Cognitive Asset Package SHOULD declare its privacy and classification status before it is shared, archived, or restored in another system.

### Public Package

A public package is intended for open publication. It MUST NOT contain credentials, unnecessary personally identifiable information, confidential client data, private communications, or sensitive operational details. It SHOULD be reviewed and redacted before publication.

### Private Package

A private package is intended for personal or restricted use. It MAY contain more detailed context than a public package, but it SHOULD still avoid unnecessary sensitive information and MUST protect credentials, secrets, and high-risk personal data.

### Internal Package

An internal package is intended for use inside a team or organization. It SHOULD follow organizational privacy, security, legal, and records-management requirements. It MUST NOT be treated as public unless it has passed a publication review.

### Redaction

Redaction removes information that should not be shared. Redaction SHOULD be used for credentials, private contact details, confidential client information, sensitive operational details, and any material that is unnecessary for restoration.

### Anonymization

Anonymization replaces identifying information with non-identifying descriptions. If anonymization changes the meaning or evidentiary value of a record, the package SHOULD state that limitation.

### Sensitive Information Handling

A Cognitive Asset Package MUST NOT include passwords, API keys, access tokens, private keys, or credentials. It SHOULD minimize personally identifiable information, confidential material, private communications, and sensitive organizational details. Where sensitive context is necessary, the package SHOULD summarize, redact, or classify it clearly.

## Review Status

Each package should clearly indicate its review status.

Suggested review status values:

- `draft` — incomplete and not yet reviewed
- `active` — currently used and maintained
- `review-needed` — usable but requires human review before restoration
- `archived` — preserved for reference, not actively maintained
- `obsolete` — no longer reliable for future use

Decision entries may also have their own review status.

## Risk Boundaries

A Cognitive Asset Package should define risk boundaries explicitly.

Risk boundaries may include:

- decisions that AI must not make
- domains requiring expert review
- claims requiring source verification
- privacy-sensitive material that must not be exported
- confidential information that must be redacted
- assumptions that must be revalidated before reuse
- actions that require human confirmation

The package should avoid creating a false sense of authority. Preservation helps restore context; it does not guarantee correctness.

## Validation Checklist

Before a package is treated as canonical MCAP-aligned, verify that:

- authority boundaries are present
- review status is defined
- evidence traceability is present
- decision history is recoverable
- privacy review is completed
- obsolete content is marked
- canonical files are present or explicitly mapped
- AI-drafted material is distinguished from human-approved material
- sensitive information has been removed, redacted, anonymized, or classified
- claims requiring verification are marked
- rejected paths and failure records are recoverable
- restoration instructions do not grant AI final judgment authority

## Example Use Cases

### Research Continuation

A researcher uses a package to preserve definitions, rejected framings, source boundaries, and unresolved questions so that future AI-assisted writing can resume without restarting the conceptual work.

### Editorial Voice Preservation

An author preserves stable writing preferences, tone boundaries, conceptual vocabulary, and unacceptable edits so that future AI editing does not distort the author's judgment.

### Software Architecture Memory

A development team records architecture decisions, rejected shortcuts, security constraints, and AI coding rules so that future implementation work remains aligned with earlier reasoning.

### Organizational Decision Support

An organization preserves AI-assisted decision context, authority boundaries, review rules, and decision history so that later reviewers can understand how recommendations were evaluated.

### Cross-Platform AI Restoration

A user migrates from one AI system to another and uses the package to restore project context, collaboration protocol, and known constraints without depending on proprietary chat memory.

## Future Versions

Future versions of this specification may address:

- machine-readable metadata schemas
- domain-specific package profiles
- privacy and redaction conventions
- versioning standards
- compatibility with GitHub template repositories
- restoration prompts for different AI systems
- package validation checklists
- links to archival repositories such as Zenodo
- integration with decision legitimacy and judgment authority frameworks

Version `v0.1` should be treated as an initial draft for experimentation and public discussion.
