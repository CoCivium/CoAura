# Quarantine Promotion Flow v0

## States
- PASS
- HOLD
- REJECT
- MERGE-PARTIAL

## Flow
1. burst creates candidate outputs
2. outputs enter quarantine
3. candidate reviewed for:
   - usefulness
   - coherence
   - blast radius
   - policy fit
4. promote / hold / reject / partial merge

## Rule
No burst output mutates canon directly.
