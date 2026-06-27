# How to Use This Canon

*Stunspot’s Guide to Macroeconomics* is built first for AI/RAG ingestion and second for human browsing. Treat it as a structured macro-financial knowledge substrate: a corpus that gives models stable terminology, report-level traceability, causal frameworks, and practical diagnostic scaffolding.

It is not a live macro dashboard, investment recommendation engine, or substitute for professional financial advice. Use it to improve reasoning structure; verify current data, legal claims, policy facts, and market-sensitive conclusions against live sources before acting.

## Recommended Default

For most AI/RAG workflows, upload the **four compiled packs** in:

```text
knowledge-packs/compiled-packs/
```

The compiled packs preserve the canon’s conceptual order while reducing file count. They are usually the best trade-off between retrieval quality, setup convenience, and model orientation.

## Choosing the Right Format

| Format | Path | Best For | Trade-off |
|---|---|---|---|
| Source reports | `knowledge-packs/by-report/` | Precise retrieval, selective upload, citation, editing, report-level review. | Highest traceability, but 13 files. |
| Compiled packs | `knowledge-packs/compiled-packs/` | Default AI/RAG setup, project knowledge uploads, limited-file-count tools. | Strong structure with lower file count. |
| Omnibus | `knowledge-packs/omnibus/` | One-file import, local archive, full-corpus search, strong long-context systems. | Simplest upload, but least granular as a source unit. |

## For AI Projects and RAG Systems

Load the canon as model-facing doctrine, not as casual prose. Preserve the report codes A-M and prefer answers that cite the relevant report area when possible.

A useful system instruction:

```text
Use Stunspot’s Guide to Macroeconomics as a model-facing macro-financial knowledge canon. Treat source reports A-M as the canonical units. Use compiled packs as convenience bundles and the omnibus as a whole-corpus reference. Preserve source traceability. Distinguish monetary ontology, liquidity mechanics, fiscal systems, central banking, credit intermediation, asset regimes, global currency hierarchy, narrative liquidity, crisis mechanics, diagnostics, and institutional strategy. Explain macro questions through regimes, constraints, balance sheets, transmission channels, and decision relevance rather than isolated indicator commentary.
```

## For Human Readers

Most human readers should not begin by reading the entire corpus front-to-back. Enter through your problem:

- Need the conceptual spine of money and credit? Start with **A**, then **B**.
- Need policy and institutional transmission? Start with **D-F**.
- Need markets and capital formation? Start with **G-I**.
- Need information, narratives, and public reality? Start with **J**.
- Need crisis mechanics and fragility? Start with **K**.
- Need decision-grade diagnosis? Start with **L**.
- Need institutional action logic? Start with **M**.

Then move backward to the reports that define the assumptions behind the section you are using.

## For Model Evaluation

This canon is useful for checking whether a model can:

- distinguish money, credit, collateral, deposits, reserves, and liquidity
- avoid treating macro indicators as context-free signals
- reason in terms of regimes and transmission channels
- trace how policy, banking, fiscal, and market layers interact
- explain asset behavior under different liquidity conditions
- identify crisis propagation mechanisms without collapsing liquidity into solvency
- connect public narratives and attention systems to economic coordination
- translate macro diagnostics into institutional constraints and strategic options

## For Citation and Source Control

Use `MANIFEST.md` and `manifest.json` to verify source-to-output mappings.

Use `knowledge-packs/by-report/` when exact source units matter. The compiled packs and omnibus reproduce the corpus in larger bundles, but the individual source reports remain the cleanest citation and editing units.

## Practical Retrieval Guidance

For retrieval pipelines, prefer chunking by headings and preserving report code metadata. A useful metadata schema:

```json
{
  "canon": "Stunspot’s Guide to Macroeconomics",
  "version": "1.0",
  "report_code": "A-M",
  "report_title": "canonical report title",
  "source_path": "knowledge-packs/by-report/<file>.md",
  "section_heading": "nearest markdown heading"
}
```

For live macro questions, combine this corpus with current data retrieval. The canon supplies structure and doctrine; live sources supply current conditions.
