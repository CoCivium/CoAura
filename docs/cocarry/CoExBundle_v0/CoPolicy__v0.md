# CoPolicy v0

State:
- PASS
- HOLD
- REDACT

## Expose Gate (Int)
- PASS: safe to publish
- HOLD: defer, needs review
- REDACT: publish with removals

## Evolve Gate (Ex)
- CoEx~: opportunistic content improvements
- CoEvo: explicit rail/policy/governance changes only
- AutoEvo: automated changes only inside clearly bounded, consented scopes

## Rules
- Default: externalize pointers, not bloated blobs
- Meta changes require explicit CoEvo
- If in doubt: HOLD
- Human relay burden should be minimized by default
