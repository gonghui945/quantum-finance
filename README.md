# Quantum Finance Notebooks

This repository contains the curated Jupyter notebooks that support the review paper
`Quantum Computing for Financial Transformation: A Unified Review of Optimisation, Pricing, Risk, Machine Learning, and Post-Quantum Security`.

The repository is deliberately notebook-only. It is intended to provide the executable layer that sits behind the empirical case studies discussed in the paper, without duplicating the full manuscript source.

## Repository structure

- `module_01_optimisation/`
  - `module_01_classical_vs_qaoa_portfolio.ipynb`
- `module_02_pricing/`
  - `module_02_asian_option_qae.ipynb`
- `module_03_risk/`
  - `module_03_single_asset_var_cvar.ipynb`
  - `module_03_multi_asset_var_cvar.ipynb`
- `module_04_qml/`
  - `module_04_case_a_quantum_classification.ipynb`
  - `module_04_case_b_macro_regime_learning.ipynb`

## How this repository maps to the paper

The paper uses article-style section numbering while retaining the original module labels. The notebook mapping is:

- `module_01_optimisation/module_01_classical_vs_qaoa_portfolio.ipynb`
  - Corresponds to Module 1 / Section 2 of the paper.
  - Supports the subsection `Reproducible Local Case: Classical Search versus QAOA on U.S. Equity Data`.

- `module_02_pricing/module_02_asian_option_qae.ipynb`
  - Corresponds to Module 2 / Section 3 of the paper.
  - Supports the subsection `Case Illustration: Quantum Pricing of an Asian Option`.

- `module_03_risk/module_03_single_asset_var_cvar.ipynb`
  - Corresponds to Module 3 / Section 4 of the paper.
  - Supports the single-asset case within `Case Illustrations`.

- `module_03_risk/module_03_multi_asset_var_cvar.ipynb`
  - Corresponds to Module 3 / Section 4 of the paper.
  - Supports the multi-asset case within `Case Illustrations`.

- `module_04_qml/module_04_case_a_quantum_classification.ipynb`
  - Corresponds to Module 4 / Section 5 of the paper.
  - Supports `Case A: asset-return direction prediction`.

- `module_04_qml/module_04_case_b_macro_regime_learning.ipynb`
  - Corresponds to Module 4 / Section 5 of the paper.
  - Supports `Case B: market-macro regime classification`.

## Scope and limitations

- The manuscript source, figures, and appendix assets are not duplicated here.
- Module 5 is not represented by a standalone notebook because the post-quantum cryptography section is documentary and architecture-focused rather than notebook-driven.
- Some notebooks are intended as reproducible research prototypes rather than production code.

## Intended use

This repository is designed for:

- readers who want to inspect or rerun the computational case studies;
- collaborators extending the benchmark notebooks;
- future linking from the review paper's appendix and reproducibility notes.
