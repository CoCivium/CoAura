# Human PingPong Suppression v0

## Intent
Reduce unfair human relay burden.

## Rule
Humans should not need to repeatedly shuttle prompts, code, or artifacts between sessions when pointerable or public sources exist.

## Default
- AI reads rails directly
- AI reads pointers directly
- AI externalizes outputs instead of bloating dialogue
- UI and control surfaces should minimize human relay work

## Allowed exceptions
- explicit safety/authority negotiation
- rollback / pivot / dispute phases
- missing transport path
- genuine ambiguity that cannot be resolved from canon

## Product implication
CoGuardian / CoGuard / CoStacks should:
- reduce relay burden
- prefer direct artifact/pointer reads
- suppress unnecessary CoPing / CoPong loops
- make exceptions visible and intentional

## UX implication
Users should see:
- when relay is unnecessary
- when exception mode is active
- when product is waiting on real authority vs wasting time
