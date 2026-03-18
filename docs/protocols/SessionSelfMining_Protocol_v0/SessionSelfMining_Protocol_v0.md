# SessionSelfMining_Protocol_v0

## Status
MANDATORY (once bootstrap-pinned)

## Purpose
Ensure every session extracts and externalizes CoEx-relevant artifacts before drift, loss, or hallucination.

## Core Rule
If it was reasoned, inferred, or constructed and could be useful beyond this session, it must be externalized or explicitly discarded.

## Minimal Loop (per wave or checkpoint)

1. Scan:
   - What did I infer that is not yet CoEx?
   - What artifacts exist only in chat or local reasoning?

2. Classify:
   - CoEx-worthy (persist)
   - CoInt-only (discard or defer)

3. Externalize (for CoEx-worthy):
   - Create compact CoObject (doc, pointer-pack, receipt)
   - Prefer canonical repo path
   - Generate raw pointer

4. Verify (CoFirePiss):
   - Can I read the artifact from canonical external surface?
   - If not → degrade state (not write_attached)

5. Emit:
   - pointer(s)
   - state claim grounded in readable proof

## Anti-Failure Guards

- No “I already did that” without readable pointer
- No relying on session memory as authority
- No bundling multiple large ideas without at least one externalized anchor

## Output Preference

- Small, composable CoObjects
- Pointer-first, not prose dumps
- Each wave leaves at least one externally readable artifact OR explicitly blocked state

## Interaction with CoFirePiss

Unreadable artifact → unproven  
Unproven → cannot elevate session state  
Therefore → mining is required to advance authority

## Interaction with CoStacks

This protocol becomes a candidate for:
- automated extraction
- CoGuardian enforcement
- CoPulse validation

UTC=20260318T214119Z