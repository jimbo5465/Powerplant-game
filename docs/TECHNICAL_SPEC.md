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

## Security
Do not include real plant layout, real control procedures, sensitive parameters or site security information.

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
