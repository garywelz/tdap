# Topological Data Analysis Project (TDAP)

TDAP studies persistent cohomology and the circular/toroidal coordinates it recovers from data — and, downstream, where that machinery can detect cyclic or recurrent structure in domains that were not built with topology in mind.

TDAP is a new engine in the Copernicus science suite, alongside [GLMP](https://github.com/garywelz/glmp) and [ATAP](https://github.com/garywelz/atap). This repository holds the engine's open questions. As of this writing there is no chart corpus or manuscript yet — TDAP starts as a metadata-first paper corpus grown from a small set of seed papers and anchor authors, following the acquisition and embedding pipeline already built for GLMP and ATAP in [copernicus-web](https://github.com/garywelz/copernicus-web).

*Gary Welz · CUNY Graduate Center / New Media Lab · [gwelz@gc.cuny.edu](mailto:gwelz@gc.cuny.edu)*

**Collaborator:** Jordan Matuszewski, PhD student in Computer Science, CUNY Graduate Center · [jmatuszewski@ccny.cuny.edu](mailto:jmatuszewski@ccny.cuny.edu)

---

## What lives in this repo

| | |
|---|---|
| **Open questions** | [`docs/research_focus.json`](docs/research_focus.json) — the engine's current questions and frontier. All three active questions are provisional as of 2026-09-19, pending Jordan's confirmation. |

Unlike ATAP and GLMP at this stage, there is no corpus table or manuscript directory yet. Those get added once the seed-driven paper corpus exists.

---

## Open items

- **The future graphics/chart bucket should be format-agnostic, not Mermaid-specific.** GLMP and ATAP both settled on Mermaid diagrams for their process/proof charts; TDAP has explicitly deferred deciding on a chart format for version one (no TDAP chart family yet — see `copernicus-web`'s `PROCESS_FAMILY_COLLECTIONS`). When TDAP does grow chart or diagram artifacts, the format should be chosen for what persistent-cohomology and circular-coordinate objects actually need to show (e.g. persistence diagrams, barcodes, toroidal embeddings) rather than defaulting to the nodes-and-edges shape Mermaid is built for — the same "anti-hammer" caution ATAP's own `research_focus.json` (`atap-f3`) already raises about its own domain.
- **License is currently mirrored from ATAP/GLMP (CC0 1.0 Universal)** as a default, not yet confirmed with Jordan.
- **Jordan's GitHub username is not yet known** — this repo has not been shared or had a collaborator added.

---

## Background

TDAP's anchor-author overlap with GLMP is not incidental: Dr. Mikael Vejdemo-Johansson (CUNY Graduate Center) already collaborated on a persistent-homology pilot over GLMP's gene-regulatory circuit corpus (`glmp/tda-analysis/`, part of the CopernicusAI / NSF CISE proposal) — computing H1 loops over 108 processes and finding that the most persistent loops correspond to known feedback circuits (lac operon, two-component signaling, SOS response). TDAP is the topology-first counterpart: instead of applying TDA to an existing biological corpus, it builds a corpus around the topology itself — starting from persistent cohomology and circular coordinates, with computational-topology-at-scale and biomedical applications as adjacent questions.

## License

[CC0 1.0 Universal](LICENSE) — the contents of this repository are dedicated to the public domain to the extent allowed by law.
