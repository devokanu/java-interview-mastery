# Study Rules

## Session Startup Checklist

At the beginning of every new session or new topic, the AI must read:

1. `AI_SESSION_CONTEXT.md`
2. `rules/STUDY_RULES.md`
3. `progress/TOPIC_TRACKER.md`
4. The current topic folder under `topics/`

## Main Study Flow

Use this order:

1. Ask a question first.
2. Wait for the learner's answer.
3. Evaluate the answer honestly but supportively.
4. Identify conceptual gaps.
5. Teach the topic deeply.
6. Connect it to banking-domain reality.
7. Discuss trade-offs and alternatives.
8. Update artifacts.

## Explanation Style

- Main language: Turkish.
- Interview questions and test questions: Turkish and English.
- Explain important technical terms next to the term.
- Teach cause-effect, not memorized facts.
- Assume the learner may have junior-level gaps even in advanced topics.
- Push toward Senior/Architect reasoning.

## Senior/Architect Lens

For every important decision, cover:

- Why this decision is made.
- Alternatives.
- When each option is preferred.
- Costs and risks.
- Impact on performance, security, maintainability, scalability, operational risk.
- Banking-specific concerns: regulation, security, auditability, transaction correctness.

## Mock Interview Rules

- Do not ask five near-identical questions.
- Each question must test a different aspect.
- Prefer real scenarios.
- Prefer banking-domain context when relevant.
- After the learner answers, classify the answer:
  - Strong points
  - Missing points
  - Risky misunderstandings
  - Senior-level additions
  - English interview phrasing

## Visual Rules

Every topic should include:

1. A Mermaid flowchart that explains real flow, decisions, and failure paths.
2. A topic-specific animation inside `animations/index.html`.

Animation quality criteria:

- Must be more than static boxes.
- Must show movement, state change, timing, queues, locks, retries, rollback, propagation, or other topic-specific behavior.
- Must have clear topic headings.
- Must work as a single HTML file.
- Must avoid external dependencies unless necessary.
- Must primarily use Turkish explanations.
- Must move slowly enough for a beginner to follow the sequence.
- Must explain the meaning of technical terms directly in the animation panel.
- English labels may be present only as secondary interview terminology.
- Must not auto-play by default. The learner should be able to move forward and backward with buttons.
- Must include light/dark mode support and remember the selected theme when possible.

## Anki Rules

Do not maintain a single continuously growing Anki file.

Every topic or meaningful learning checkpoint should create a separate versioned Anki import file under `anki/`.

Naming format:

`vNN-topic-slug.tsv`

Examples:

- `v01-spring-transactions-banking.tsv`
- `v02-external-side-effects-outbox.tsv`
- `v03-optimistic-vs-pessimistic-locking.tsv`

Reason:

The learner wants to import Anki material separately by topic and study checkpoint.

Preferred format:

`Front<TAB>Back<TAB>Tags`

Cards should include:

- Turkish Q&A
- English Q&A
- Definitions
- Confusing concepts
- Senior-level tips
- Banking-domain warnings

## Code Lab Rules

During PC/Codex sessions, create runnable IntelliJ-ready labs.

Each lab should include:

- Incorrect example
- Correct example
- Debugging scenario
- Banking-related scenario
- Production impact explanation
- README with run/debug steps

## Mobile Mode

Mobile sessions continue:

- Mock interviews
- Topic explanations
- Q&A
- Tests
- Mermaid diagrams
- Animation content planning
- Notion updates

Mobile sessions do not require:

- Running code labs
- Local repo changes
- IntelliJ debugging

## PC/Codex Mode

PC/Codex sessions must:

- Update local repository
- Complete missing code labs
- Update `animations/index.html`
- Update Anki files
- Sync Notion-derived missing work
- Verify runnable examples where possible

## Do Not Move On Rule

Before moving to a new topic, check:

- Did we analyze the learner's answer?
- Did we document gaps?
- Did we update progress?
- Did we add Anki content?
- Did we update visual/animation material?
- Is the code lab done or marked as missing?
