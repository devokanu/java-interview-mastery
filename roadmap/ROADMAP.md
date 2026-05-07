# Roadmap

## Priority Order

### 1. Banking-Grade Correctness Foundations

- Spring transaction management
- Isolation levels
- Rollback rules
- Optimistic and pessimistic locking
- Idempotency
- Retry safety
- Audit logs
- Outbox pattern
- Consistency boundaries

Why first: banking systems fail expensively when correctness is weak. Senior engineers are expected to protect money movement, customer trust, auditability, and operational stability before discussing scale.

### 2. Core Java Depth

- JVM memory model
- Collections internals
- Generics
- Exceptions
- Immutability
- Concurrency primitives
- Thread lifecycle
- Executors
- CompletableFuture
- Virtual threads
- GC behavior
- Performance profiling

### 3. Spring and Spring Boot Senior Topics

- Bean lifecycle
- Dependency injection design
- AOP and proxy behavior
- `@Transactional` internals
- Validation
- Configuration
- Security
- Observability
- Testing slices
- Auto-configuration

### 4. Database and Persistence

- SQL fundamentals at senior level
- Indexing and query plans
- JPA/Hibernate internals
- Lazy loading
- N+1 queries
- Dirty checking
- Locking
- Connection pooling
- Migration strategy

### 5. Distributed Systems

- Synchronous vs asynchronous communication
- Messaging
- Event-driven architecture
- Saga
- Outbox/inbox
- Exactly-once myth
- At-least-once delivery
- Circuit breaker
- Timeout, retry, bulkhead
- Backpressure

### 6. Banking Domain Architecture

- Payment flows
- Ledger concepts
- Core banking integration
- Reconciliation
- Fraud checks
- KYC/AML awareness
- Auditability
- Regulatory reporting
- Operational risk

### 7. Security

- OAuth2/OIDC
- JWT trade-offs
- mTLS
- Secrets management
- OWASP
- Data encryption
- PII protection
- Authorization models
- Secure logging

### 8. System Design and Architecture

- Modular monolith vs microservices
- Clean architecture
- Hexagonal architecture
- DDD tactical patterns
- API design
- Resilience
- Scalability
- Reliability
- Architecture decision records

### 9. Testing and Delivery

- Unit, integration, contract, E2E testing
- Testcontainers
- Mutation testing
- CI/CD
- Blue-green/canary releases
- Feature flags
- Rollback strategy

### 10. Interview Practice Tracks

- Scenario-based questions
- Live coding
- Debugging
- LeetCode-style algorithms
- Multiple-choice screening tests
- Fill-in-the-blank questions
- True/false questions
- TestGorilla-style English questions
- Architecture decision exercises

## First Mock Interview Topic

Spring transaction management in a banking money-transfer scenario.

Core interview target:

Can the candidate reason about transaction boundaries, rollback behavior, isolation, concurrency, auditability, and production failure impact?
