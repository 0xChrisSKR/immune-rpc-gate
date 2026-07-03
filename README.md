# Immune RPC Gate

![Immune RPC Gate architecture](assets/diagrams/architecture.svg)

Immune RPC Gate is a public-safe architecture showcase for RPC dependency risk, Normal Mode, Degraded Mode, OFF Mode, Read-only Gate, explicit 503 behavior, and platform reliability.

This repository is an engineering showcase. It does not expose implementation details.

## Problem

RPC dependencies can become unstable, slow, unavailable, abusive, or untrusted. AI and product workflows need clear read/write boundaries, degraded modes, and safe response behavior.

## What I Designed

- Normal Mode for healthy RPC behavior.
- Degraded Mode for limited operation under elevated risk.
- OFF Mode for disabling unsafe operations.
- Read-only Gate for constrained non-mutating access.
- Explicit 503 behavior when the system cannot process a request safely.
- Threat model for external dependency risk.

## Architecture

See [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md).

## Public Status

Immune RPC Gate is presented as architecture and research. It does not claim production deployment.
