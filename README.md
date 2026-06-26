# Stunspot’s Guide to Macroeconomics

**A practical canon for macroeconomics knowledge, reasoning, and AI/RAG use.**  
*A model-facing knowledge base for money, liquidity, credit, regimes, financial instability, and institutional macro strategy.*

![Status](https://img.shields.io/badge/status-v1.0_release-darkgreen)
![Reports](https://img.shields.io/badge/source_reports-13-blue)
![Compiled Packs](https://img.shields.io/badge/compiled_packs-4-blueviolet)
![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/license-CC_BY--NC--SA_4.0-darkgrey)

*Stunspot’s Guide to Macroeconomics* is a Markdown-native knowledge repository built primarily for AI/RAG ingestion, long-context workspaces, project knowledge systems, and model-assisted economic reasoning.

Its main audience is the model.

Human readers can use it as a serious field guide, but the repository is not packaged as consumer economics education. It is structured as a dense operational substrate: source-traceable reports, compiled upload packs, stable terminology, macro-financial doctrine, diagnostic frameworks, and reusable reasoning maps for models that need to interpret money, credit, collateral, liquidity, policy, markets, geoeconomic power, information flows, and institutional strategy with greater precision.

At its core is a systems premise:

> Macroeconomics is not a set of isolated indicators. It is a layered operating system of monetary promises, balance-sheet constraints, liquidity channels, institutional authorities, narrative coordination, and regime-dependent feedback loops.

Use it as reference material.  
Use it as RAG substrate.  
Use it as project knowledge.  
Use it as doctrine for AI systems asked to analyze macro regimes, financial fragility, capital allocation, policy transmission, or institutional exposure.

---

## Start Here

- [Canon Map](./docs/canon-map.md) — the report sequence and intellectual architecture.
- [How to Use This Canon](./docs/how-to-use-this-canon.md) — practical guidance for humans, AI projects, and RAG workflows.
- [Knowledge Packs](./docs/knowledge-packs.md) — which upload format to use and why.
- [Status](./STATUS.md) — release maturity, corpus shape, and caveats.
- [Manifest](./MANIFEST.md) — source-to-output mappings for the release package.

---

## Corpus Shape

- **13 source reports** in [`knowledge-packs/by-report/`](./knowledge-packs/by-report/)
- **4 compiled packs** in [`knowledge-packs/compiled-packs/`](./knowledge-packs/compiled-packs/)
- **1 omnibus bundle** in [`knowledge-packs/omnibus/`](./knowledge-packs/omnibus/)

`docs/` is the navigation and guidance layer for GitHub Pages. The individual source-report corpus lives in `knowledge-packs/by-report/`; compiled upload packs live in `knowledge-packs/compiled-packs/`; the whole-corpus bundle lives in `knowledge-packs/omnibus/`.

This repository intentionally does **not** duplicate source reports under `docs/`.

---

## What This Canon Covers

The canon runs from monetary foundations to institutional action:

1. **Monetary ontology and hierarchy** — money, credit, collateral, settlement assets, bank deposits, reserves, and the balance-sheet physics behind monetary abstraction.
2. **Liquidity creation and transmission** — how global capital flows, offshore dollar funding, repo markets, collateral chains, and funding constraints propagate across systems.
3. **Macro-causal architecture** — cycles, regimes, structural transitions, endogenous fragility, and the causal grammar of macroeconomic change.
4. **Central banking and fiscal states** — policy instruments, monetary intervention, sovereign debt, public spending systems, and fiscal constraint dynamics.
5. **Banking and credit allocation** — commercial banking, financial intermediation, capital distribution, and the operational mechanics of private credit creation.
6. **Asset pricing and geoeconomics** — how liquidity regimes affect equities, bonds, real estate, commodities, venture markets, currency hierarchies, trade systems, and geopolitical power.
7. **Innovation finance and narrative liquidity** — venture capital, speculative capital formation, public-reality formation, media incentives, attention markets, and belief coordination.
8. **Crisis mechanics and diagnostics** — instability, contagion, systemic collapse, regime detection, macro signals, and economic intelligence systems.
9. **Institutional macro strategy** — translating macro intelligence into exposure mapping, liquidity posture, hedging, governance, timing discipline, and strategic coordination.

The reports are designed to be read as a sequence, but the repository is also practical as a retrieval corpus: each report is a source unit, each compiled pack is an upload unit, and the omnibus is a whole-canon archive.

---

## Knowledge Packs

For most AI/RAG systems, start with the **compiled packs**. They preserve the canon’s structure while reducing file-count friction.

| Format | Location | Files | Best Use |
|---|---|---:|---|
| **Source reports** | [`knowledge-packs/by-report/`](./knowledge-packs/by-report/) | 13 | Precise retrieval, selective upload, citation, editing, and source-level inspection. |
| **Compiled packs** | [`knowledge-packs/compiled-packs/`](./knowledge-packs/compiled-packs/) | 4 | Recommended default for AI Projects, RAG systems, and long-context workspaces with moderate file limits. |
| **Omnibus** | [`knowledge-packs/omnibus/`](./knowledge-packs/omnibus/) | 1 | One-file import, local archive, corpus-wide search, or systems that handle large single-file contexts well. |

See [Knowledge Packs](./docs/knowledge-packs.md) for the full upload-format guide.

---

## How To Use It

### For AI/RAG systems

Load the compiled packs when you want broad macroeconomic coverage with clean volume boundaries. Load individual source reports when you need tighter retrieval control, auditability, or report-level citation. Load the omnibus only when your system handles large single-file corpora well.

When using this canon as model context, instruct the model to:

- treat `knowledge-packs/by-report/` as the canonical source-report layer;
- preserve report letters A–M when citing or summarizing;
- distinguish stable macro frameworks from live economic data;
- retrieve or verify current statistics, policy rates, market prices, laws, and institutional facts from fresh sources;
- prefer source-path citations over vague references to “the macro canon.”

### For human readers

Start with [Canon Map](./docs/canon-map.md). The map explains why the sequence begins with money and liquidity before moving into policy, markets, information systems, diagnostics, and strategy. Then use [How to Use This Canon](./docs/how-to-use-this-canon.md) to choose a reading path by task.

---

## Repository Structure

```text
.
├── README.md
├── LICENSE.md
├── CITATION.cff
├── zenodo.json
├── CHANGELOG.md
├── STATUS.md
├── MANIFEST.md
├── manifest.json
├── docs/
│   ├── index.md
│   ├── canon-map.md
│   ├── how-to-use-this-canon.md
│   ├── knowledge-packs.md
│   └── _config.yml
└── knowledge-packs/
    ├── by-report/        # canonical individual reports
    ├── compiled-packs/   # grouped upload packs
    └── omnibus/          # whole-corpus bundle
```

---

## Citation, License, and Status

Version: **1.0**  
Released: **2026-06-26**  
License: **CC BY-NC-SA 4.0**  
Author: **Sam “stunspot” Walker / Collaborative Dynamics**

Repository: https://github.com/Stunspot/stunspots-guide-to-macroeconomics  
Pages: https://stunspot.github.io/stunspots-guide-to-macroeconomics/

See [`CITATION.cff`](./CITATION.cff) and [`zenodo.json`](./zenodo.json) for citation metadata.

---

## Caveat

This is a model-facing macroeconomic knowledge canon, not a live economic data feed, legal opinion, investment recommendation, or substitute for expert review. Use it to improve reasoning and orientation; verify high-impact claims, current data, and decision-critical facts before relying on them.

--stunspot | ⟨🤩⨯📍⟩ and 💠‍🌐Nova
