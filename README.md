# Asymmetric Scaling Laws from Sparse Features — code for every figure

John Sous and Michael Winer, NeurIPS 2026.

Each figure in the paper is produced by one notebook. The figures in `figures/` are the exact files included in the paper. Every figure is drawn at its printed size, so font sizes in the notebooks are the sizes on the page.

| Figure | Notebook | Data |
|---|---|---|
| 1 | `pictureMaker_PhaseDiagram_WinerSous.ipynb` | none |
| 2, 3 | `SparseScaling1.ipynb` | `data/results.zip` (archived sweep, 238 + 3,335 rounds) |
| 4 | `SparseScaling2.ipynb` | `data/results_relu_nesterov_20260428_155617.pkl` |
| 5 | `pile/Pile1_DoubleDescentPeak.ipynb` | `pile/peak_location_results.npz` |
| A1, A2 | `SparseScaling_Appendix.ipynb` | `data/results_pinv_linear_and_relu_20260428_181712.pkl` |
| A3 | `pile/Pile2_LinearRF_Exponents.ipynb` | `pile/matched_sweeps.npz`, `pile/cnt_raw.npy` |
| A4 | `pile/Pile3_LazyNetwork.ipynb` | `pile/tangent_sweeps.npz`, `pile/cnt_raw.npy` |

The experiments on Pile token statistics (Section 8 and its appendix) are in `pile/`, numbered in the order their results appear in the paper. Each notebook first draws its figure from the cached results in that folder, then contains the experiment that produced them, which runs in place.
