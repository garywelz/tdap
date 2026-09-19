# TDAP seed papers

Six seed papers drive TDAP's citation-graph expansion (one hop, references-only, capped — see `copernicus-web`'s `huggingface-space/scripts/acquire_papers/citation_expansion_pilot.py`). All DOIs verified live against Crossref/OpenAlex on 2026-09-19 (not from memory). **Provisional — pending Jordan Matuszewski's and Mikael Vejdemo-Johansson's confirmation**, same as the three questions in [`research_focus.json`](research_focus.json).

## tdap-q1 — circular and toroidal coordinates from persistent cohomology

| Paper | DOI | Reference-list source |
|---|---|---|
| de Silva, Morozov, Vejdemo-Johansson — *Persistent Cohomology and Circular Coordinates* (Discrete Comput. Geom., 2011) | `10.1007/s00454-011-9344-x` | Crossref (19 refs) |
| Perea — *Sparse Circular Coordinates via Principal ℤ-Bundles* (Abel Symposia, 2020) | `10.1007/978-3-030-43408-3_17` | Crossref (24 refs) |
| Scoccola, Gakhar, Bush, Schonsheck, Rask, Zhou, Perea — *Toroidal Coordinates: Decorrelating Circular Coordinates With Lattice Reduction* (SoCG 2023, LIPIcs) | `10.4230/lipics.socg.2023.57` | Not on Crossref; OpenAlex empty. **Has references via Semantic Scholar, queried by arXiv ID `2212.07201`** (32 refs) — not yet wired into the pilot script. |

## tdap-q2 — computing persistent (co)homology at scale

| Paper | DOI | Reference-list source |
|---|---|---|
| Zomorodian, Carlsson — *Computing Persistent Homology* (Discrete Comput. Geom., 2005) | `10.1007/s00454-004-1146-y` | Crossref empty; falls back to OpenAlex (19 refs) |
| Otter, Porter, Tillmann, Grindrod, Harrington — *A roadmap for the computation of persistent homology* (EPJ Data Science, 2017) | `10.1140/epjds/s13688-017-0109-5` | Crossref (179 refs) |
| Nigmetov, Morozov — *Distributed Computation of Persistent Cohomology* (ALENEX 2026 / arXiv:2410.16553) | `10.1137/1.9781611978957.15` | Not on Crossref/OpenAlex by DOI. **Has references via Semantic Scholar, queried by arXiv ID `2410.16553`** (28 refs) — not yet wired into the pilot script. |

Two seeds (Scoccola et al., Nigmetov–Morozov) are real, on-topic papers but can't be expanded *from* via the current DOI-keyed Crossref/OpenAlex mechanism — both are recent enough that neither source has indexed their reference lists by DOI. Semantic Scholar has both, but only when queried by arXiv ID rather than DOI; that's a proposed, not-yet-built third source for the pilot script.

## tdap-q3 — cyclic/recurrent structure in biomedical or physiological data

No confirmed seeds yet. Four candidates proposed by Claude Chat (2026-09-19), DOIs verified live, **topical fit not yet confirmed by Jordan or Mikael**:

| Paper | DOI | Reference-list source |
|---|---|---|
| Perea, Harer — *Sliding Windows and Persistence: An Application of Topological Methods to Signal Analysis* (Found. Comput. Math., 2015) | `10.1007/s10208-014-9206-z` | Crossref (30 refs) |
| Gardner, Hermansen, Pachitariu, Burak, Baas, Dunn, Moser, Moser — *Toroidal topology of population activity in grid cells* (Nature, 2022) | `10.1038/s41586-021-04268-7` | Crossref (92 refs) |
| Rybakken, Baas, Dunn — *Decoding of Neural Data Using Cohomological Feature Extraction* (Neural Computation, 2019) | `10.1162/neco_a_01150` | Crossref (39 refs) |
| Kang, Xu, Morozov — *Evaluating State Space Discovery by Persistent Cohomology in the Spatial Representation System* (Frontiers in Computational Neuroscience, 2021) | `10.3389/fncom.2021.616748` | Crossref (54 refs) |

Notably, the Gardner et al. and Kang/Xu/Morozov papers already appear inside Scoccola et al.'s own reference list (via the Semantic Scholar lookup above) — independent cross-validation that they're topically adjacent to the tdap-q1 seed set, not just individually plausible.

## Dry-run status (2026-09-19)

A citation-expansion dry run against the six tdap-q1/q2 seeds (no Firestore writes) admitted 18 candidates (17 resolvable, 1 unresolved), 0 of which already existed in the corpus under any existing project's tag, 16 of 17 passing metadata validation. **Zero real TDAP papers exist in the corpus as of this writing** — everything above is dry-run validated, not yet written. Full report and methodology: `papers/TDAP_BACKFILL_RECON_2026-09-19.md` in `copernicus-web`.
