# Quantum Finance Computational Assets

This repository contains the executable and data assets that support the review paper
`Quantum Computing for Financial Transformation: A Unified Review of Optimisation, Pricing, Risk, Machine Learning, and Post-Quantum Security`.

The repository is organised by module so that each empirical section of the paper can be audited from a single package. The manuscript source and figure files are maintained separately; this repository is the public computational companion.

## Repository structure

### `module_01_optimisation`

- `module_01_classical_vs_qaoa_portfolio.ipynb`
- `AAPL_2024-01-01_2025-11-21_daily.csv`
- `AMD_2024-01-01_2025-11-21_daily.csv`
- `AMGN_2024-01-01_2025-11-21_daily.csv`
- `COST_2024-01-01_2025-11-21_daily.csv`
- `CSX_2024-01-01_2025-11-21_daily.csv`
- `GOOGL_2024-01-01_2025-11-21_daily.csv`
- `module_01_qaoa_frontier.csv`
- `module_01_qaoa_portfolio_summary.csv`

### `module_02_pricing`

- `module_02_asian_option_qae.ipynb`
- `module_02_asian_option_histogram.csv`
- `module_02_asian_option_pricing_summary.csv`
- `module_02_asian_option_parameters.json`

### `module_03_risk`

- `module_03_single_asset_var_cvar.ipynb`
- `module_03_multi_asset_var_cvar.ipynb`
- `AAPL_2024-01-01_2025-11-21_daily.csv`
- `MSFT_2024-01-01_2025-11-21_daily.csv`
- `GOOGL_2024-01-01_2025-11-21_daily.csv`
- `AMZN_2024-01-01_2025-11-21_daily.csv`
- `module_03_single_asset_var_cvar_summary.csv`
- `module_03_multi_asset_var_cvar_summary.csv`
- `module_03_risk_data_manifest.json`

### `module_04_qml`

- `module_04_case_a_quantum_classification.ipynb`
- `module_04_case_b_macro_regime_learning.ipynb`
- `module_04_case_a_data_manifest.json`
- `module_04_case_b_data_manifest.json`
- `README.md`

## Mapping to the paper

The manuscript uses `Section 0` for the introduction and then aligns the technical review with the original module labels. The repository mapping is:

- `module_01_optimisation`
  - Corresponds to Module 1 / Section 1.
  - Supports the local classical-versus-QAOA portfolio benchmark.

- `module_02_pricing`
  - Corresponds to Module 2 / Section 2.
  - Supports the Asian-option pricing case based on Quantum Amplitude Estimation.

- `module_03_risk`
  - Corresponds to Module 3 / Section 3.
  - Supports the single-asset and multi-asset VaR/CVaR case studies.

- `module_04_qml`
  - Corresponds to Module 4 / Section 4.
  - Supports the direction-classification and macro-regime learning case studies.

- Module 5 / Section 5 is policy- and architecture-driven rather than notebook-driven, so it is not represented by a standalone computational package in this repository.

## Reproducibility notes

- Module 1 and Module 3 include market-data extracts used by the current manuscript revision.
- Module 2 uses simulated pricing data exported from the executed notebook.
- Module 4 preserves reproducibility through notebooks plus data manifests; the underlying SPY and macroeconomic series are still downloaded dynamically at runtime.
- The repository is intended for methodological transparency and research reuse rather than production deployment.

## Intended use

This repository is designed for readers who want to inspect or rerun the computational case studies, collaborators extending the benchmark notebooks, and future appendix links from the review paper.
