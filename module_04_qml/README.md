# Module 4 Data Notes

This directory stores data manifests for the two QML case studies.

- `module_04_case_a_data_manifest.json`: market-data acquisition settings for the SPY direction-classification case.
- `module_04_case_b_data_manifest.json`: market and macro acquisition settings for the macro-regime case.

The raw data are fetched dynamically inside the notebooks via `yfinance` and `fredapi`; they were not vendored as static CSV files in the current revision.
