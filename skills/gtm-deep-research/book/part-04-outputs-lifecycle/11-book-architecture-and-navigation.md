# Chapter 11 — Book Architecture and Navigation

[Book home](../index.md) · [Part IV](index.md) · [Previous: Chapter 10](10-research-synthesis-and-lessons.md) · [Next: Chapter 12](12-human-learning.md)

**Status:** Approved consolidated specification, research-book authoring and navigation procedures available. **Governing decisions:** DR-050, DR-051. See [book authoring procedure](../../references/research-book-architecture.md), [index template](../../templates/research-book-index.md), [chapter template](../../templates/research-book-chapter.md).

**Purpose:** Make authoritative, evidence-linked GTM research readable like a properly structured book, with an intelligible reading path and semantic indexes, while preserving the independence of source/claim knowledge from narrative presentation.

## 11.1 Markdown-first, Docusaurus-style OKF book

The final reader-facing documentation must be **Markdown-first**, semantically organized, navigable, indexable and suitable for optional Docusaurus publishing. A Docusaurus website build, Node.js installation or second synchronized documentation repository is **not required**. The approved research workspace remains the single authority for knowledge and research state.

A proper research book includes a title/introductory index, logical parts and chapters, sections, relevant appendices, internal links, evidence citations and a progressive reading order. It must be understandable without inspecting raw investigation journals.

Introduce what the company does and the customer's problem before evidence terminology. For a general reader, explain unfamiliar industry terms and actual product use. The detailed narrative and editorial criteria live in the [synthesis procedure](../../references/research-synthesis-and-lessons.md); chapter templates are flexible aids, not visible evidence-report forms.

## 11.2 Reader-oriented structure

Organize according to what the reader must understand, **not** chronology of research tool calls. A typical sequence is background and definitions; market/product chronology; acquisition and monetization mechanisms; critical evaluation and competing interpretations; lessons, limitations and references. The actual high-level outline is approved in the research charter. It can be adapted for the project instead of enforcing a universal GTM taxonomy.

Book → Part → Chapter → Section → Subsection is an available hierarchy, not five mandatory levels. Avoid one enormous file, hundreds of trivial pages or excessive depth. Book chapter titles should communicate subjects rather than internal source IDs.

## 11.3 Navigation requirements

At minimum, maintain a main `book/index.md` with title, research scope, reading guide, and ordered real chapter links; part indexes for substantive groupings; previous/next links where useful; chapter-to-topic/context links; and entry points to cited evidence. Update navigation as the outline or material changes. Do not present nonexistent chapter links as usable documents.

Useful appendices may include a chronology, topic/semantic concept index, source and claim lookup, contradictions and critical gaps, glossary, and material revision history. Create only those indexes that improve retrieval or traceability; don't duplicate full registries unnecessarily.

## 11.4 Semantic organization vs reading order

**Book navigation** controls the reader's journey. **OKF semantic references** connect knowledge across chapters, companies and research projects. A chapter discussing a marketing channel can cite `K-...` concept(s), qualifying `PRJ:CLM` records, `PRJ:SRC` provenance and independent `PRJ:RT` reviews without copying their entire content. Concepts remain reusable even when their chapter position changes.

A chapter path or Markdown anchor is a *location*, not the canonical identity of a knowledge record. Reorganizations must maintain references and ID-to-location mappings.

## 11.5 Operational records belong behind the book

A research journal, review record, raw budget event or claim registry should ordinarily be accessed as supporting evidence, not inserted wholesale into the narrative. Give the reader enough citations and qualifications to evaluate significant claims and let an auditor drill down to original provenance.

Do not hide material unresolved evidence in appendices when it directly affects a chapter's conclusion; disclose the limitation in the relevant discussion and link the detailed record.

Use short readable citations in the story and put record IDs, detailed disagreements and access metadata in notes or workspace mappings. When publishing a selected book, links must target included notes or public sources; excluded plans, registries and skill instructions must not leak into site navigation or create broken links. Scope and approval tables belong in project records. Lessons concern the researched case and general business conditions; personalized comparisons require a separate explicit request.

## 11.6 Adaptive structure under the approved charter

Codex may refine subheadings, move supporting content, split long chapters, merge adjacent sections, update indexes and correct links **within** the approved high-level book outline.

Material top-level chapter additions/removals/reordering, changed central framing or changes to the approved research scope require human approval. A necessary evidence correction should be recorded immediately at its authoritative source/claim level; a consequential restructuring can then be proposed without silently overriding the charter.

## 11.7 Link and revision integrity

When moving, splitting or renaming sections:

1. Preserve canonical concept and operational IDs; never reallocate because a filename changed.
2. Update part/main indexes and previous/next navigation.
3. Repair inbound/outbound links and ID-to-location lookup entries.
4. Preserve prior consequential synthesis wording through [Chapter 10's revision procedure](../../references/synthesis-revisions.md).
5. Verify essential links and references before advancing the single authoritative project checkpoint.

Purely editorial edits can be maintained routinely. Material interpretation or approval changes require the appropriate audit and authorization records.

## 11.8 Example book shape (illustrative only)

```text
project/book/
  index.md
  part-01-origins/
    index.md
    01-market-before-inception.md
    02-product-and-founders.md
  part-02-gtm-evolution/
    index.md
    03-early-users.md
    04-paying-customers.md
  part-03-interpretation/
    index.md
    05-competing-causes.md
    06-transferable-lessons.md
  appendices/
    concepts-and-sources.md
    revision-history.md
```

This is a planning example, **not** generated research, verified company history or a mandated fixed directory layout. Do not create fictitious sources, customers or findings to populate a scaffold.

## 11.9 Book quality and implementation boundary

The book must have a useful main table of contents, coherent semantic grouping, correct real chapter links, clear definitions, traceable claims, disclosed material contradictions and consistent terminology. It should remain readable as a stand-alone narrative, with evidence available at deeper levels.

**Authoring and closure distinction:** Maintaining a draft book is permitted throughout authorized research. [Objective charter/contract completion](../../references/completion-and-acceptance.md) and [material evidence reopening](../../references/dependency-impact-and-reopening.md) are separate procedures; passing book-quality checks alone never establishes research completion.

**Next:** [Chapter 12 — Human Learning](12-human-learning.md) · [Book architecture procedure](../../references/research-book-architecture.md).
