# Proposed architecture

This is a design direction, not deployed software. Prefer a small Java/Spring Boot control application with durable relational persistence and separately isolated execution workers. Do not introduce a fleet of microservices before a tested end-to-end need exists.

The browser, voice interface and API submit the same typed commands. Authentication, scope checks, current-revision validation, approval evaluation and idempotency happen at the server boundary. Display technical diagnostics as optional detail beneath a plain-language status and next action.

Persist projects, source conversations/segments, extracted proposals, decisions, requirement revisions, specification revisions, approvals, agent runs, jobs/checkpoints, tests, artifacts, deployments and audit events as separate records with stable IDs. Use explicit relationships and append-only revision evidence. Store credentials through a secret interface; business records contain references, never secret values. Record a decision's provenance without claiming a model's reasoning is authoritative evidence.

Provider adapters cover capture, speech-to-text, text-to-speech, models, coding agents, Git/artifact storage and deployment. Pin and validate their supported contracts. API/provider failure must leave a durable retryable or terminal state, with clear limits and a user-facing recovery action. No connector may broaden access beyond the authorized identity or silently export private transcript material.

Execute generated code, dependency installation and repository scripts outside the control application in disposable sandboxes. Bound CPU, memory, duration, filesystem mounts and network destinations. Credentials are task-scoped and expire; deployment privileges belong to the release worker rather than the build worker. Treat repositories, transcripts, tool output and model responses as untrusted input.

Proposed state progression: idea → draft plan → awaiting plan approval → approved plan → queued/running build → tested preview → awaiting release approval → deploying → healthy release. Failed, cancelled, superseded and recovery-needed states are first-class, not success-shaped placeholders. Resuming a run cannot replay a chargeable or irreversible action without reconciling the provider's outcome.

Approval binds to exact inputs, artifact digest, environment, cost ceiling and action scope. The operator sees the relevant change before approving. Revisions that change the approved result invalidate downstream authority. Agents cannot self-approve. Keep a single-owner default; optional enterprise policy can add reviewers later.

Use server-side persistence/migrations and a transactional outbox for long-running work. Choose database and queue implementations at the first runnable slice and record their operating limits. Local preview, disposable-cloud evaluation and production deployments are distinct targets with different evidence gates. Rollback of executable artifacts does not imply reversal of data changes or external effects.
