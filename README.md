---
language:
- en
license: mit
pretty_name: Cancer Abstract Dataset
size_categories:
- 1K<n<10K
tags:
- biomedical
- oncology
- cancer
- text-classification
- nlp
- graph-neural-networks
- document-classification
task_categories:
- text-classification
---

# Cancer Abstract Dataset

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![DOI](https://img.shields.io/badge/DOI-10.1038%2Fs41598--026--39894--6-blue)](https://doi.org/10.1038/s41598-026-39894-6)
[![Dataset](https://img.shields.io/badge/HuggingFace-Dataset-orange)](https://huggingface.co/datasets/EliasHossain/CancerAbstracts)

## Overview

The **Cancer Abstract Dataset** is a curated collection of 1,874 biomedical research abstracts annotated by cancer type. Developed to support document classification, low-resource biomedical NLP, and graph-based deep learning research, this dataset serves as the benchmark resource for the following peer-reviewed publication:

> Hossain, E., Nuzhat, T., Masum, S., et al.
> **R-GAT: Cancer Document Classification Leveraging Graph-Based Residual Network for Scenarios with Limited Data.**
> *Scientific Reports*, 16, 6582 (2026).
> https://doi.org/10.1038/s41598-026-39894-6

---

## Dataset Description

| Property        | Value                          |
|----------------|--------------------------------|
| Total Samples   | 1,874 abstracts                |
| Format          | CSV                            |
| Language        | English                        |
| Domain          | Biomedical / Oncology          |
| Task            | Text Classification            |
| License         | MIT                            |

### Schema

| Field      | Type   | Description                      |
|------------|--------|----------------------------------|
| `Abstract` | string | Full research abstract text      |
| `Category` | string | Cancer type label (see below)    |

### Class Labels

| Label            | Description                          |
|------------------|--------------------------------------|
| `Lung_Cancer`    | Abstracts related to lung cancer     |
| `Thyroid_Cancer` | Abstracts related to thyroid cancer  |
| `Colon_Cancer`   | Abstracts related to colon cancer    |
| `Generic`        | General oncology abstracts           |

---

## Usage

```python
from datasets import load_dataset

dataset = load_dataset("EliasHossain/CancerAbstracts")
print(dataset["train"][0])
```

---

## Intended Use

This dataset is designed for academic and research purposes, including:

- Supervised biomedical text classification
- Graph neural network (GNN) research
- Transformer-based fine-tuning in low-resource settings
- Biomedical NLP benchmarking
- Uncertainty-aware language model evaluation

> **⚠️ Important:** This dataset is strictly intended for research use and is **not suitable for clinical decision-making or diagnostic purposes**.

---

## Data Collection & Ethics

Abstracts were systematically curated from publicly available biomedical literature and annotated by cancer type. Standard preprocessing was applied to ensure formatting consistency across samples.

- No personally identifiable information (PII) is included.
- No protected health information (PHI) is included.
- All source material is publicly available.

---

## Citation

If you use this dataset in your research, please cite the following paper:

```bibtex
@article{hossain2026rgat,
  title     = {R-GAT: Cancer Document Classification Leveraging Graph-Based Residual Network for Scenarios with Limited Data},
  author    = {Hossain, Elias and Nuzhat, Tasfia and Masum, S. and others},
  journal   = {Scientific Reports},
  volume    = {16},
  pages     = {6582},
  year      = {2026},
  publisher = {Nature Publishing Group},
  doi       = {10.1038/s41598-026-39894-6},
  url       = {https://doi.org/10.1038/s41598-026-39894-6}
}
```

---

## Contributors

| Name | Affiliation |
|------|-------------|
| **Elias Hossain** | Mississippi State University, USA |
| **Tasfia Nuzhat** | Chittagong Independent University, Bangladesh |

---

## License

This dataset is released under the [MIT License](https://opensource.org/licenses/MIT). See `LICENSE` for details.
