---
type: Reference
title: Goal memory OKF profile
description: Local rules for private OKF context, navigation, IDs and recovery.
tags: [okf, context, memory]
status: draft
---

# Private OKF profile

This local profile is based on OKF v0.2, not the complete upstream specification. The bundle is memory temp/, private and Git-ignored. Protect it from cleanup; ignore rules do not prevent deletion or untrack files. Never silently commit, export, overwrite or delete it.

Each ordinary Markdown concept has YAML frontmatter with type; use a useful title and description, and focused tags when helpful. OKF status describes knowledge maturity (draft, stable, deprecated), not progress or verification. index.md and log.md are reserved structural files: indexes link concepts with reasons to read them; logs group material changes under dates, newest first. Standard Markdown links express relationships. The upstream concept ID is the bundle-relative path without .md.

Initialize with index.md, log.md, local SPEC.md and HOW-TO-USE.md, plus 001-working-agreement.md, 002-active-state.md and 003-working-patterns.md. The two references are ordinary concepts and local exceptions to numbering. Other concepts receive an immutable bundle-wide numeric prefix. Store last_issued_id in active-state frontmatter; persist the increment before creating a concept, allow gaps and never reuse numbers. Reconcile counter conflicts before allocation. Moving a concept changes its path ID: repair links while retaining its numeric prefix.

For each substantial goal or coherent discussion, create a descriptively named directory within the bundle and an index.md explaining its contents. Link it from the root index and active state. Keep its overall outcome, understanding and provisional plan in a numbered concept within that directory. Give each independently reviewable phase a separate numbered concept there when prepared, linked to the goal and current state. Add subdirectories and indexes when useful. Number concepts across the whole bundle, including nested directories. Keep one authoritative shared concept for shared knowledge and link to it. A material change to shared assumptions may affect linked goals; identify and discuss affected work.

Use optional OKF provenance and trust fields where they help: sources identifies material the concept draws on; generated records its producer and timestamp; verified records an actual confirmation against sources by an identified actor and time; stale_after records a known expiry. Do not infer document verification from an implementation test or a commit. Local phase progress is separate from OKF status, which describes knowledge maturity.

The detailed concept owns agreements, rationale, phase progress and evidence. Active state points to current and paused work and next action; indexes help find context; the log records dated material changes. At checkpoints update detailed evidence first, active state second, then affected indexes and log. Reconcile interrupted updates from evidence. Distinguish proposed, implemented, verified, reviewed, approved and committed; record only events that actually occurred. Preserve earlier decisions and reasons when amending them.

Installed references are initialization templates. Project copies are local snapshots; do not silently overwrite them or erase local agreements. Consult the operating guide for initialization and collaboration.
