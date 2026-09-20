# Topological Data Analysis Project (TDAP)

TDAP studies persistent cohomology and the circular/toroidal coordinates it recovers from data — and, downstream, where that machinery can detect cyclic or recurrent structure in domains that were not built with topology in mind.

TDAP is a new engine in the Copernicus science suite, alongside [GLMP](https://github.com/garywelz/glmp) and [ATAP](https://github.com/garywelz/atap). This repository holds the engine's open questions. As of 2026-09-19, TDAP has a 130-paper metadata-first corpus (see **Corpus status** below) grown from six seed papers and anchor authors, following the acquisition and embedding pipeline already built for GLMP and ATAP in [copernicus-web](https://github.com/garywelz/copernicus-web) — there is still no chart corpus or manuscript.

*Gary Welz · CUNY Graduate Center / New Media Lab · [gwelz@gc.cuny.edu](mailto:gwelz@gc.cuny.edu)*

**Collaborator:** Jordan Matuszewski, PhD student in Computer Science, CUNY Graduate Center · [jmatuszewski@ccny.cuny.edu](mailto:jmatuszewski@ccny.cuny.edu)

---

## What lives in this repo

| | |
|---|---|
| **Open questions** | [`docs/research_focus.json`](docs/research_focus.json) — the engine's current questions and frontier. All three active questions are provisional as of 2026-09-19, pending Jordan's confirmation. |
| **Seed papers** | [`docs/seed_papers.md`](docs/seed_papers.md) — the papers TDAP's citation-graph expansion grows from. Six confirmed (named by Jordan); four additional tdap-q3 candidates still pending Jordan's and Mikael's confirmation. |
| **Claude Project instructions** | [`docs/project_instructions.md`](docs/project_instructions.md) — the canonical, paste-in instruction set for running a Claude Project against this repo (v0.2, 2026-09-19). |

Unlike ATAP and GLMP at this stage, there is no corpus table or manuscript directory yet. Those get added once TDAP has its own chart or manuscript artifacts.

---

## Corpus status (2026-09-19)

**130 papers, 100% embedded.** Grown by one-hop citation-graph expansion from the six confirmed seed papers, keeping candidates cited by 2+ seeds or citing a confirmed seed directly. Full method, every number, and every verification step: [`TDAP_BACKFILL_RECON_2026-09-19.md`](https://github.com/garywelz/copernicus-web/blob/main/papers/TDAP_BACKFILL_RECON_2026-09-19.md) in `copernicus-web`. A further 66-paper hold list — broader background material from one seed's survey-style bibliography, plus everything reachable only from the four not-yet-confirmed tdap-q3 candidate seeds — awaits Jordan's and Mikael's spot-check: [`tdap_hold_list_v2_2026-09-19.md`](https://github.com/garywelz/copernicus-web/blob/main/papers/tdap_hold_list_v2_2026-09-19.md).

Known limits (detail in the recon doc above): the live Knowledge Engine toggle doesn't yet scope paper search to TDAP specifically (shared with GLMP/ATAP); a couple of DOI pairs point to the same underlying paper (kept as separate records, not deduplicated); a few titles carry unnormalized HTML or LaTeX artifacts from their source metadata; one seed (Scoccola et al.) has no DOI on file, only an arXiv id.

---

## Open items

- **The future graphics/chart bucket should be format-agnostic, not Mermaid-specific.** GLMP and ATAP both settled on Mermaid diagrams for their process/proof charts; TDAP has explicitly deferred deciding on a chart format for version one (no TDAP chart family yet — see `copernicus-web`'s `PROCESS_FAMILY_COLLECTIONS`). When TDAP does grow chart or diagram artifacts, the format should be chosen for what persistent-cohomology and circular-coordinate objects actually need to show (e.g. persistence diagrams, barcodes, toroidal embeddings) rather than defaulting to the nodes-and-edges shape Mermaid is built for — the same "anti-hammer" caution ATAP's own `research_focus.json` (`atap-f3`) already raises about its own domain.
- **License is currently mirrored from ATAP/GLMP (CC0 1.0 Universal)** as a default, not yet confirmed with Jordan.
- **Jordan's GitHub username is not yet known** — no collaborator added yet, though the repo is now public and readable/forkable without one.
- **Jordan's name and CCNY email are listed publicly in this README** (mirroring how Gary's own contact info is listed) — not yet confirmed acceptable with Jordan, and now a real question since the repo went from private to public.

---

## Using TDAP inside your own Claude

TDAP is a collaboration between Jordan Matuszewski (CUNY Graduate Center, PhD student in Computer Science, advised by Mikael Vejdemo-Johansson) and Gary Welz (CUNY Graduate Center / New Media Lab), part of the Copernicus Knowledge Engine suite. If you use Claude, you can give it live access to this project's current state — it fetches directly from this repository, so it stays current automatically without any uploading or re-syncing.

**Set it up once:**

1. In Claude, create a new Project (name it "TDAP" or similar).
2. Turn on web access for the Project — the instructions below fetch live files from this repo, which needs it.
3. Open [`docs/project_instructions.md`](docs/project_instructions.md), copy its full contents, and paste them into the Project's custom instructions.
4. Fill in the `[bracketed]` items in what you pasted — those are yours to decide, not preset.

`docs/project_instructions.md` is the single canonical instruction set — this README doesn't carry its own separate copy, so there's nothing here to fall out of sync. If the instructions need to change, edit that file, not this section.

## Background

TDAP's anchor-author overlap with GLMP is not incidental: Dr. Mikael Vejdemo-Johansson (CUNY Graduate Center) already collaborated on a persistent-homology pilot over GLMP's gene-regulatory circuit corpus (`glmp/tda-analysis/`, part of the CopernicusAI / NSF CISE proposal) — computing H1 loops over 108 processes and finding that the most persistent loops correspond to known feedback circuits (lac operon, two-component signaling, SOS response). TDAP is the topology-first counterpart: instead of applying TDA to an existing biological corpus, it builds a corpus around the topology itself — starting from persistent cohomology and circular coordinates, with computational-topology-at-scale and biomedical applications as adjacent questions.

## License

[CC0 1.0 Universal](LICENSE) — the contents of this repository are dedicated to the public domain to the extent allowed by law.
