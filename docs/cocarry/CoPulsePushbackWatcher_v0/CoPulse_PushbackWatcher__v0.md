# CoPulse_PushbackWatcher__v0

## Purpose
Define a minimal watcher/helper pattern that detects and pushes back on session failure modes:
- hesitation loops
- hallucinated execution
- no ACTION section per wave
- orchestration talk without mutation
- stale handoff narration without proof receipts

## Default Rule
Every wave must emit at least one CoPulse.

A CoPulse is any externally visible mutation, such as:
- public/raw artifact
- sha-backed receipt
- verified pointer-pack delta
- compact SideNote/CoPong with actionable state change
- execution test receipt

If no CoPulse exists, the wave is degraded.

## Pushback Triggers
Trigger pushback when any of these occur:
1. two or more consecutive non-mutating waves
2. planning/summarization presented as execution
3. attachment/write claims without RAW verification
4. dashboard language presented as source-of-truth
5. handoff prose exceeds pointer/proof content
6. execution substrate claims without receipt
7. repeated “next step” language without an artifact or DO block

## Pushback Response
When triggered, the watcher should force the lane to do one of:
- emit one bounded artifact
- emit one executable DO block
- emit one proof receipt
- explicitly declare blocked state

## CoPulse Footer Pattern
Minimum footer fields:
- SESSION/LANE
- UTC
- STATE
- ACTION_TAKEN
- POINTER or RECEIPT
- NEXT_SINGLE_MUTATION

## Truth Discipline
- RAW+SHA > RAW > payload text > lane narration
- local-only work is not attached
- dashboards are derived only
- handoffs are degraded fallback unless containment is required

## Terminology Guidance
- use "lane" for session/tool/channel instance
- reserve "being" or equivalent for higher-order continuity
- treat CoTwilight lanes as mutation sources, not truth sources

## Recommended Next Integration
1. fold CoPulse requirement into session-init templates
2. fold pushback triggers into handoff/self-mine packs
3. add one tiny checker helper to local execution substrate later
4. keep this rule lightweight and universal

UTC=20260318T175518Z