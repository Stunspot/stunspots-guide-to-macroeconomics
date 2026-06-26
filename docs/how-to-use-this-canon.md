# How to Use This Canon

*Stunspot’s Guide to Macroeconomics* is built for model-facing use first. The practical goal is to improve how AI systems reason about macro-financial structure: money, liquidity, credit, policy, regimes, instability, narrative, diagnostics, and institutional action.

The repository is human-readable, but it is not trying to be a glossy popular-economics course. Treat it as a structured knowledge substrate.

---

## The Fast Path

For most AI/RAG systems, start with the **compiled packs** in [`knowledge-packs/compiled-packs/`](https://github.com/Stunspot/stunspots-guide-to-macroeconomics/tree/main/knowledge-packs/compiled-packs).

They provide four files, one per canon volume:

1. **A–C** — monetary reality, liquidity, and macro causality.
2. **D–F** — central banking, fiscal states, and banking systems.
3. **G–I** — asset pricing, geoeconomic power, and innovation finance.
4. **J–M** — information liquidity, crisis mechanics, diagnostics, and institutional strategy.

This format usually gives the best balance of coverage, upload simplicity, retrieval coherence, and manageable file count.

---

## Choose the Right Format

| Format | Path | Best For | Tradeoff |
|---|---|---|---|
| **Source reports** | [`knowledge-packs/by-report/`](https://github.com/Stunspot/stunspots-guide-to-macroeconomics/tree/main/knowledge-packs/by-report) | Precise retrieval, selective upload, source citation, editing, and report-level inspection. | More files to manage. |
| **Compiled packs** | [`knowledge-packs/compiled-packs/`](https://github.com/Stunspot/stunspots-guide-to-macroeconomics/tree/main/knowledge-packs/compiled-packs) | Recommended default for AI Projects, RAG systems, NotebookLM-style tools, and long-context workspaces. | Broader files; retrieval boundaries are volume-level. |
| **Omnibus** | [`knowledge-packs/omnibus/`](https://github.com/Stunspot/stunspots-guide-to-macroeconomics/tree/main/knowledge-packs/omnibus) | One-file import, local archive, corpus-wide search, or strong long-context systems. | Large file; weaker natural retrieval segmentation. |

---

## How Humans Should Read It

Start with the [Canon Map](./canon-map.md). It explains the report sequence and why the canon begins with monetary ontology before moving through liquidity, regimes, institutions, markets, information systems, diagnostics, and strategy.

Then choose by task:

### If you need the conceptual foundations

Read:

1. **A. Monetary Ontology & Economic Reality Models**
2. **B. Liquidity Physics and Global Capital Flow Dynamics**
3. **C. Macro-Causal Architecture & Economic Regime Theory**

This path establishes the core grammar: money is hierarchical, liquidity is transmitted through balance sheets, and macro signals are regime-dependent.

### If you need policy and institutional machinery

Read:

1. **D. Central Banking Systems & Monetary Intervention Architecture**
2. **E. Fiscal States, Sovereign Debt, and Political Capital Allocation**
3. **F. Banking Systems, Credit Allocation, and Financial Intermediation**

This path explains how state authority, central-bank tools, fiscal capacity, debt markets, and banking systems shape macro outcomes.

### If you need markets and capital allocation

Read:

1. **G. Asset Pricing Regimes & Cross-Market Liquidity Transmission**
2. **H. Global Trade Systems, Currency Hierarchies, and Geoeconomic Power**
3. **I. Innovation Finance, Venture Liquidity, and Speculative Capital Formation**

This path connects liquidity conditions to asset prices, global power, reserve hierarchies, and speculative innovation cycles.

### If you need diagnostics, crisis awareness, or strategy

Read:

1. **J. Information Liquidity, Narrative Markets, and Attention Allocation Systems**
2. **K. Financial Instability, Crisis Cascades, and Systemic Collapse Mechanics**
3. **L. Macro Diagnostics, Regime Detection, and Economic Intelligence Systems**
4. **M. Institutional Macro Strategy, Adaptive Positioning, and Strategic Coordination**

This path is the most operational. It turns macro structure into signal interpretation, crisis mapping, and organizational decision support.

---

## How AI/RAG Systems Should Use It

When loading this canon into a model, RAG pipeline, project knowledge base, or agent memory system, preserve the repository’s source hierarchy:

- `knowledge-packs/by-report/` contains the canonical report units.
- `knowledge-packs/compiled-packs/` contains grouped upload units.
- `knowledge-packs/omnibus/` contains the whole corpus in one file.
- `docs/` contains navigation and usage guidance only.

Do not treat `docs/` as the source-report corpus.

### Suggested Model Instruction

Use the following instruction block when attaching the canon to an AI workspace:

```text
Use Stunspot’s Guide to Macroeconomics as a model-facing macroeconomic knowledge canon. Treat the source reports in knowledge-packs/by-report/ as the canonical individual units, preserving report letters A–M and source paths when citing or summarizing. Treat compiled packs as upload convenience bundles and the omnibus as an archival whole-corpus bundle.

Use the canon to reason about monetary hierarchy, liquidity transmission, credit creation, central banking, fiscal systems, banking intermediation, asset regimes, geoeconomic power, innovation finance, information liquidity, crisis cascades, macro diagnostics, and institutional strategy.

Distinguish stable conceptual frameworks from live economic data. Verify current statistics, policy rates, market prices, laws, central-bank decisions, institutional roles, and post-release events from fresh sources before relying on them. When answering, prefer source-grounded synthesis over generic macro commentary.
```

### Retrieval Guidance

For RAG systems, index the source reports when you need report-level citation and clean provenance. Index the compiled packs when the platform has tight file-count limits. Avoid mixing source reports and compiled packs in the same retrieval collection unless your system deduplicates aggressively; otherwise the same text may be retrieved twice from different packaging layers.

Recommended metadata fields:

| Field | Example | Purpose |
|---|---|---|
| `canon` | `stunspots-guide-to-macroeconomics` | Distinguishes this corpus from other knowledge bases. |
| `report_code` | `A`, `B`, `C` | Preserves the canonical sequence. |
| `report_title` | `Monetary Ontology & Economic Reality Models` | Improves citation and retrieval display. |
| `source_path` | `knowledge-packs/by-report/a-monetary-ontology-and-economic-reality-models.md` | Enables source traceability. |
| `pack_type` | `source-report`, `compiled-pack`, `omnibus` | Prevents duplicate-source confusion. |
| `release_version` | `1.0` | Supports version-aware retrieval. |
| `release_date` | `2026-06-26` | Helps models distinguish canon date from current events. |

---

## Citation and Answering Discipline

When generating answers from the canon, prefer this hierarchy:

1. Cite or name the specific report when using a source-report claim.
2. Preserve technical distinctions from the corpus, especially money versus credit, liquidity versus solvency, reserves versus deposits, and narrative visibility versus empirical truth.
3. State uncertainty when the canon provides a conceptual model but not current data.
4. Use fresh sources for current macro conditions, market data, policy decisions, laws, and institutional facts.
5. Avoid flattening the corpus into generic “economics says” summaries; the value is in its structural distinctions.

---

## What This Canon Is Not

This is not a live data dashboard, investment recommendation engine, legal opinion, trading system, or substitute for professional review. It is a reasoning substrate. It improves orientation, vocabulary, causal mapping, and diagnostic thinking; it does not automatically make a model current, certain, or decision-authorized.
