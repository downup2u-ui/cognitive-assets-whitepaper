# Three Levels of Cognitive Asset Format {.unnumbered}

The Cognitive Assets framework does not require a single technical format at the beginning. Different users and organizations need different levels of structure.

A useful way to think about implementation is to distinguish three levels.

## Level 1: Human-Readable Package {.unnumbered}

Format:
Markdown files, folders, diagrams, checklists, decision logs, and failure records.

Best for:

- individuals
- writers
- researchers
- founders
- small teams
- early-stage projects

Strengths:

- easy to create
- easy to inspect
- easy to version with Git
- readable by humans
- usable by AI systems through context upload or retrieval

Limitations:

- limited validation
- limited automation
- depends on user discipline
- may become inconsistent without review

Level 1 is the recommended starting point because it preserves human ownership and low friction.

## Level 2: Structured Machine-Readable Package {.unnumbered}

Format:
Markdown plus YAML front matter, JSON, CSV, SQLite, or structured metadata.

Best for:

- multi-project systems
- AI migration workflows
- automated retrieval
- version tracking
- team collaboration
- repeated decision workflows

Possible structured fields:

- `asset_id`
- `project_id`
- `status`
- `owner`
- `last_reviewed`
- `confidence`
- `source_type`
- `authority_status`
- `review_required`
- `related_decisions`
- `related_failures`

Strengths:

- easier to search
- easier to validate
- easier to migrate
- easier to connect to AI retrieval systems
- better suited to automation

Limitations:

- higher maintenance cost
- requires schema design
- can become rigid too early
- may create false confidence if metadata is poorly maintained

Level 2 should emerge after the human-readable package is stable.

## Level 3: Cognitive Asset Infrastructure {.unnumbered}

Format:
Graph databases, semantic retrieval, permission systems, audit trails, review workflows, provenance tracking, and organizational governance.

Best for:

- institutions
- enterprises
- regulated domains
- long-running research programs
- AI-native organizations
- multi-user knowledge environments

Capabilities:

- access control
- review cycles
- source tracing
- relationship mapping
- decision lineage
- failure pattern retrieval
- uncertainty tracking
- portability across systems

Strengths:

- supports organizational scale
- supports governance
- supports auditability
- supports complex retrieval
- can integrate with AI systems directly

Limitations:

- expensive to build
- requires governance
- can become opaque
- may recreate platform lock-in if not designed for export

Level 3 should not replace human judgment authority. It should make judgment continuity easier to inspect, govern, and transfer.

## Recommended Path {.unnumbered}

The recommended path is:

```text
Level 1: Markdown-first package
    ↓
Level 2: Structured metadata and machine-readable records
    ↓
Level 3: Governed cognitive asset infrastructure
```

The mistake would be to begin with heavy infrastructure before the judgment structure is clear.

The safest path is to start simple, preserve the core reasoning, and add structure only when reuse, migration, or governance requires it.

