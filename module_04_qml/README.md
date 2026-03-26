# Module 4 Data Notes

This directory stores the local data snapshots and manifests for the two QML case studies.

- `SPY_2024-01-01_2025-12-31_daily.csv`: local SPY daily-price history shared by both notebooks.
- `FEDFUNDS_2024-01-01_2025-12-31.csv`, `CPIAUCSL_2024-01-01_2025-12-31.csv`, and `INDPRO_2024-01-01_2025-12-31.csv`: local FRED series used by the macro-regime notebook.
- `module_04_case_a_data_manifest.json`: SPY direction-classification manifest.
- `module_04_case_b_data_manifest.json`: market-and-macro regime-classification manifest.

The notebooks now read from these bundled CSV snapshots so that the manuscript's executed results are tied to a fixed two-year window from 1 January 2024 to 31 December 2025.
