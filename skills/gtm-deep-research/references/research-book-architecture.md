# Markdown-first OKF research book architecture

[Book home](../book/index.md) · [Chapter 11](../book/part-04-outputs-lifecycle/11-book-architecture-and-navigation.md) · [Synthesis](research-synthesis-and-lessons.md) · [Index template](../templates/research-book-index.md) · [Chapter template](../templates/research-book-chapter.md)

**Output contract:** Every full GTM research project's reader-facing deliverable is a coherent, navigable **Markdown-first OKF book**. Docusaurus-*style* describes logical parts, chapters, category indexes, stable links and reader navigation; no Node.js build, website, sidebars configuration or duplicated publishing source is mandatory. The underlying evidence/semantic records remain authoritative for knowledge; the book is its readable derived presentation.

## 1. Obtain and respect the approved book plan

- Read the research charter's intended audience, coverage, deliverables and high-level book outline before creating a draft book.
- Material top-level chapter additions/removals/reordering, central narrative reframing and changed scope require a **human-approved charter/plan amendment** where consequential (DR-051). Codex may refine section titles, split overlong sections, move supporting passages and maintain indexes within the approved outline.
- A project's topics determine its organization; do not force the GTM example outline onto every subject or mistake the skill specification book's 14 chapters for the company's research book.
- The initial book may be incrementally developed during authorized investigation; distinguish **draft** from final completion. Completion is decided solely by the separate [contract/charter completion audit](completion-and-acceptance.md).

## 2. Required navigational surfaces

At minimum create or maintain the following as useful and warranted by the charter:

1. **Main `book/index.md`:** title, audience, research scope, confidence/review caveat, how-to-read guidance, current draft/revision state and ordered links to parts/chapters.
2. **Part/category indexes** for substantive collections: short framing, ordered chapter links, relevant neighboring parts, and semantic topic links.
3. **Chapters:** concise purpose, subject/timeframe, sections in logical reading order, evidence-linked findings, contradictions/limitations, related topics, and previous/next/back-to-index navigation.
4. **Reference appendices:** topic/concept index, chronological timeline, source/claim references, glossary, unresolved gaps and significant revision history **when useful**; link to authoritative registries instead of copying them.
5. **Cross-chapter semantic links** to the concepts or mechanisms they discuss; maintain a distinct logical *reading order* vs semantic *knowledge network*.

Use relative Markdown links with stable document targets plus canonical IDs for records; file location alone is not a stable `K`/`CLM`/`SRC` identity. Maintain lightweight ID→current-file/anchor lookup as records move or split.

## 3. Preferred minimal on-disk book structure (illustrative, not a fixed taxonomy)

```text
projects/<PRJ_ID-or-slug>/book/
  index.md
  part-01-<semantic-name>/
    index.md
    01-<chapter-name>.md
    02-<chapter-name>.md
  part-02-<semantic-name>/
    index.md
    03-<chapter-name>.md
  appendices/
    topic-and-concept-index.md
    evidence-and-limitations.md
    revisions.md
```

Create folders and supporting indexes only when actual content warrants them; do not create blank placeholders as though research existed. An individual shorter project can use a flat chapter collection while preserving navigability.

## 4. Authoring a chapter

1. Define the chapter's role and mandatory questions from the charter/plan; identify current `K`/qualified `CLM`/`SRC` evidence and required `RT` review status.
2. Put reader-oriented explanation first; place short citations near material claims rather than dumping raw source entries into prose.
3. Clearly distinguish **fact**, **reported account**, **inference**, **causal model**, **transferable hypothesis**; mark disputed, unverified or pending major review as appropriate.
4. Use meaningful headings, manageable sections, tables/timelines only when they clarify, and coherent chapter transitions.
5. Include a concise "Evidence and limitations" passage for consequential uncertainties; link to the exact underlying records, both supporting and contradicting.
6. Include links to next/previous chapters and semantic neighboring topics; keep links resolvable after edits.
7. Keep the narrative clean: journals, `RT` investigation notes, budget events and raw registry records are references, not the structure of the book.

## 5. Index maintenance and link integrity

When creating, splitting, moving or renaming a chapter:

- Preserve `K`, `SRC`, `CLM`, `RT` and design-decision identities; moving a Markdown file **never** reallocates a record ID.
- Update main and part table-of-contents links and relevant previous/next pointers.
- Update inbound chapter links and the stable ID-to-location lookup for any moved operational record.
- Run a local link/anchor check where possible; if a link cannot be resolved, record the limitation before checkpoint advancement.
- For a consequential new top-level hierarchy or change of central thesis, propose approval **before** applying the structural change; correcting underlying false evidence should not wait for cosmetic approval.
- Keep significant prior chapter versions via [revision protocol](synthesis-revisions.md), not unnecessary whole-book snapshots on every edit.

## 6. Semantic and operational separation

A semantic `K-...` concept may be referenced by several books/projects. The canonical concept's ID and evidence relationships stay in the workspace knowledge layer; a chapter's prose need not be duplicated into the concept record. Cross-project use requires contextual revalidation. A chapter does not become a new source citation merely by summarizing another chapter.

## 7. Book quality check

- [ ] Main book index clearly communicates audience, scope, current **draft** status and reading order.
- [ ] All existing parts and chapters appear in the appropriate indexes and support navigation.
- [ ] Each material conclusion is linked to traceable underlying evidence and review states.
- [ ] Major unresolved contradictions and qualifications are visible in relevant chapters.
- [ ] Introductory context precedes complex causal interpretations; topics are semantically grouped.
- [ ] Terminology is consistent; first user vs first customer, list price vs realized revenue, observation vs causation are distinguished.
- [ ] Relative links resolve, and stable canonical record IDs survive chapter changes.
- [ ] No operational journal is presented as a reader-facing chapter substitute.
- [ ] No Docusaurus build, live workspace, complete research project, or finalized release is claimed by the template alone.

Full project completion and reopening follow their [separate completion](completion-and-acceptance.md) and [dependency/reopening](dependency-impact-and-reopening.md) procedures; final external publication requires any applicable human authorization. Passing draft-book quality checks does not establish completion.
