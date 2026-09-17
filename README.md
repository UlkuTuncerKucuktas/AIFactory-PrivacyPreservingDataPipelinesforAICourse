![BSC AI Factory — Privacy-Preserving Data Pipelines for AI](assets/headers/course-banner.png)

# Privacy-Preserving Data Pipelines for AI

Five notebooks for Module 8 of the BSC AI Factory course.

| Notebook | Content |
| --- | --- |
| [01 — Document anonymization](01_Document_Anonymization.ipynb) | Detect identifying fields in a synthetic multipage PDF and replace repeated values consistently. Preserve the page layout and check that the original identifiers are absent from the saved PDF's text. |
| [02 — Re-identification risk](02_Reidentification_Risk.ipynb) | Link unnamed hospital records to a named demographic table using birth year, postal code and sex. Generalize these fields and compare successful matches and the sizes of groups sharing the same values. |
| [03 — Differential privacy](03_Differential_Privacy.ipynb) | Reconstruct diagnoses from count queries, then add Laplace noise and compare reconstruction accuracy and count error. Track the accumulated privacy budget and reject queries when that budget is exhausted. |
| [04 — Federated learning](04_Federated_Learning.ipynb) | Compare local, pooled and federated training across four hospitals. Test how mean and median aggregation handle a corrupted update, with optional experiments using FedProx and FedAdam. |
| [05 — Homomorphic encryption](05_Homomorphic_Encryption.ipynb) | Encrypt patient inputs, run a decision-tree prediction on encrypted data and decrypt the result. Compare predictions and execution times, with an optional decision-tree versus logistic-regression experiment. |

## Run

Use **Python 3.11** and open the notebooks in Jupyter or VS Code. Run the setup cell, restart the kernel if requested, then run all cells in order.

Use separate environments: `requirements-core.txt` for notebooks 01–04 and `requirements-he.txt` for notebook 05. Notebook 05 requires macOS or Linux (WSL on Windows).

Internet access is needed for initial setup and dataset downloads. Notebooks 04–05 download the [UCI Heart Disease dataset](https://doi.org/10.24432/C52P4X) automatically and verify its hashes. Results are generated locally. The extra comparisons in 04 and 05 are optional.

## Code co-created by

Ülkü Tuncer Küçüktaş · Simge Danışoğlu · Tolga Turan · Gizem Acer
