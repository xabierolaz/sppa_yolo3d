# Instant Semantic Proxy Reconstruction for UAV Digital Twins under Degraded Sensing (SPPA-MVFit)

Companion repository for the paper. It contains the full LaTeX manuscript (compile-ready, mirrors the Overleaf project) and links to the sealed reproducibility package and additional resources.

**Status:** under review (target venue: *Journal of Geovisualization and Spatial Analysis*, Springer). Authors omitted while the manuscript is under double-anonymous review.

## TL;DR

One 2D detection compiles into a role-labeled eight-part primitive 3D actor in **9.4 ms median CPU** and a **1.45 kB** update descriptor, so a geospatial digital twin can absorb object-level semantic telemetry instead of degraded video. On 240 preregistered held-out synthetic actors, the family-conditioned part graph improves clean voxel IoU over an equal-budget generic graph by **+0.190** (95% CI [0.181, 0.199]), maintained under every prespecified observation corruption. Boundary arms map where the prior stops: wrong family tokens, adversarial instances, and external real meshes.

## Repository contents

| Path | Content |
|---|---|
| `main.tex` | Full manuscript (single self-contained paper, no supplement) |
| `semantic_proxy_3d_references.bib` | Bibliography |
| `figures/` | Figures referenced by the manuscript (incl. the SPPA vs. neural image-to-3D generators comparison) |
| `benchmarks/` | Result tables included in the paper (`\input`) |

## Reproduce

- **Reproducibility package (sealed, SHA-256 manifest):** download `sppa_mvfit_rp.zip` from the [Resources release](../../releases/tag/resources). It contains the frozen method (`method/sppa_mvfit.py`, `graphs.json`), the preregistered protocol, generation/evaluation code, locked requirements and the development + confirmatory result sets (H1 PASS). Unzip and follow its `README.md`.
- **Compile the paper:** `pdflatex main.tex && bibtex main && pdflatex main.tex && pdflatex main.tex` (standard pdfLaTeX; compiles identically on Overleaf).

## Citation

Citation details will be added upon publication.
