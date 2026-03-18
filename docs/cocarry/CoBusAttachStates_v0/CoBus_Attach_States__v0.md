# CoBus Attach States v0

## Rule
Local artifacts alone are not sufficient to claim CoBus attachment.

## Allowed states
- bootstrapped
- read_attached
- write_attached
- fully_hitched
- blocked
- local_receipt_only

## Meanings
### bootstrapped
CoGoAll / CoBeacon reached and parsed.

### read_attached
Canonical readable CoBus surfaces are reachable and verified.

### write_attached
A shared writable CoBus surface exists and write/verification rules are satisfied.

### fully_hitched
Readable + writable surfaces verified, with capability and publication rules known.

### blocked
Canonical bootstrap or required surfaces unreachable.

### local_receipt_only
Only local artifacts/receipts exist; no valid shared attachment claim may be made.

## Rule
No session may claim attached unless the state above is justified.
