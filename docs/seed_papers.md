# TDAP seed papers

Ten seed papers, two different provenances:

- **The six tdap-q1/q2 seeds are confirmed — named by Jordan Matuszewski in his original email to Gary Welz (2026-09), not chosen by Claude Code.** Jordan's email named exact titles ("Perea, Sparse Circular Coordinates via Principal ℤ-Bundles"; "Scoccola et al., Toroidal Coordinates..."), which didn't reach Claude Code directly — an earlier hand-off relayed authors only ("Perea," "Scoccola et al."), so Claude Code independently searched Crossref and picked the same papers Jordan had already named, by title/topic match. Resolved 2026-09-19: the seed choices stand on Jordan's authority, not on that search.
- **The four tdap-q3 seeds are Claude Chat's suggestions, DOI-verified by Claude Code, NOT yet confirmed by Jordan or Mikael Vejdemo-Johansson.**

All DOIs verified live against Crossref/OpenAlex/Semantic Scholar on 2026-09-19 (not from memory). The three questions in [`research_focus.json`](research_focus.json) remain provisional pending Jordan's confirmation, same as before.

## tdap-q1 — circular and toroidal coordinates from persistent cohomology

| Paper | DOI | Reference-list source |
|---|---|---|
| de Silva, Morozov, Vejdemo-Johansson — *Persistent Cohomology and Circular Coordinates* (Discrete Comput. Geom., 2011) | `10.1007/s00454-011-9344-x` | Crossref (19 refs) |
| Perea — *Sparse Circular Coordinates via Principal ℤ-Bundles* (Abel Symposia, 2020) | `10.1007/978-3-030-43408-3_17` | Crossref (24 refs) |
| Scoccola, Gakhar, Bush, Schonsheck, Rask, Zhou, Perea — *Toroidal Coordinates: Decorrelating Circular Coordinates With Lattice Reduction* (SoCG 2023, LIPIcs) | `10.4230/lipics.socg.2023.57` | Not on Crossref; OpenAlex empty. Semantic Scholar, queried by arXiv ID `2212.07201` (32 refs) — wired into the pilot script as a third fallback source, 2026-09-19. |

## tdap-q2 — computing persistent (co)homology at scale

| Paper | DOI | Reference-list source |
|---|---|---|
| Zomorodian, Carlsson — *Computing Persistent Homology* (Discrete Comput. Geom., 2005) | `10.1007/s00454-004-1146-y` | Crossref empty; falls back to OpenAlex (19 refs) |
| Otter, Porter, Tillmann, Grindrod, Harrington — *A roadmap for the computation of persistent homology* (EPJ Data Science, 2017) | `10.1140/epjds/s13688-017-0109-5` | Crossref (179 refs) |
| Nigmetov, Morozov — *Distributed Computation of Persistent Cohomology* (ALENEX 2026 / arXiv:2410.16553) | `10.1137/1.9781611978957.15` | Not on Crossref/OpenAlex by DOI. Semantic Scholar, queried by arXiv ID `2410.16553` (28 refs) — wired into the pilot script as a third fallback source, 2026-09-19. |

Two seeds (Scoccola et al., Nigmetov–Morozov) are real, on-topic papers that couldn't be expanded *from* via Crossref/OpenAlex alone — both were too recent for either source to have indexed their reference lists by DOI. Semantic Scholar has both, keyed by arXiv ID rather than DOI; `citation_expansion_pilot.py` now tries it as a third fallback (`semanticscholar_refs_by_arxiv()`), 2026-09-19.

