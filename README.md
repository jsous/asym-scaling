# Asymmetric Scaling Laws from Sparse Features — code for every figure

John Sous and Michael Winer, NeurIPS 2026.

Each figure in the paper is produced by one notebook. The figures in `figures/` are the exact files included in the paper. Every figure is drawn at its printed size, so font sizes in the notebooks are the sizes on the page.

| Figure | Notebook | Data |
|---|---|---|
| 1 | `pictureMaker_PhaseDiagram_WinerSous.ipynb` | none |
| 2, 3 | `sparsemodel/Sparse1_ScalingCollapse_ComputeFrontier.ipynb` | `sparsemodel/results.zip` (archived sweep, 238 + 3,335 rounds) |
| 4 | `sparsemodel/Sparse2_ReLU_Nesterov.ipynb` | `sparsemodel/results_relu_nesterov_20260428_155617.pkl` |
| 5 | `pile/Pile1_DoubleDescentPeak.ipynb` | `pile/peak_location_results.npz` |
| A1, A2 | `sparsemodel/Sparse3_MinNorm_Linear_ReLU.ipynb` | `sparsemodel/results_pinv_linear_and_relu_20260428_181712.pkl` |
| A3 | `pile/Pile2_LinearRF_Exponents.ipynb` | `pile/matched_sweeps.npz`, `pile/cnt_raw.npy` |
| A4 | `pile/Pile3_LazyNetwork.ipynb` | `pile/tangent_sweeps.npz`, `pile/cnt_raw.npy` |

The experiments on the sparse model (Sections 4–7 and Appendix F) are in `sparsemodel/`, and those on Pile token statistics (Section 8 and its appendix) are in `pile/`. In each folder the notebooks are numbered in the order their results appear in the paper, and each one draws its figures from the cached results in that folder, followed by the code of the experiment that produced them. Run the notebooks from their own folder; figures are written to `figures/`.
