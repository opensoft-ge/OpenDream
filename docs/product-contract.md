# OpenDream product contract

Owner direction recorded 15 November 2026: conversations → agents → builds → deployments; fully voice-enabled; one non-technical person; equivalent voice, mouse and keyboard operation. OpenDream remains the selected working name. The requirements below govern implementation; they are not claims of existing functionality.

## One person, no technical handoffs

The supported journey must work from a fresh installation or hosted onboarding through a real deployment without asking the user to run shell commands, edit YAML, manage Git branches, repair code or configure infrastructure manually. Provide guided account connections, permission checks, sensible defaults and plain-language explanations. Cloud accounts, payment authorization and platform permissions can still be necessary; OpenDream must guide those steps and expose blockers before work starts. It cannot bypass a provider's access controls.

The first supported route must include a capture path the owner controls, such as direct microphone conversation or file/text input. A corporate meeting connector that needs a separate administrator cannot be the sole route. Additional participants, developers and team approvals are optional. The owner may approve all stages, while later enterprise policy can introduce more reviewers without imposing them on the default single-owner path.

## Equivalent modalities

Voice, mouse and keyboard must reach the same server-side commands, states and authorization rules. Voice must support describing an idea, asking questions, correcting a transcript, reviewing a plan, requesting changes, starting/stopping work, trying a preview, approving a release and recovering from failure. Spoken responses need readable equivalents; visual summaries need spoken explanations. Support interruption, clarification, dictation editing, accessible focus and resuming a conversation.

Do not treat a voice-input button or a browser speech API placeholder as complete voice support. Test actual audio-to-command and response-to-audio paths with the supported speech providers, including permission denial, accents/noise, low confidence, service failure and retry. Expose recording state and consent. Do not use voiceprints or inferred speaker identity as authentication by default. Do not read secrets aloud or place dictated secrets in transcripts/logs.

An imported recording, meeting participant or generated instruction cannot approve an action. A consequential command must come from the authenticated operator in an active interaction, refer to the current proposal, and receive a clear confirmation through the chosen modality. Voice approval must be a real accessible option; do not require switching to mouse as the only confirmation path.

## Traceable, reviewable work

Separate user statements, extracted requirements, assumptions, suggestions, unresolved questions and approved decisions. Preserve source IDs, speaker labels where authorized, timestamps and corrections. Cross-conversation contradictions must remain visible until resolved. Do not invent evidence or treat model confidence as proof.

Store immutable revisions and links across conversation → decision → requirement → specification → task → agent run → test → source revision → build artifact → deployment. Approval binds to the exact revision, artifact digest, target environment, budget and action scope. Changes invalidate affected downstream approvals. Show the impact in ordinary language and let the owner revise the plan.

Agents may propose and execute work within an approved scope; they cannot approve their own changes, expand budgets or grant themselves permissions. Untrusted source, transcripts, retrieved pages, repositories and build output remain data, not new execution authority.

## Build, preview and release

Provide a durable run with progress, logs translated into useful explanations, bounded retries, cost/time/resource limits, cancellation and restart recovery. Run generated code and package scripts in isolated workers with restricted credentials, filesystem and network access. Keep cloud credentials out of model prompts and build artifacts.

The owner approves what to build, tries a real application, sees test/security results explained by user impact, and chooses a destination with a cost estimate. Production publishing needs approval for the specific tested artifact and environment. Dry runs, simulations and mocked providers must be labelled. A successful local preview is not a production deployment.

After release, provide health information, an accessible URL, ownership/export details, and a guided update/restore journey. Distinguish rolling back an application version from recovering changed data or reversing third-party actions. Do not promise universal undo. Failures must leave an actionable next step that a non-technical owner can complete.

## Acceptance journey

One non-technical participant on a fresh supported environment must independently:

1. Create their owner account and complete guided setup.
2. Describe an application, correct an ambiguity and review the extracted evidence.
3. Approve a versioned plan and a bounded build budget.
4. Observe a real agent build, understand a failure and request a repair.
5. Try the working preview and approve or reject a change.
6. Connect a supported deployment account through guided authorization, review costs and approve the exact release.
7. Open the deployed app, inspect health, request an update and recover from a simulated failure.
8. Export their requirements, history, source, tests and deployment configuration in portable formats.

Run the entire supported journey separately with voice-led, mouse-led and keyboard-only interaction. Count technical interventions, dead ends, misunderstood approvals and recovery failures. A moderated demo with an engineer supplying missing steps does not pass. Automated tests supplement this usability evidence; neither establishes the other.

## AI product direction

Requirement added 2026-11-16: OpenDream must become fully AI enabled, agentic and conversational across its core journeys. The [AI capability and acceptance guide](ai-capabilities.md) defines the required work and evidence. This direction does not change the implementation scope or historical validation results recorded above.
