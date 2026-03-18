# ExecutionPolicy_Wrapper_Policy_Patch__v1

## Policy Decision
Do not assume direct invocation of local .ps1 helpers will succeed.

## Default Rule
For local helper rails, prefer process-scoped wrapper execution:
- pwsh/powershell
- -NoProfile
- -ExecutionPolicy Bypass
- -File <helper>

Do not default to machine-wide execution policy changes.

## Readiness Rule
A helper is not ready merely because:
- path exists
- file exists
- file was written successfully

A helper is ready only when it is proven callable through the intended host/wrapper path.

## Local Helper Readiness Ladder
1. path exists
2. folder writable
3. config/schema present
4. helper file written
5. helper callable through intended wrapper
6. helper returns expected output

Only then:
STATE=local_helper_ready

## Why
This prevents false-green waves caused by:
- execution policy blocking
- direct invocation assumptions
- file existence mistaken for operational readiness

## Applies To
- CoLowKey resolver pattern
- CoStacks execution helper
- pregate/preflight
- watcher/pushback rails
- ACTION-last execution receipts

UTC=20260318T223613Z