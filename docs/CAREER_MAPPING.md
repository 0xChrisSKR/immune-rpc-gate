# Career Mapping

## Project

Immune RPC Gate

## Problem

RPC-dependent products need explicit behavior when upstream state becomes slow, inconsistent, unavailable, or unsafe.

## Role

Reliability model, operating modes, read-only boundary, failover behavior, threat model, and public architecture package.

## Tech Stack

RPC gateway architecture, health checks, failover design, read-only boundaries, API contract design, Web3 infrastructure risk modeling

## Architecture

Client request -> RPC gate -> Health evaluator -> Mode controller -> Read-only boundary -> Upstream RPC providers

## Key Decisions

- Keep public claims verifiable.
- Separate product story, engineering notes, API examples, deployment preview, security notes, and future work.
- Use CI and validation to make the repository reviewable as an engineering artifact.
- Use PNG diagrams for recruiter-friendly first impression and docs for deeper review.

## Engineering Challenges

- Translating private or experimental system work into public-safe artifacts.
- Showing architecture and judgment without exposing runtime internals or private deployment details.
- Making the project legible to AI platform, backend, data, infrastructure, robotics/ROS-adjacent, and overseas engineering reviewers.

## Business Impact

Makes infrastructure failure states understandable and reviewable before they affect product behavior.

## Interview Talking Points

- Why this problem matters.
- What boundaries were required to keep the system safe and reviewable.
- How AI-assisted development was directed and validated.
- What is publicly verifiable and what is intentionally not claimed.
- How this project connects to the broader portfolio ecosystem.
