# Code Labs

This folder will contain IntelliJ-ready Java/Spring labs.

## Planned First Lab

Path:

`code-labs/spring-transaction-banking`

Goal:

Show incorrect and correct implementations of a banking transfer service.

Planned scenarios:

- Missing `@Transactional`
- Wrong rollback expectations for checked exceptions
- Calling external notification inside transaction
- Concurrent transfer race condition
- Correct transaction boundary
- Outbox-based notification
- Optimistic/pessimistic locking comparison
