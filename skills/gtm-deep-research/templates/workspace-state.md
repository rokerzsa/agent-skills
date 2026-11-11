# Workspace State — allocation and compatibility

> **Template only**; single-writer counters. Never reset after allocation has begun.

| Field | Value |
|---|---|
| Workspace ID | `{{WORKSPACE_ID}}` |
| Convention version | `{{CONVENTION_VERSION}}` |
| Last issued project number | `0` (initial value only) |
| Last issued concept number | `0` (initial value only) |
| Unresolved recovery | `none` (initial value only) |

## Allocation invariants

- Persist counter increment **before** creating the record; issued numbers remain spent even after a failed write.
- On restart, compare counters against records and any allocation journal; if inconsistent, halt and reconcile without issuing duplicates.
- Do not claim concurrency safety or atomic multi-file commits.
