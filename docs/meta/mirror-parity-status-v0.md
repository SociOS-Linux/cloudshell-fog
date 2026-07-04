# Mirror Parity Status v0 — SociOS-Linux/cloudshell-fog

This document tracks drift between the canonical upstream:
- `SocioProphet/cloudshell-fog`

and the mirror:
- `SociOS-Linux/cloudshell-fog`

## Current finding

The mirror is materially behind the canonical repo.

Confirmed examples of artifacts present on canonical but missing on mirror at the time of this refresh:
- `docs/spec/runtime-isolation-v0.md`
- `deploy/k8s/overlays/k8s-connector-incluster/README.md`

## Why this matters

Without periodic parity refresh, the mirror stops being a trustworthy secondary source for:
- operator guidance
- security posture
- deployment overlays
- implementation-adjacent specifications

## Recommended next actions

1. mirror the merged documentation/spec wave from canonical
2. mirror the k8s connector overlays from canonical
3. mirror the latest control docs (`live status`, `runbooks`, validation workflow) as needed
4. keep future parity checks lightweight but regular

## Working rule

Any agent operating against the mirror should verify whether canonical `main` has advanced before assuming the mirror reflects current project state.
