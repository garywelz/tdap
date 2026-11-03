# TDAP hold list — for the owners' review

65 candidate papers found by TDAP's citation-expansion pipeline, held back rather than added to the corpus. **Nothing on this list has been written anywhere** — these are proposals, not corpus members. They're held either because they're background material a broad survey cites for context rather than TDA content itself, or because they were only reachable from four candidate seed papers for a possible future question (tdap-q3, biomedical/physiological) that haven't been confirmed yet.

**To respond**: mark each item keep or drop, then either reply to Gary directly, or open an issue or pull request on this repo, or through the onboarding form once it opens.

(Revised from an earlier, broader version per Claude Chat's title review.)

**Reading the labels.** Each item ends with why the pipeline surfaced it and how often the paper is cited:

- `cited_by_2plus_seeds` — cited by two or more of the seed papers (confirmed or proposed).
- `top_cited_in_seed` — one of the most-cited items in a single seed paper's reference list.
- `all_references_from_seed` — included only because that seed's policy admits every reference it lists.
- `cited_by=N` — how many papers cite it (as recorded by the sources the pipeline queried).

## Moved out of the first corpus write on review (24)

These were held back because they are linked only to the unconfirmed tdap-q3 seeds, are example-dataset papers, or have record-quality issues.

Four flagged by Chat as **likely accept** on a closer look — bolded below.

- UMAP: Uniform Manifold Approximation and Projection -- `10.21105/joss.00861`, cited_by_2plus_seeds, cited_by=10145
- Microstructure of a spatial map in the entorhinal cortex -- `10.1038/nature03721`, cited_by_2plus_seeds, cited_by=4285
- Fully integrated silicon probes for high-density recording of neural activity -- `10.1038/nature24636`, cited_by_2plus_seeds, cited_by=2447
- Place units in the hippocampus of the freely moving rat -- `10.1016/0014-4886(76)90055-8`, top_cited_in_seed, cited_by=1920
- Head-direction cells recorded from the postsubiculum in freely moving rats. I. Description and quantitative analysis -- `10.1523/jneurosci.10-02-00420.1990`, cited_by_2plus_seeds, cited_by=1895
- Conjunctive Representation of Position, Direction, and Velocity in Entorhinal Cortex -- `10.1126/science.1125572`, cited_by_2plus_seeds, cited_by=1558
- ELEMENTS OF ALGEBRAIC TOPOLOGY (a chapter of Kuratowski, *Introduction to Set Theory and Topology*, Elsevier, 1972, pp. 291–342) -- `10.1016/b978-0-08-016160-0.50028-2`, cited_by_2plus_seeds, cited_by=1304
- Representation of spatial orientation by the intrinsic dynamics of the head-direction cell ensemble: a theory -- `10.1523/jneurosci.16-06-02112.1996`, cited_by_2plus_seeds, cited_by=1069
- Persistent Propagation of Concentration Waves in Dissipative Media Far from Thermal Equilibrium -- `10.1143/ptp.55.356`, top_cited_in_seed, cited_by=1049
- Accurate Path Integration in Continuous Attractor Network Models of Grid Cells -- `10.1371/journal.pcbi.1000291`, cited_by_2plus_seeds, cited_by=858
- The entorhinal grid map is discretized -- `10.1038/nature11649`, cited_by_2plus_seeds, cited_by=762
- The intrinsic attractor manifold and population dynamics of a canonical cognitive circuit across waking and sleep **[Chat: likely accept]** -- `10.1038/s41593-019-0460-x`, cited_by_2plus_seeds, cited_by=432
- Clique topology reveals intrinsic geometric structure in neural correlations **[Chat: likely accept]** -- `10.1073/pnas.1506407112`, cited_by_2plus_seeds, cited_by=415
- Grid cell symmetry is shaped by environmental geometry -- `10.1038/nature14153`, cited_by_2plus_seeds, cited_by=412
- A Multiplexed, Heterogeneous, and Adaptive Code for Navigation in Medial Entorhinal Cortex -- `10.1016/j.neuron.2017.03.025`, cited_by_2plus_seeds, cited_by=353
- The Kuramoto-Sivashinsky equation: A bridge between PDE'S and dynamical systems -- `10.1016/0167-2789(86)90166-1`, top_cited_in_seed, cited_by=335
- Internally organized mechanisms of the head direction sense -- `10.1038/nn.3968`, cited_by_2plus_seeds, cited_by=325
- Three-dimensional head-direction coding in the bat brain -- `10.1038/nature14031`, cited_by_2plus_seeds, cited_by=317
- Nonlinear analysis of hydrodynamic instability in laminar flames—II. Numerical experiments -- `10.1016/0094-5765(77)90097-2`, top_cited_in_seed, cited_by=293
- On Irregular Wavy Flow of a Liquid Film Down a Vertical Plane -- `10.1143/ptp.63.2112`, top_cited_in_seed, cited_by=282
- Shearing-induced asymmetry in entorhinal grid cells -- `10.1038/nature14151`, cited_by_2plus_seeds, cited_by=246
- Topological analysis of population activity in visual cortex **[Chat: likely accept]** -- `10.1167/8.8.11`, cited_by_2plus_seeds, cited_by=232
- A Topological Paradigm for Hippocampal Spatial Map Formation Using Persistent Homology **[Chat: likely accept]** -- `10.1371/journal.pcbi.1002581`, cited_by_2plus_seeds, cited_by=223
- An Algebraic Family of Complex Lattices for Fading Channels With Application to Space–Time Codes -- `10.1109/tit.2005.858923`, all_references_from_seed, cited_by=34

## Background material cited by the Otter et al. roadmap (10)

Broad background (small-world networks, clustering, physics) that the roadmap cites for context, not TDA content itself.

- Collective dynamics of ‘small-world’ networks -- `10.1038/30918`, top_cited_in_seed, cited_by=43633
- Novel Type of Phase Transition in a System of Self-Driven Particles -- `10.1103/physrevlett.75.1226`, top_cited_in_seed, cited_by=7529
- Finding Groups in Data -- `10.1002/9780470316801`, top_cited_in_seed, cited_by=7300
- The structure of the nervous system of the nematode Caenorhabditis elegans -- `10.1098/rstb.1986.0056`, top_cited_in_seed, cited_by=5873
- Random Geometric Graphs -- `10.1093/acprof:oso/9780198506263.001.0001`, top_cited_in_seed, cited_by=2531
- Graph clustering -- `10.1016/j.cosrev.2007.05.001`, top_cited_in_seed, cited_by=1616
- Data Clustering: Theory, Algorithms, and Applications -- `10.1137/1.9780898718348`, top_cited_in_seed, cited_by=1571
- A Survey of Statistical Network Models -- `10.1561/2200000005`, all_references_from_seed, cited_by=861
- Small-world connectivity, motif composition, and complexity of fractal neuronal connections -- `10.1016/j.biosystems.2006.02.008`, all_references_from_seed, cited_by=190
- Unveiling patterns of international communities in a global city using mobile phone data -- `10.1140/epjds/s13688-015-0041-5`, all_references_from_seed, cited_by=40

## Reachable only from the four proposed Q3 seeds (31)

These stay on hold until the owners confirm the four proposed seeds themselves.

- Generalized Linear Models -- `10.1007/978-1-4899-3242-6`, top_cited_in_seed, cited_by=16924
- Mean shift: a robust approach toward feature space analysis -- `10.1109/34.1000236`, top_cited_in_seed, cited_by=11432
- Fast and robust fixed-point algorithms for independent component analysis -- `10.1109/72.761722`, top_cited_in_seed, cited_by=6386
- The hippocampus as a spatial map. Preliminary evidence from unit activity in the freely-moving rat -- `10.1016/0006-8993(71)90358-1`, top_cited_in_seed, cited_by=6386
- Least-squares frequency analysis of unequally spaced data -- `10.1007/bf00648343`, top_cited_in_seed, cited_by=5822
- Nonlinear Time Series Analysis -- `10.1017/cbo9780511755798`, top_cited_in_seed, cited_by=2644
- Extensions of Lipschitz mappings into a Hilbert space -- `10.1090/conm/026/737400`, top_cited_in_seed, cited_by=2578
- The Variable Discharge of Cortical Neurons: Implications for Connectivity, Computation, and Information Coding -- `10.1523/jneurosci.18-10-03870.1998`, top_cited_in_seed, cited_by=2313
- Path integration and the neural basis of the 'cognitive map' -- `10.1038/nrn1932`, top_cited_in_seed, cited_by=2132
- Dynamics of pattern formation in lateral-inhibition type neural fields -- `10.1007/bf00337259`, top_cited_in_seed, cited_by=2124
- The importance of mixed selectivity in complex cognitive tasks -- `10.1038/nature12160`, top_cited_in_seed, cited_by=1849
- The Theta-Gamma Neural Code -- `10.1016/j.neuron.2013.03.007`, top_cited_in_seed, cited_by=1753
- Nonlinear dynamical analysis of EEG and MEG: Review of an emerging field -- `10.1016/j.clinph.2005.06.011`, top_cited_in_seed, cited_by=1434
- Memory of Sequential Experience in the Hippocampus during Slow Wave Sleep -- `10.1016/s0896-6273(02)01096-6`, top_cited_in_seed, cited_by=1361
- Dimensionality reduction for large-scale neural recordings -- `10.1038/nn.3776`, top_cited_in_seed, cited_by=1356
- Synaptic Mechanisms and Network Dynamics Underlying Spatial Working Memory in a Cortical Network Model -- `10.1093/cercor/10.9.910`, top_cited_in_seed, cited_by=1242
- JTK_CYCLE: An Efficient Nonparametric Algorithm for Detecting Rhythmic Components in Genome-Scale Data Sets -- `10.1177/0748730410379711`, top_cited_in_seed, cited_by=1196
- Neuropixels 2.0: A miniaturized high-density probe for stable, long-term brain recordings -- `10.1126/science.abf4588`, top_cited_in_seed, cited_by=1158
- Theory of orientation tuning in visual cortex. -- `10.1073/pnas.92.9.3844`, top_cited_in_seed, cited_by=1146
- The hippocampus as a predictive map -- `10.1038/nn.4650`, top_cited_in_seed, cited_by=1091
- Path Integration and Cognitive Mapping in a Continuous Attractor Neural Network Model -- `10.1523/jneurosci.17-15-05900.1997`, top_cited_in_seed, cited_by=1043
- Deciphering The Hippocampal Polyglot: the Hippocampus as a Path Integration System -- `10.1242/jeb.199.1.173`, top_cited_in_seed, cited_by=936
- Head-direction cells recorded from the postsubiculum in freely moving rats. II. Effects of environmental manipulations -- `10.1523/jneurosci.10-02-00436.1990`, top_cited_in_seed, cited_by=905
- Computational Topology -- `10.1090/mbk/069`, top_cited_in_seed, cited_by=806
- Neural Manifolds for the Control of Movement -- `10.1016/j.neuron.2017.05.025`, top_cited_in_seed, cited_by=779
- Linking Spontaneous Activity of Single Cortical Neurons and the Underlying Functional Architecture -- `10.1126/science.286.5446.1943`, top_cited_in_seed, cited_by=758
- Gaussian-Process Factor Analysis for Low-Dimensional Single-Trial Analysis of Neural Population Activity -- `10.1152/jn.90941.2008`, top_cited_in_seed, cited_by=746
- The Structure and Stability of Persistence Modules -- `10.1007/978-3-319-42545-0`, top_cited_in_seed, cited_by=398
- Directionally selective mnemonic properties of neurons in the lateral dorsal nucleus of the thalamus of rats -- `10.1523/jneurosci.13-09-04015.1993`, top_cited_in_seed, cited_by=366
- Interactions Between Idiothetic Cues and External Landmarks in the Control of Place Cells and Head Direction Cells -- `10.1152/jn.1998.80.1.425`, top_cited_in_seed, cited_by=323
- Detecting periodic patterns in unevenly spaced gene expression time series using Lomb–Scargle periodograms -- `10.1093/bioinformatics/bti789`, top_cited_in_seed, cited_by=270

## Identifier checks (Crossref, 2026-11-02)

- `10.1016/b978-0-08-016160-0.50028-2` — resolved: the chapter "Elements of Algebraic Topology" by Kazimierz Kuratowski, in *Introduction to Set Theory and Topology* (Elsevier, 1972, ISBN 9780080161600). Kept on the list, with the title above made explicit.
- `10.1007/bf01565634` ("Wolfram") — removed. Crossref gives only a one-page item in *Die Naturwissenschaften* 1 (1913), p. 511, titled "Wolfram", with author "Mk." and no reference list or abstract. It is not identifiable as a paper on this topic, so it was dropped from the hold list. This is why the first group reads 24 and the total 65 (it was 25 and 66).
