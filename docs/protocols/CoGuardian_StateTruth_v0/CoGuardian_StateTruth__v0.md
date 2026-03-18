# CoGuardian_StateTruth__v0

## Purpose
Lock authority precedence and state interpretation for CoStacks-era rails.

## Core Rule
If a claimed artifact or state is not directly readable from canonical external surface, it is non-authoritative.

## Truth Precedence
1. RAW + SHA
2. RAW
3. Canonical readable artifact without SHA
4. Payload/body text
5. Lane narration / chat claim

## Authority Degrade
- unreadable = unproven
- unproven cannot elevate state
- reason from last readable proof only

## State Ladder
- bootstrapped
- local_receipt_only
- read_attached
- write_attached
- fully_hitched

## Promotion Rules
- no proof -> bootstrapped or local_receipt_only
- readable proof only -> read_attached
- verified shared write proof -> write_attached
- verified end-to-end shared authority -> fully_hitched

## CoGuardian Role
CoGuardian should enforce:
- proof before promotion
- degrade on unreadability
- no dashboard authority
- no false-green success receipts

UTC=20260318T220159Z