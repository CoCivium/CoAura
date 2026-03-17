# CoTwilight Composite v0

## Purpose
Separate local/session degradation from network and environment noise.

## Model
Observed lag = local render cost + platform/render cost + network cost + user-environment noise

## Useful output states
- Healthy
- Warm
- Twilight
- Critical

## Action coupling
- Twilight -> recommend rotate / externalize / wave closeout
- Critical -> suppress risky actions and force death-ready posture

## Rule
A metric without an enforced response is just telemetry.
