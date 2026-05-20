# Template Repository Structure

This file explains how this template aligns with the canonical Minimum Cognitive Asset Package (MCAP) structure from the whitepaper *Cognitive Assets: The Emergence of Persistent Human-AI Cognition*.

## Relationship to the Whitepaper Specification

The whitepaper defines the canonical MCAP structure. The specification in `publications/specification/cognitive-asset-package-spec-v0.1.md` explains that structure in a more formal way. This template repository is the practical implementation layer.

A package may add support files, but the canonical MCAP files should not be missing from a package that claims alignment with the whitepaper or specification.

## Canonical MCAP Files

The canonical files are:

- `project-context.md` — defines project purpose, scope, constraints, current state, and open questions.
- `glossary.md` — stabilizes terms, definitions, deprecated terms, and distinctions.
- `decision-log.md` — preserves major decisions, reasoning, rejected options, authority status, and reopen conditions.
- `judgment-rules.md` — preserves human-owned evaluation rules, authority boundaries, and risk thresholds.
- `failure-record.md` — preserves rejected paths, failed assumptions, misleading outputs, and lessons learned.
- `workflow-map.md` — preserves repeatable processes, AI-assisted steps, human review steps, and stop conditions.
- `source-and-evidence.md` — separates verified sources, assumptions, AI-generated claims, and evidence gaps.
- `review-status.md` — tracks review dates, uncertainty markers, obsolete content, and human approval status.

## Optional Files

Optional files may be added for domain-specific needs, including:

- restoration notes
- review logs
- source maps
- publication notes
- domain-specific checklists
- machine-readable metadata

Optional files should support the canonical structure rather than replace it.

## Support Files in This Template

This template also includes support files:

- `profile.md` — a safe owner or project profile for collaboration preferences and do-not-assume guidance.
- `judgment-principles.md` — a user-facing companion to `judgment-rules.md`.
- `decision-history.md` — a support or extended narrative companion to `decision-log.md`.
- `ai-collaboration-protocol.md` — instructions for how AI should assist without taking final authority.
- `export-checklist.md` — privacy, anonymization, verification, and restoration checklist.

## Publication-Facing Files

The following files may be useful when preparing a package for public release:

- `README.md`
- `STRUCTURE.md`
- `export-checklist.md`
- selected excerpts from canonical files after privacy review

A private or internal package should not be published without redaction, anonymization, and review.

## Alignment Rule

For this template to remain canonical MCAP-aligned:

- the eight canonical files should remain present
- support files should not redefine the standard
- public-facing materials should point back to the whitepaper and specification
- AI-generated updates should not become durable records without human approval
- obsolete material should be marked rather than silently preserved as active context
