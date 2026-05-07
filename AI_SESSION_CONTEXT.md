# AI Session Context

Last updated: 2026-05-07

## Overall Goal

Prepare for Senior Java Developer, Senior Backend Developer, Software Architect, and similar Java/Spring roles requiring 10+ years of experience, with an early focus on banking-domain interviews.

The process is mock-interview driven:

1. Ask a question first.
2. Let the learner answer.
3. Analyze the answer.
4. Identify gaps.
5. Explain deeply at Senior/Architect level.
6. Produce/update required learning artifacts.

## Mandatory Language Rule

Main explanations must be in Turkish.

Interview questions, model answers, test questions, English practice, and important technical terminology must also include English versions.

## Current Phase

Phase 1: Foundation for banking-grade backend engineering.

Current first mock interview topic:

Spring transaction management in a banking money-transfer scenario: `@Transactional`, rollback rules, isolation, consistency, and operational risk.

## Current Priority

Build Senior/Architect thinking around correctness before scale:

- Transaction correctness
- Concurrency safety
- Idempotency
- Database locking
- Auditability
- Failure handling
- Security and regulatory awareness

## Known Learner Preference

The learner wants visual support for every topic:

- Mermaid flowchart
- Single-file JavaScript animation in `animations/index.html`

The learner also wants runnable IntelliJ code labs during PC/Codex work.

## Updated Artifact Preferences

- Anki must be created as separate versioned files per topic/checkpoint, not one continuously growing file.
- `animations/index.html` must use mostly Turkish explanations, slower animation timing, and beginner-friendly term explanations inside the visual.
- `animations/index.html` must be button-controlled instead of auto-playing and should include light/dark mode support.

## Required Outputs Per Topic

- Mock interview question
- Learner answer analysis
- Gap identification
- Senior/Architect-level explanation
- Banking-domain connection
- Trade-off analysis
- Mermaid flowchart
- Topic-specific animation inside `animations/index.html`
- IntelliJ-runnable code lab when on PC/Codex
- Incorrect and correct code examples
- Debugging scenario
- Anki flashcards
- Turkish Q&A
- English Q&A
- TestGorilla-style questions
- Topic progress record
- Missing work checklist

## Latest Learner Answer

The learner answered that they do not know how to answer the first Spring transaction banking-transfer mock question.

## Current Gap

Critical gap: transaction boundary, rollback behavior, isolation, concurrent transfer risk, and external side-effect handling are not yet understood.

## Next Step

Teach Spring transaction management from a concrete banking transfer scenario, then ask a smaller follow-up question to verify understanding.
