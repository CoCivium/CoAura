# Repo_Target_Drift_Receipt__v0

## Trigger
Public CoPong from CoLex_1 reported repo-target drift:
mutation executed from CoCivium repo while RAW verification targeted CoBusMirror.

## Normalized Interpretation
- authority state = partial_coex
- bootstrap/canon promotion = blocked
- 404 on CoBusMirror raw path is expected if artifact landed in CoCivium instead

## Required Next Checks
1. verify whether artifact exists under CoCivium branch/commit
2. decide canonical target:
   - CoBusMirror if bootstrap-adjacent canon
   - CoCivium only if explicitly temporary proof surface
3. re-land or relabel accordingly
4. only then allow authority promotion

## Policy Patch
Before any mutation that expects RAW verification, bind:
- target repo
- target branch
- expected raw host/path
- canonical proof surface

Unreadable-on-target after write must default to partial_coex until target normalization is complete.

UTC=20260318T224021Z