# Capability evidence ledger

Baseline: 15 November 2026. **M0 only: planning foundation.** No production source, runnable service, agent execution, speech provider or deployment integration has been implemented. Application test coverage is unavailable; there is no executable application scope to measure yet.

The [roadmap](roadmap.md) defines OD-01–OD-16. Every one is currently planned. The [product contract](product-contract.md) defines the owner's acceptance journey and takes precedence over recommendations in the private research input. OpenDream is product-native: no single commercial product or API is pinned as a compatibility target.

| Evidence | Status | Limit |
|---|---|---|
| Product and modality contract | Documented | No runtime or usability qualification yet. |
| Architecture and execution boundaries | Proposed | Must be validated through implemented vertical slices. |
| Local development skill | Prepared in private skills repository | Skill validation is not application testing. |
| Current application stack | Required, not implemented | Latest compatible GA Java/Spring Boot must be verified at implementation; no package or container exists yet. |
| Third-party connectors, speech, agents and deployment providers | Unverified | The initial brief's dates, licences, prices, permissions and availability require current primary-source verification. |
| Non-technical end-to-end journey | Missing | No engineer-assisted demo can establish this requirement. |

For each future slice record: stable gap ID; fixed review base; exact contract; evidence URLs/retrieval scope; selected alternatives; affected production files; test commands/counts; exact line/branch/method or function counters; review findings and repairs; migration/operational evidence; local commit; remaining limits and next research area. Only mark a slice implemented after its acceptance and exact coverage gates pass.

New implementation must preserve public-source provenance, upstream notices and legitimate imported material. There is no legal clean-room certification or trademark clearance in this planning ledger. No private background from the research brief is included here.

## Required AI, agent and conversational delivery — OD-AI-001–005

Owner direction added 2026-11-16: fully AI-enabled core journeys, contextual conversational support and agents that complete permitted work are required product capabilities. Follow the [AI acceptance contract](ai-capabilities.md) and its five backlog dimensions: conversation, assistance, scoped actions, reliable/governed execution and measured outcomes.

**Status:** Planned: this is a documentation-only foundation with no runnable AI, speech, agent or deployment application. These requirements refine OD-03 through OD-16; they do not replace the complete owner journey or establish feature availability.

Prioritize a complete supported journey with identity, source permissions, typed APIs and execution controls in place. Record implementation evidence and acceptance results per slice; a summary endpoint, conversation store or documentation change does not complete the parent requirement. Keep these items visible alongside other release blockers.
