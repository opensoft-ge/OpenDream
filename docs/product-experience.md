# Product experience requirements

Status: planned. OpenDream has no browser interface or voice runtime yet.

Use a restrained blue-grey palette, clear typography and plain-language navigation around Describe, Plan, Build, Try, Release and Improve. Show the current stage, what has been approved, what is happening, expected cost/time, and the next useful action. Avoid presenting Git, YAML, IAM, stack traces or infrastructure consoles as required user steps. Offer technical detail progressively for those who want it.

Provide complete light and dark themes across onboarding, login/recovery, conversations, plans, previews, approvals, administration and errors. The toggle must be visible, labelled, keyboard-operable and persistent; use the system preference until manually overridden and handle unavailable storage. Use semantic colours, visible focus, readable contrast, reduced-motion support and responsive desktop/mobile layouts. Automated accessibility checks supplement manual workflow and visual inspection.

Voice is a full interaction mode with captions/transcripts, spoken summaries, interruption, correction and explicit confirmation. Mouse and keyboard expose the same actions and results. Every command uses the same server authorization and approval rules. Imported audio, background speech and model suggestions cannot authorize actions. Do not assume browser-native speech alone is universally supported, private or offline; qualify actual providers and client combinations.

The owner must be able to ask “What happens next?”, “What will this cost?”, “What changed?”, “Why did it fail?”, “Stop”, and “How do I recover?” at the appropriate stages and receive an actionable explanation. Confirm consequences for the specific build and destination before release. Do not rely on colour, hearing or sight alone to communicate state.

Qualify the [complete acceptance journey](product-contract.md#acceptance-journey) separately in voice-led, mouse-led and keyboard-only modes. Include denied microphone permission, interrupted speech, low confidence, corrections, stale approval, network/provider failures, restart/resume and unavailable storage. Track every technical intervention; an unresolved requirement to ask a developer or IT person blocks the supported no-IT journey.

## AI product direction

Requirement added 2026-11-16: OpenDream must become fully AI enabled, agentic and conversational across its core journeys. The [AI capability and acceptance guide](ai-capabilities.md) defines the required work and evidence. This direction does not change the implementation scope or historical validation results recorded above.
