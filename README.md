---
language:
- en
license: mit
pretty_name: Cancer Abstract Dataset
size_categories:
- 1K\<n\<10K
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
- text-mining
---

# Cancer Abstract Dataset

## Dataset Summary

The **Cancer Abstract Dataset** is a curated collection of biomedical
research abstracts categorized by cancer type. It was developed to
support research in document classification, low-resource biomedical
NLP, and graph-based deep learning approaches.

This dataset was introduced in the following publication:

> Hossain, E., Nuzhat, T., Masum, S., et al.\
> **R-GAT: cancer document classification leveraging graph-based
> residual network for scenarios with limited data.**\
> *Scientific Reports*, 16, 6582 (2026).\
> https://doi.org/10.1038/s41598-026-39894-6

------------------------------------------------------------------------

## Dataset Description

This dataset contains categorized research abstracts related to major
cancer types. It is suitable for:

-   Biomedical text classification
-   Topic modeling
-   Low-resource learning experiments
-   Graph-based NLP methods
-   Transformer-based fine-tuning
-   Benchmarking uncertainty-aware LLMs

------------------------------------------------------------------------

## Dataset Structure

### Total Samples

**1,874 abstracts**

### Format

CSV (Comma-Separated Values)

### Fields

  Field        Description
  ------------ -----------------------------
  `Abstract`   Full research abstract text
  `Category`   Cancer type label

### Categories

-   `Lung_Cancer`
-   `Thyroid_Cancer`
-   `Colon_Cancer`
-   `Generic`

------------------------------------------------------------------------

## Example Usage

``` python
from datasets import load_dataset

dataset = load_dataset("EliasHossain/CancerAbstracts")

print(dataset["train"][0])
```

------------------------------------------------------------------------

## Intended Use

The dataset is intended for:

-   Supervised text classification
-   Graph neural network research
-   Transformer-based fine-tuning
-   Biomedical NLP benchmarking
-   Limited-data learning evaluation

This dataset is **not intended for clinical decision-making**.

------------------------------------------------------------------------

## Data Collection and Processing

Abstracts were curated and categorized for research purposes in
oncology-related document classification experiments. Standard
preprocessing steps were applied to ensure formatting consistency.

No personally identifiable information (PII) or protected health
information (PHI) is included.

------------------------------------------------------------------------

## Citation

If you use this dataset, please cite:

``` bibtex
@article{hossain2026rgat,
  title={R-GAT: cancer document classification leveraging graph-based residual network for scenarios with limited data},
  author={Hossain, Elias and Nuzhat, Tasfia and Masum, S. and others},
  journal={Scientific Reports},
  volume={16},
  pages={6582},
  year={2026},
  doi={10.1038/s41598-026-39894-6}
}
```

------------------------------------------------------------------------

## Contributors

-   **Elias Hossain**\
    Mississippi State University, USA

-   **Tasfia Nuzhat**\
    Chittagong Independent University, Bangladesh

------------------------------------------------------------------------

## License

MIT License
