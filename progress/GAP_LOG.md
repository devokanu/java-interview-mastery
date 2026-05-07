# Gap Log

## 2026-05-07 - Spring Transaction Management For Banking Transfer

Learner answer:

> bu yapıyı bilmiyorum

Identified gap:

The learner does not yet have a working mental model for Spring transaction boundaries, rollback behavior, external side effects, isolation level, and concurrent money movement risk in a banking transfer scenario.

Severity: Critical

Why critical:

In banking systems, weak transaction reasoning can cause incorrect balances, duplicate transfers, missing audit records, inconsistent notifications, and operational incidents.

Correction plan:

Start from the mental model of a transaction as an atomic unit of database truth, then explain `@Transactional`, rollback rules, isolation, locking, outbox, idempotency, and banking auditability through one money-transfer scenario.

## 2026-05-07 - External Side Effects And Rollback

Learner answer:

> bilmiyorum

Question:

Can `@Transactional` roll back an external HTTP call?

Identified gap:

The learner does not yet distinguish between database state controlled by a DB transaction and external side effects such as HTTP calls, SMS, email, or message publishing.

Severity: Critical

Why critical:

In banking systems, sending an irreversible external notification or event before the database transaction commits can create inconsistent customer communication, duplicate operations, audit mismatch, and incident recovery complexity.

Correction plan:

Explain that `@Transactional` can roll back database changes made through the same transactional resource, but it cannot undo external side effects. Introduce outbox pattern as the safer alternative.
