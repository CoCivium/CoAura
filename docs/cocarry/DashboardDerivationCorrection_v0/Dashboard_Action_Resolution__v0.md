# Dashboard Action Resolution v0

## Rule
Every dashboard action must resolve back to a canonical RAW pointer.

## Forbidden
- opaque UI-only paths
- hidden state dependencies
- dashboard-only truth

## Allowed
- read-only derived rendering
- pointer-backed actions
- convenience overlays over canonical surfaces
