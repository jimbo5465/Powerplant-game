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


## AI Toolchain

This project uses an explicit AI-assisted production chain so each tool has a defined responsibility and the workflow stays repeatable.

### Core Pilot Toolchain
- **ChatGPT** — game design, episode design, UX/HSE logic, prompts, technical decisions, documentation
- **Nano Banana / Google Flow** — character, environment and game-art asset generation
- **Codex** — GDScript, project structure, refactoring, debugging, repository changes
- **Godot** — gameplay assembly, scenes, UI, animation, save/progress logic, Android build

### Optional / Later-Phase Tools
- **Flow / Veo** — short video-style cutscenes and transitions, not core interactive gameplay
- **Godot MCP** — development automation layer between AI coding agents and Godot
- **Gemini TTS / alternative TTS** — Persian voice-over generation
- **Android-UI-Analyser (AUA) + ADB** — Android UI and regression testing after the first playable APK
- **GitHub** — source control, project documentation and decision history

### Toolchain Rule
Do not introduce a new tool unless it solves a defined problem better than the existing stack. The toolchain is a controlled workflow, not a collection of tools.



## Code Architecture Rule

The codebase must remain **layered, modular and maintainable**.

Required principles:
- Do not concentrate all gameplay logic in one script or one oversized scene.
- Separate responsibilities into focused scripts/components.
- Keep gameplay logic, UI, persistence, audio, HSE guidance and level-specific logic decoupled where practical.
- Prefer reusable components and small interfaces/signals over direct cross-dependencies.
- Keep episode-specific code isolated so changing one episode does not unintentionally affect others.
- Shared systems such as Save/Progress, Audio, HSE prompts and global state should live in clearly defined shared modules.
- Avoid duplicated logic; extract shared behavior only when it is genuinely shared.
- Refactoring for clarity is preferred over accumulating patches in a monolithic file.

**Reason:** The project will be developed iteratively with AI assistance. Modular structure makes debugging, review, replacement and future changes faster and safer.


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
