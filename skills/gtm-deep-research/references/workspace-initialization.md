# First-time standalone OKF workspace initialization

[Back to specification](../book/index.md) · [Workspace conventions](standalone-okf-conventions.md) · [Recovery](recovery-and-consistency.md)

**Scope:** A checklist for **authorized first-time setup**. Reading this file or installing the skill does not grant permission to create or overwrite any workspace. Never create a Goal Memory or `memory temp/` dependency.

## 1. Authorization and preflight

1. Ask for and record the human-approved canonical research root and intended scope. Distinguish an empty new location from an incomplete or inconsistent existing workspace.
2. Check whether the directory already contains an `index.md`, `control/workspace-state.md`, `control/conventions.md`, or other research files. If any existing state is present, **do not reset it**; inspect and follow [recovery](recovery-and-consistency.md) before writes.
3. Confirm no concurrent writer will issue project or concept IDs, and record the approval evidence in the chosen control convention.
4. Agree the pinned convention revision and ID widths. The proposed defaults are `K-000001` for concepts and `PRJ-0001` for projects; `DR-001` is reserved for skill decisions.
5. If the approved hard-budget limits cannot be enforced or no persistent workspace is available, stop affected work; do not create an ad-hoc shadow knowledge base.

## 2. Minimal first-time files

After explicit initialization authorization, create only these initial records, resolving placeholders from real approval and workspace facts:

| Destination within approved root | Source template | Purpose |
|---|---|---|
| `index.md` | [Workspace index](../templates/workspace-index.md) | Root navigation, not a decision ledger |
| `control/workspace-state.md` | [Workspace state](../templates/workspace-state.md) | Stable workspace ID, pinned revision, monotonic project/concept counters |
| `control/conventions.md` | [Workspace conventions](../templates/workspace-conventions.md) | Authoritative local naming, link and recovery rules |
| `knowledge/index.md` | [Knowledge index](../templates/knowledge-index.md) | Empty semantic concept index; no fake concepts |

Do not create a `PRJ-...` project directory or `knowledge/K-...` concept file simply to populate examples. Create a project only after authorization and when actual research context warrants it; the charter and detailed plan have their own separate approval gates.

## 3. Illustrative initial state (not a real created workspace)

```text
root/index.md                       # workspace W-EXAMPLE; approved-root placeholder filled
root/control/workspace-state.md     # last project 0, last concept 0, recovery none
root/control/conventions.md         # approved convention version 1, one writer
root/knowledge/index.md            # empty semantic groups and index
```

`last issued = 0` is valid **only for a genuinely new workspace with no prior IDs**. Never infer zero because existing files are temporarily missing or cannot be inspected.

## 4. Post-initialization validation

- Check all four files exist, root navigation names the actual workspace, and the convention revision and workspace ID agree across the records.
- Verify `index.md` can navigate to the knowledge index and control files once links are populated; avoid leaving rendered broken placeholders.
- Confirm project/concept issuance counters do not contradict existing names or ledgers.
- Record initialization completion only **after** substantive control records and indexes are valid; checkpoint-last principles apply when an active project exists.
- Preserve a brief auditable note about which files were actually created and which checks were performed.

**Not a research start gate:** Successful initialization does not approve a company's research charter, detailed plan, external spending, or contact with third parties.
