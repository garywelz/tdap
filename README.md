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
| **Seed papers** | [`docs/seed_papers.md`](docs/seed_papers.md) — the papers TDAP's citation-graph expansion grows from, one per question, DOI-verified. Provisional, pending Jordan's and Mikael's confirmation. |

Unlike ATAP and GLMP at this stage, there is no corpus table or manuscript directory yet. Those get added once the seed-driven paper corpus exists.

---

## Open items

- **The future graphics/chart bucket should be format-agnostic, not Mermaid-specific.** GLMP and ATAP both settled on Mermaid diagrams for their process/proof charts; TDAP has explicitly deferred deciding on a chart format for version one (no TDAP chart family yet — see `copernicus-web`'s `PROCESS_FAMILY_COLLECTIONS`). When TDAP does grow chart or diagram artifacts, the format should be chosen for what persistent-cohomology and circular-coordinate objects actually need to show (e.g. persistence diagrams, barcodes, toroidal embeddings) rather than defaulting to the nodes-and-edges shape Mermaid is built for — the same "anti-hammer" caution ATAP's own `research_focus.json` (`atap-f3`) already raises about its own domain.
- **License is currently mirrored from ATAP/GLMP (CC0 1.0 Universal)** as a default, not yet confirmed with Jordan.
- **Jordan's GitHub username is not yet known** — no collaborator added yet, though the repo is now public and readable/forkable without one.
- **Jordan's name and CCNY email are listed publicly in this README** (mirroring how Gary's own contact info is listed) — not yet confirmed acceptable with Jordan, and now a real question since the repo went from private to public.

---

## Using TDAP inside your own Claude

If you use Claude, you can give it live access to TDAP's current state — the project overview and its open research questions — so it can help you explore the corpus and shape your suggestions. It reads directly from this repository, so it's always current.

**Set it up once:**

1. In Claude, create a new Project (name it "TDAP" or similar).
2. Open the project's **instructions** and paste the block below.
3. That's it — every conversation in that project now reads TDAP's current context live from GitHub.

```
This project works with the Topological Data Analysis Project (TDAP).
At the start of substantive work, fetch these from GitHub and treat them
as the current source of truth:
- https://raw.githubusercontent.com/garywelz/tdap/main/README.md
- https://raw.githubusercontent.com/garywelz/tdap/main/docs/research_focus.json
- https://raw.githubusercontent.com/garywelz/tdap/main/docs/seed_papers.md

TDAP is a collaboration between Jordan Matuszewski (CUNY Graduate Center,
PhD student in Computer Science, advised by Mikael Vejdemo-Johansson) and
Gary Welz (CUNY Graduate Center / New Media Lab), part of the Copernicus
Knowledge Engine suite. This is your window into the project: explore the
seed papers and citation-expansion corpus, and the open research questions,
and use what you find to shape suggestions and analysis for Jordan's
research. The project's canonical files live in GitHub and are maintained
by the project's collaborators -- so treat this as a rich read-only context
to think with, not a workspace to edit.
```

Nothing to upload, nothing to keep in sync — when the project updates, your Claude sees it the next time you start a conversation.

## Background

TDAP's anchor-author overlap with GLMP is not incidental: Dr. Mikael Vejdemo-Johansson (CUNY Graduate Center) already collaborated on a persistent-homology pilot over GLMP's gene-regulatory circuit corpus (`glmp/tda-analysis/`, part of the CopernicusAI / NSF CISE proposal) — computing H1 loops over 108 processes and finding that the most persistent loops correspond to known feedback circuits (lac operon, two-component signaling, SOS response). TDAP is the topology-first counterpart: instead of applying TDA to an existing biological corpus, it builds a corpus around the topology itself — starting from persistent cohomology and circular coordinates, with computational-topology-at-scale and biomedical applications as adjacent questions.

## License

[CC0 1.0 Universal](LICENSE) — the contents of this repository are dedicated to the public domain to the extent allowed by law.
