# OpenDream

From a conversation to working software, guided by one person.

OpenDream is an OpenSoft project for turning ideas and conversations into reviewed requirements, agent-built applications, previews and deployments. A single non-technical person must be able to complete the journey using voice, mouse or keyboard. No developer, terminal, source-code editor or separate IT operator should be required for the supported journey.

**Status: planning foundation.** This repository currently contains the product contract, build plan and evidence ledger. There is no runnable application, speech integration, coding agent or deployment connector yet. Those capabilities must be implemented and demonstrated before being advertised as available.

The intended journey is **Describe → Plan → Build → Try → Release → Improve**. OpenDream explains the next decision in ordinary language, presents a working preview, and asks for approval of the specific version, destination and cost before publishing. The same person can approve every stage; a team is optional.

Every requirement should retain its evidence: a conversation segment or the owner's explicit decision. That trail continues through the approved specification, agent task, test, source revision, build and release. When a decision changes, OpenDream identifies the affected work and asks for fresh approval where needed.

All product features are intended to remain fully open source under [Apache 2.0](LICENSE), including administration, security, voice, enterprise integration and deployment controls. Consulting and support are optional services, not prerequisites or feature unlocks. External cloud/model costs must be shown before the user authorizes them; local providers and portable exports are required roadmap items.

- [Product contract and acceptance journey](docs/product-contract.md)
- [Roadmap and release gates](docs/roadmap.md)
- [Capability evidence ledger](docs/capabilities.md)
- [Architecture and execution boundaries](docs/architecture.md)
- [Professional appearance and multimodal experience](docs/product-experience.md)

The development skill is `$open-dream`, maintained in OpenSoft's private skills repository. It implements one bounded capability at a time, researches current public capabilities, requires acceptance tests and exact coverage, and commits locally without publishing. The application stack must use the latest mutually compatible stable Java and Spring Boot releases; verify current releases when implementation begins. Build/deployment targets for generated applications must be explicitly supported and tested, not assumed from the orchestration stack.

## AI product direction

Requirement added 2026-11-16: OpenDream must become fully AI enabled, agentic and conversational across its core journeys. The [AI capability and acceptance guide](docs/ai-capabilities.md) defines the required work and evidence. This direction does not change the implementation scope or historical validation results recorded above.