All six tdap-q1/q2 seeds use `admit_policy=all_references` (admit every resolvable reference, not just the top-cited or multiply-cited ones) — their bibliographies are already predominantly computational topology, so the gates built for a broad, mixed-topic seed just under-yielded. The four tdap-q3 candidates below stay on the default `strict` policy, since their bibliographies (e.g. Gardner et al.'s, mostly grid-cell neuroscience) are not predominantly TDA and admitting them wholesale would flood the corpus with off-topic papers.

## tdap-q3 — cyclic/recurrent structure in biomedical or physiological data

No confirmed seeds yet. Four candidates proposed by Claude Chat (2026-09-19), DOIs verified live, **topical fit not yet confirmed by Jordan or Mikael**:

| Paper | DOI | Reference-list source |
|---|---|---|
| Perea, Harer — *Sliding Windows and Persistence: An Application of Topological Methods to Signal Analysis* (Found. Comput. Math., 2015) | `10.1007/s10208-014-9206-z` | Crossref (30 refs) |
| Gardner, Hermansen, Pachitariu, Burak, Baas, Dunn, Moser, Moser — *Toroidal topology of population activity in grid cells* (Nature, 2022) | `10.1038/s41586-021-04268-7` | Crossref (92 refs) |
| Rybakken, Baas, Dunn — *Decoding of Neural Data Using Cohomological Feature Extraction* (Neural Computation, 2019) | `10.1162/neco_a_01150` | Crossref (39 refs) |
| Kang, Xu, Morozov — *Evaluating State Space Discovery by Persistent Cohomology in the Spatial Representation System* (Frontiers in Computational Neuroscience, 2021) | `10.3389/fncom.2021.616748` | Crossref (54 refs) |

Notably, the Gardner et al. and Kang/Xu/Morozov papers already appear inside Scoccola et al.'s own reference list (via the Semantic Scholar lookup above) — independent cross-validation that they're topically adjacent to the tdap-q1 seed set, not just individually plausible.

## Corpus status (2026-09-19) — written and live

**130 papers, 100% embedded — no longer a dry run.** After Claude Chat's title review found the round-2 filter too permissive in two directions (co-citation admitting candidates with no confirmed-seed parent; holding all of Otter et al.'s references too bluntly), the write set was narrowed to the six confirmed seeds plus 124 expansion candidates meeting a trust rule (cited by 2+ confirmed seeds, or citing a confirmed seed directly). All 124 verified admitted before writing; all written (1 as a merge onto a pre-existing GLMP paper, `pubmed_28459448`, which now carries `tdap-q2` alongside its original `glmp-q9` tag); all 129 new/updated docs embedded (`text-embedding-3-small`). Live-verified: the Statistics tab's "Papers by initiative" shows `tdap: 130`, and a real query ("circular coordinates from persistent cohomology") now returns 7 of its top 10 results as genuine TDAP records. Full method, every number, every check: `papers/TDAP_BACKFILL_RECON_2026-09-19.md` in `copernicus-web`.

**Hold list (66 papers)**, not written, awaiting Jordan's/Mikael's spot-check: [`hold_list.md`](hold_list.md) — 25 papers moved out of the write set on review (4 flagged by Chat as "likely accept" on a closer look), 10 of Otter et al.'s off-topic background references, and 31 reachable only from the four not-yet-confirmed tdap-q3 candidate seeds.

**Limits carried into the live corpus**: Otter et al.'s biomedical-application papers inherit the `tdap-q2` tag regardless of actual topic (re-taggable later); two DOI pairs point to the same underlying paper, kept as separate records (no dedup logic exists for this); a few titles carry unnormalized HTML or LaTeX artifacts (e.g. Perea's seed record title still has raw `$$\mathbb {Z}$$`); Scoccola et al.'s seed record has no `doi` field, only an `arxiv_id` (its DOI isn't indexed on Crossref at all).

**Prior dry-run history, superseded, kept for the record:**
- **Round 2** (all ten seeds, before Chat's title review): 198 admitted, 189 would-create, 1 would-merge, 183/190 validated.
- **Round 1** (six tdap-q1/q2 seeds only, `strict` policy, no Semantic Scholar/OpenAlex backfill): 18 candidates, 17 would-create, 16 validated.
