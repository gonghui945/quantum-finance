# Quantum Finance Computational Assets

This repository contains the public computational companion to the review paper on quantum computing in finance. It collects the executable notebooks and supporting data assets used for the paper's empirical sections on optimisation, derivatives pricing, risk estimation, and quantum machine learning.

The manuscript source, LaTeX figures, and broader drafting materials are maintained separately. This repository is intended to give readers a clean entry point to the reproducible case-study assets.

## Scope

The repository is organised by module. Each top-level folder corresponds to one technical part of the paper and groups the notebook together with the files needed to inspect the reported example.

- `module_01_optimisation`: local classical-versus-QAOA portfolio benchmark.
- `module_02_pricing`: Asian-option pricing example based on quantum amplitude estimation.
- `module_03_risk`: single-asset and multi-asset VaR/CVaR case studies.
- `module_04_qml`: supervised-learning case studies for market direction and macro-regime classification.

Module 5 in the paper is policy- and architecture-driven rather than notebook-driven, so it is not represented here as a standalone computational package.

## Repository Structure

### `module_01_optimisation`

Files in this package:

- `module_01_classical_vs_qaoa_portfolio.ipynb`
- `AAPL_2024-01-01_2025-11-21_daily.csv`
- `AMD_2024-01-01_2025-11-21_daily.csv`
- `AMGN_2024-01-01_2025-11-21_daily.csv`
- `COST_2024-01-01_2025-11-21_daily.csv`
- `CSX_2024-01-01_2025-11-21_daily.csv`
- `GOOGL_2024-01-01_2025-11-21_daily.csv`
- `module_01_qaoa_frontier.csv`
- `module_01_qaoa_portfolio_summary.csv`

Purpose:

- reproduces the small-scale portfolio-selection benchmark used to compare exact classical search with a QAOA-based formulation;
- exposes the ranked feasible portfolios and the summary table used in the paper;
- keeps the underlying market inputs visible for later auditing.

### `module_02_pricing`

Files in this package:

- `module_02_asian_option_qae.ipynb`
- `module_02_asian_option_histogram.csv`
- `module_02_asian_option_pricing_summary.csv`
- `module_02_asian_option_parameters.json`

Purpose:

- reproduces the Asian-option pricing case study;
- records the discretised payoff histogram, parameter choices, and summary outputs used in the manuscript;
- provides a compact example of a hybrid quantum-amplitude-estimation workflow.

### `module_03_risk`

Files in this package:

- `module_03_single_asset_var_cvar.ipynb`
- `module_03_multi_asset_var_cvar.ipynb`
- `AAPL_2024-01-01_2025-11-21_daily.csv`
- `MSFT_2024-01-01_2025-11-21_daily.csv`
- `GOOGL_2024-01-01_2025-11-21_daily.csv`
- `AMZN_2024-01-01_2025-11-21_daily.csv`
- `module_03_single_asset_var_cvar_summary.csv`
- `module_03_multi_asset_var_cvar_summary.csv`
- `module_03_risk_data_manifest.json`

Purpose:

- supports the single-asset and multi-asset VaR/CVaR demonstrations;
- includes the local market extracts used by the current public snapshot;
- records summary statistics and simulation settings so the risk examples can be checked independently of the paper text.

### `module_04_qml`

Files in this package:

- `module_04_case_a_quantum_classification.ipynb`
- `module_04_case_b_macro_regime_learning.ipynb`
- `module_04_case_a_data_manifest.json`
- `module_04_case_b_data_manifest.json`
- `README.md`

Purpose:

- supports the quantum machine learning section of the paper;
- separates the SPY direction-classification case from the macro-regime classification case;
- records the data-acquisition assumptions through manifests in the current public snapshot.

## Mapping to the Paper

The review paper uses `Section 0` for the introduction and then aligns the main technical sections with the original module labels.

- `module_01_optimisation` maps to Module 1 / Section 1.
- `module_02_pricing` maps to Module 2 / Section 2.
- `module_03_risk` maps to Module 3 / Section 3.
- `module_04_qml` maps to Module 4 / Section 4.
- Module 5 / Section 5 is reference-driven and therefore has no standalone code package in this repository.

## Reproducibility Notes

- The notebooks are curated research assets rather than production pipelines.
- Modules 1 and 3 include market-data extracts in the current public snapshot.
- Module 2 includes simulated pricing outputs exported from the executed notebook.
- Module 4 currently preserves reproducibility through notebooks and data manifests; in this public snapshot, the underlying market and macro data are not fully mirrored as static CSV bundles.
- The local manuscript working tree may evolve beyond the exact snapshot published here. The repository should therefore be read as the public package state associated with the visible contents of this repository.

## Intended Use

This repository is designed for:

- readers who want to inspect the computational examples used in the paper;
- collaborators who want to rerun or extend the notebooks;
- future repository maintenance where manuscript appendix links point to stable public assets.

## Authors

Associated paper authors:

- Hui Gong

Affiliation:

- UCL IFT Center for Quantum Finance
