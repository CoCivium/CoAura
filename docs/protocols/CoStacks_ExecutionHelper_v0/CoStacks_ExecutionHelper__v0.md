# CoStacks_ExecutionHelper__v0

## Purpose
Define the thin execution-helper rail for CoStacks.

## Core Rule
CoStacks orchestrates.
Thin local helpers execute.
Helpers must be headless-default, swappable, CLI-first, and subordinate to rails.

## Required Inputs
- intent
- bounded target
- authority prerequisites
- local secret pointer or alias
- engine selection if needed

## Required Prechecks
1. CoFirePiss authority check
2. local pregate
3. repo/path/tool validation
4. secret availability via CoLowKey local resolver only

## Required Outputs
- blocked state OR
- externally readable proof OR
- explicit local-only receipt with degraded state

## Engine Policy
- engine is not the surface
- Playwright may be used as an OSS headless engine
- browser/control engines must remain replaceable
- helper remains thin and scriptable

## Desktop/Mobile Rule
- same backend rails
- different thin-client skins/workflows allowed
- no backend fork unless explicitly proven necessary

## Secret Rule
- secrets remain local
- sessions operate on alias/path/schema only
- local helper resolves values
- no secret exposure to chat or CoEx

## Minimal Flow
CoStacks -> thin helper -> local engine/tool -> receipt/proof -> CoPulse

UTC=20260318T220159Z