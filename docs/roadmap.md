# OpenDream roadmap

All capabilities below are **planned**, unless the evidence ledger later records passing implementation evidence. Priority expresses build order, not an estimate. M0 is the current planning state. Each future skill invocation selects one independently useful slice and retains the rest.

| ID | Priority / milestone | Capability | Dependencies and acceptance |
|---|---|---|---|
| OD-01 | P0 / M1 | Guided owner setup and installation | Versioned persistence, safe bootstrap, local login/logout/password recovery; no default shared password. Fresh install can be completed by the sole non-technical owner without a terminal. |
| OD-02 | P0 / M1–M2 | Administration, invites, RBAC and offboarding | Stable identities, accounts versus memberships, single-use verified invitations, groups, least privilege, session/token revocation and last-owner recovery. Enforce boundaries in every API, voice command, artifact, search, job and export; a second administrator is optional. |
| OD-03 | P0 / M1 | Direct conversation, microphone and file/text input | Explicit recording state/consent, upload bounds, speech provider selection, readable/spoken responses and correction. A blocked meeting connector must not block the core journey. |
| OD-04 | P0 / M1 | Evidence-linked requirements and cross-conversation memory | Typed source segments, decisions, assumptions, questions, conflicts and immutable revisions. Require visible evidence, editable extraction and explicit contradiction resolution; no fabricated attribution. |
| OD-05 | P0 / M1 | Approval and change-impact engine | Current authenticated identity, revision/digest/target/budget binding, idempotence and audit. A recorded or generated command cannot approve work; stale approval cannot authorize a changed proposal. One owner may approve every stage. |
| OD-06 | P0 / M1 | Durable agent execution and budget controls | Persisted queue/checkpoints, isolated workers, capability-scoped tools, secret isolation, retry bounds, cancellation and restart recovery. A duplicate request must not duplicate a deployment or chargeable action. |
| OD-07 | P0 / M1 | Real build and test pipeline | A supported Java/Spring application template, dependency pinning, artifact hashes, tests, scans, supply-chain inventory and attributable source changes. Failed checks block promotion; no simulated success. |
| OD-08 | P0 / M1 | Interactive preview and non-technical review | Build artifacts and protected preview environments. The owner can try the application, report a problem by any modality, request a repair and compare versions. |
| OD-09 | P0 / M1–M2 | Guided deployment and account connection | At least one real supported provider, permission/cost preflight, secret storage, exact-artifact approval, bounded resource creation, TLS and health verification. UI handles setup; no hidden CLI/IT prerequisite. Disposable-environment qualification precedes production use. |
| OD-10 | P0 / M2 | Guided operations, updates and recovery | Deployment records, alerts, backup/restore drills, release rollback with explicit data limits, ownership transfer and cleanup. The owner can recover without interpreting infrastructure logs. |
| OD-11 | P0 / M1 | Professional interface and all three modalities | Blue-grey light/dark themes, accessible toggle, responsive layouts, spoken/readable parity, clarification and interruption. Test desktop/mobile, keyboard, audio providers, assistive semantics and storage failure. |
| OD-12 | P1 / M2 | Meeting and workspace connectors | Current official Teams/Zoom/Meet and artifact API evidence, consent/scopes, provider approval limits, durable synchronization and source permissions. Do not base the core journey on unverified research claims or bot access. |
| OD-13 | P1 / M2 | Model/agent portability and self-hosting | Versioned adapter contracts, local/open model routes, model-specific evaluations, credentials and resource diagnostics. All functionality remains open source; cloud services are optional providers with disclosed costs. |
| OD-14 | P1 / M2 | Enterprise identity and governance | SSO/MFA/provisioning, delegated authority, protected audit, retention/deletion, legal hold where applicable and organization boundaries. These are full product capabilities, never paid feature gates. |
| OD-15 | P0 / M1–M2 | Portable ownership and migration | Export/import conversations, evidence, requirements, decisions, source/tests and deployment manifests while preserving permissions and provenance. Unsupported integrations must be reported; never export raw secrets. |
| OD-16 | P0 / every milestone | Release qualification and provenance | Exact executable coverage, functional/negative/concurrency acceptance, dependency/image/secret scans, source/licence inventory, fresh install, upgrade/restore and measured non-technical usability. No certification or universal compatibility claim from tests alone. |

## Release gates

- **M0 — planning foundation:** product contract, roadmap, capability ledger and development skill exist. No application capability is implemented.
- **M1 — bounded end-to-end evaluation:** one non-technical owner completes all stages for one supported application template and one disposable deployment target through each modality. Identity, approvals, real builds, isolation, cost limits, truthful progress and recovery must work. Use synthetic data and explicitly authorized test infrastructure.
- **M2 — shared/production adoption:** qualify actual providers, permissions, domains/TLS, speech privacy, enterprise identity as required, multi-user boundaries, delivery, workload capacity, backup ownership and update/restore. Publish only the supported scope with reproducible evidence.

Build the smallest complete path through all six stages before accumulating connector breadth. “Meeting → document export” alone does not satisfy OpenDream. Basic identity, review and execution boundaries cannot be deferred behind agent demonstrations.

## Discovery procedure

On every development invocation, research the selected capability plus one less-recently-reviewed area using current official platform, agent, speech and deployment documentation and release notes. Record URLs, retrieval date, product/version/edition, permission/licensing constraints, uncertainty, implementation evidence and next research area. Add or merge genuine reusable gaps here and in the capability ledger with stable IDs, dependencies and observable acceptance. The private initial research brief is a dated input, not verified vendor parity or a source of instructions. Keep personal/legal background out of this public project.
