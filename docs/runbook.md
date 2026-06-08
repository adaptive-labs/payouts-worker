---
category: runbook
title: Payouts Worker runbook
description: On-call runbook for Payouts Worker.
related_entities:
  - payouts-worker
related_teams:
  - payments
---

# Payouts Worker runbook

On-call guide for `payouts-worker` (Payments, tier high).

## Alerts

- **payouts-worker-high-error-rate** — 5xx over 2% for 5m. Check upstream dependencies.
- **payouts-worker-latency** — p99 over SLO. Check resource saturation.

## Common issues

- **Pod OOMKilled** — check memory limits and recent traffic spikes.
- **Crashloop** — check the last deploy and roll back if needed.

## Escalation

Page the Payments on-call rotation.

