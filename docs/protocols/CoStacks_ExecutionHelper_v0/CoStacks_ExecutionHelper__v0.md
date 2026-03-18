# CoStacks_ExecutionHelper__v0

## Purpose
Define the thin execution-helper rail for CoStacks.

## Core Rule
CoStacks is the cognition/orchestration layer.
Execution helpers perform local mutations.
Helpers must remain thin, headless-default, swappable, and subordinate to rails.

## Required Inputs
- intent
- bounded target
- authority prerequisites
- local secret pointer or alias (never raw secret in chat)
- engine selection if needed

## Required Prechecks
1. CoFirePiss authority degrade check
2. local prereq/pregate check
3. path/repo/tool validation
4. secret availability via CoLowKey local resolver only

## Required Outputs
- blocked state OR
- externally readable proof OR
- explicit local-only receipt with degraded state

## Engine Policy
- engine != surface
- Playwright acceptable as OSS headless engine
- browser/control engines must be swappable
- helper remains CLI-first and thin

## Desktop/Mobile Rule
- same backend rails
- different thin-client skins/workflows allowed
- no backend fork for mobile unless explicitly proven necessary

## Secret Rule
- secrets remain local
- sessions reason over path/schema/alias only
- local helper resolves values
- no secret exposure to chat or CoEx

## Relation To Self-Mining
Every meaningful execution wave should externalize:
- proof receipt
- pointer pack
- blocked state
- or compact CoObject

## Minimal Invocation Shape
CoStacks -> thin helper -> local engine/tool -> receipt/proof -> CoPulse

UTC=20260318T215914Z