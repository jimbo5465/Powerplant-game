# Technical Specification

**Status:** Draft / Direction selected

## Target
- Platform: Android
- Dimension: 2D
- Engine: Godot
- AI-Assisted / Vibe Coding
- Offline-first
- Persian-only MVP

## Save / Progress
**Local Offline Progress System**

Required:
- Highest unlocked level
- Completed levels
- Stars per level
- Badges
- Character selection
- Final completion state

Behavior:
- Auto Save after level completion
- Resume progress
- Replay completed levels
- Future levels locked

## Audio & Guidance
- Short Persian Voice-over
- Minimal Persian text
- Visual guidance

Voice-over categories:
1. Mission instruction
2. Important HSE message
3. Success / transition

## Android Build & Distribution
1. Export APK
2. Host on company server/infrastructure
3. Send download link to families, potentially via SMS
4. Direct installation

Public Google Play / Myket release is not required for MVP.

## Completion Proof
- Digital Certificate
- Completion/Verification Code

Exact validation method remains open.

## Architecture Direction
- Shared Main/Progress Map
- Independent Level Scenes
- One Main Mechanic per level
- Reusable UI
- Reusable HSE guidance component
- Shared Save/Progress Manager

## AI-Assisted Development

### Candidate: Godot MCP
Use a Godot-compatible Model Context Protocol (MCP) integration to let an AI coding agent interact more directly with the Godot editor/project.

Candidate implementations to evaluate:
- triforge0/godot-mcp
- elfensky/godot-mcp

Potential uses:
- Inspect scene tree and nodes
- Create/edit nodes and scenes
- Edit GDScript
- Run scenes and inspect runtime/debug output
- Capture screenshots or state for AI-assisted iteration
- Reduce manual copy/paste between the AI agent and Godot

**Decision:** Godot MCP is useful but not mandatory. Do not make the project architecture dependent on it. First stabilize the Godot version and initial project structure; then evaluate and connect one MCP implementation as a development-automation layer.

## Security
Do not include real plant layout, real control procedures, sensitive parameters or site security information.

## AI-Assisted QA / Android Testing

### Candidate Tool: Android-UI-Analyser (AUA)
Repository: https://github.com/The-Wordlab/Android-UI-Analyser

**Role in this project:** Candidate for AI-assisted Android UI testing and regression testing after the first playable APK is available.

Potential uses:
- Automated testing of menus, dialogs, buttons and navigation
- Testing save/load and episode unlock flow
- Testing character selection
- Verifying expected Persian UI text
- Re-running regression scenarios after AI-assisted/Vibe Coding changes
- Allowing an AI agent to inspect and interact with the Android build through ADB

Important limitation:
- Godot gameplay elements implemented as sprites, custom Canvas/UI nodes, drag-and-drop interactions or non-standard accessibility elements may not appear reliably in the Android accessibility/view hierarchy.
- In those cases AUA may need screenshot/vision/OCR fallback, which is less deterministic than structured UI inspection.

**Decision:** Do not integrate AUA during the current design/asset phase. Re-evaluate it when the first playable Android APK exists and define a small automated QA suite at that point.

**Current assessment:**
- Game creation value: low (approximately 2/10)
- Post-build Android QA value: high (approximately 8/10)

## Open Technical Topics
- Exact Godot architecture
- Save format details
- Completion Code validation
- Audio production workflow
- APK update/versioning
- Minimum Android version
- Device performance baseline

## Reference
See: [PROJECT_SPEC.md](PROJECT_SPEC.md)
