# Export Checklist

Use this checklist before exporting, sharing, archiving, or restoring a Cognitive Asset Package in another AI system.

## What to Export

Export materials that are necessary for responsible continuation:

- package `README.md`
- owner or project `profile.md`
- `judgment-principles.md`
- `decision-history.md`
- `ai-collaboration-protocol.md`
- important glossary or terminology notes
- current project status
- unresolved questions
- known risks and constraints
- review notes
- restoration instructions

Optional exports:

- summarized chat history
- failure log
- source map
- selected examples of preferred output
- selected examples of rejected output

## What to Remove

Remove material that is unnecessary, misleading, obsolete, or unsafe to transfer:

- passwords, tokens, API keys, or credentials
- unrelated personal information
- irrelevant raw chat material
- duplicate drafts that create confusion
- outdated instructions not marked as obsolete
- unverified claims presented as settled facts
- private information that is not required for restoration

## What to Anonymize

Anonymize or generalize sensitive information before export:

- names of private individuals
- private contact information
- confidential organizational details
- client or participant identifiers
- sensitive location information
- unpublished private communications
- personal biographical details not required for the work

When anonymization changes meaning, add a note explaining the limitation.

## What to Verify

Before export, verify:

- the package version
- last reviewed date
- current review status
- whether decision entries are up to date
- whether rejected paths are clearly explained
- whether AI authority boundaries are explicit
- whether factual claims requiring sources are marked
- whether sensitive information has been removed or anonymized
- whether restoration instructions are understandable

## How to Restore in Another AI System

To restore the package in another AI system:

1. Upload or provide the required package files.
2. Instruct the AI to read the files before making recommendations.
3. Ask the AI to summarize the active context and judgment principles.
4. Ask the AI to identify missing or outdated information.
5. Confirm which decisions remain active.
6. Confirm which authority boundaries apply.
7. Ask the AI to proceed only after clarifying unresolved issues.

Suggested restoration prompt:

```text
You are assisting with a Cognitive Asset Package. First read the provided package files. Summarize the project context, judgment principles, decision history, authority boundaries, unresolved risks, and collaboration protocol. Do not make recommendations until you identify any missing context and ask necessary clarification questions.
```

## Final Export Review

Before completing export, confirm:

- the package contains no credentials
- sensitive information has been removed or anonymized
- review status is visible
- core files are complete enough for restoration
- AI authority boundaries are clear
- unresolved risks are marked
- the package can be understood without the original chat platform
