# Large-Language-Models-for-Math-Education-in-Low-Resource-Languages-A-Study-in-Sinhala-and-Tamil

This repository provides a parallel trilingual dataset of mathematical word problems in English, Sinhala, and Tamil. The dataset is designed to evaluate the mathematical reasoning capabilities of Large Language Models (LLMs), particularly in low-resource language settings.

The dataset accompanies our research paper:

**Large Language Models for Math Education in Low-Resource Languages: A Study in Sinhala and Tamil**

[Read the paper on arXiv](https://arxiv.org/abs/2602.14517)

## Dataset Overview

The dataset contains 450 mathematical word-problem instances across three languages: English, Sinhala, and Tamil.

It covers six mathematical problem categories, with 25 problems per category per language.

| Mathematical Problem Category | English | Sinhala |   Tamil |   Total |
| ----------------------------- | ------: | ------: | ------: | ------: |
| Single-Step                   |      25 |      25 |      25 |      75 |
| Multi-Step                    |      25 |      25 |      25 |      75 |
| Extraneous Information        |      25 |      25 |      25 |      75 |
| Unit Conflict                 |      25 |      25 |      25 |      75 |
| Logical Deduction             |      25 |      25 |      25 |      75 |
| Optimization                  |      25 |      25 |      25 |      75 |
| **Total**                     | **150** | **150** | **150** | **450** |

## Dataset Construction

Problems were natively authored in English, Sinhala, and Tamil rather than translated from existing benchmarks. Semantic equivalence across language versions was verified without requiring word-for-word correspondence, preserving natural language expressions.

The dataset comprises six mathematical problem categories, with 25 problems per category per language, resulting in 450 instances.

## Dataset File

The dataset is provided as a single Excel workbook:

`data/trilingual_math_reasoning_dataset.xlsx`

The workbook contains mathematical word problems in English, Sinhala, and Tamil.

## Mathematical Problem Categories

The dataset includes the following six categories:

1. **Single-Step(Category 1):** Problems requiring a single mathematical operation or reasoning step.
2. **Multi-Step(Category 2):** Problems requiring multiple mathematical operations or sequential reasoning.
3. **Extraneous Information(Category 3):** Problems containing irrelevant information that must be identified and disregarded.
4. **Unit Conflict(Category 4):** Problems involving conflicting or inconsistent measurement units that require appropriate handling.
5. **Logical Deduction(Category 5):** Problems requiring logical reasoning to derive the correct answer.
6. **Optimization(Category 6):** Problems requiring the identification of an optimal solution under given conditions.

## Intended Use

This dataset is intended to support research in:

- Evaluating mathematical reasoning capabilities of LLMs across multiple languages.
- Comparing mathematical reasoning performance between high-resource and low-resource languages.
- Investigating the impact of language on mathematical problem-solving.
- Analysing LLM performance across different mathematical problem categories.
- Advancing multilingual NLP research for Sinhala and Tamil.

## Usage

The dataset can be downloaded directly from the `data/` directory.

It can also be loaded using Python and pandas:

```python
import pandas as pd

# Load the Excel dataset
df = pd.read_excel(
    "data/trilingual_math_reasoning_dataset.xlsx"
)

print(df.head())
```

If the workbook contains multiple sheets, specify the required sheet using the `sheet_name` parameter.

## Citation

**If you use this dataset in any research publication, scientific study, benchmark evaluation, or other academic work, you must cite the accompanying research paper.**

Please use the following BibTeX citation:

```bibtex
@misc{kishanthan2026mathreasoning,
  title={Large Language Models for Math Education in Low-Resource Languages: A Study in Sinhala and Tamil},
  author={Kishanthan, Sukumar and Thushalika, Kumar and Jayasekara, Buddhi and Hevapathige, Asela},
  year={2026},
  eprint={2602.14517},
  archivePrefix={arXiv},
  primaryClass={cs.CL}
}
```



## License

This dataset is released under the **Creative Commons Attribution 4.0 International (CC BY 4.0)** license.

You are free to share and adapt this dataset for any purpose, including commercial use, provided that appropriate credit is given to the original authors, a link to the license is provided, and any changes are indicated.

For further details, see the [CC BY 4.0 License](https://creativecommons.org/licenses/by/4.0/).

## Acknowledgements

We acknowledge everyone who contributed to the development, validation, and evaluation of this dataset.

## Contact

For questions, feedback, or collaboration opportunities related to this dataset, please refer to the corresponding authors listed in the accompanying research paper.
