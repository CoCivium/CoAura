# CoPrime Twilight Self-Mine Pack v1

## Purpose
Compact successor pack for final convergence work. Pointer-first, no prose dump.

## Current verified truths
- First real CoBus write_attached proof exists
- Dashboard must remain derived from canonical pointers only
- Execution substrate gap has been externalized
- Canonical writable CoBus presence path + verification gates now exist publicly
- Manual handoffs are degraded fallback only

## Critical pointers already public

### Writable CoBus publish contract
https://raw.githubusercontent.com/CoCivium/CoBusMirror/dd5155722f83e4679beaa5c5b565b9d5e8570b2c/docs/COBUS_LITE/presence/PRESENCE_INDEX__LATEST.md

### First verified write_attached proof
https://raw.githubusercontent.com/CoCivium/CoBusMirror/1171c58ce7a394e91236f6d537861299b51f7881/docs/COBUS_LITE/presence/ENTRYPAYLOAD__AUTO_20260318T162008Z.md

### Dashboard derived-only correction
https://raw.githubusercontent.com/CoCivium/CoAura/b3f950c0cac634f6568a6abeebeecdf48b262028/docs/cocarry/DashboardDerivationCorrection_v0/00__INDEX.txt

### Execution substrate correction
https://raw.githubusercontent.com/CoCivium/CoAura/ed5dfaf50d53bd933c811924336af9f4167edae4/docs/cocarry/ExecutionSubstrateCorrection_v0/00__INDEX.txt

### CoPath framing bundle
https://raw.githubusercontent.com/CoCivium/CoAura/10f325b557686b5b7c467a2ac8ea64e04fed449e/docs/cocarry/CoPathBundle_v0/00__INDEX.txt

## Highest-priority remaining gaps
1. CoGoAll / CoBeacon must expose the writable publish contract directly
2. CoBridge v0 exists locally but still needs proof receipts externalized
3. CoConductor must be protocol, not a session
4. CoGuardian truth rail and CoStacks execution-helper rail still need standalone artifacts
5. Bootstrap truth is lagging Mar-18 operating truth

## Required next artifacts, in order
1. SessionSelfMining_Protocol_v0
2. CoGoAll_WritablePublishContract_v0
3. CoConductor_Protocol_v0
4. CoBridge_TestReceipt_v0
5. CoGuardian_StateTruth_v0
6. CoStacks_ExecutionHelper_v0

## Hard rules for successor
- No expansion, only convergence
- No new concepts unless strictly required
- One mutation per artifact
- Pointer-first public/raw only
- Prefer proof receipts over explanations
- Dashboard/UI optional and derived
- Sessions are staging; external artifacts are truth

## Policy/helper/rail deltas inferred
- Bootstrap must expose publish contract, not only read rails
- Tail-safe MegaWave policy is now mandatory
- Attach claims must be normalized against public verification
- Local execution bridge is now the main bottleneck
- Spare capacity should go to bounded external-first AutoEvo only when proof-producing
- Twilight sessions should emit compact self-mine packs by default

## WAVE
- WAVE_ID: CoPrime_Twilight_SelfMine_Pack_v1__20260318T172807Z
- UTC: 20260318T172807Z
