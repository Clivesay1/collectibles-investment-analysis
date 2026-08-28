# Data Notes

## Included Snapshot

This directory contains the committed inputs for the consolidated analysis notebook:

| File | Purpose |
|---|---|
| `annual_returns.csv` | Annual return series for the 12 modeled asset classes, 2000–2024. |
| `investment_summary.csv` | Summary metrics, including CAGR, volatility, and Sharpe ratio. |
| `portfolio_growth.csv` | Growth-of-$10,000 comparison series. |
| `asset_returns.csv` and `collectibles_data.csv` | Supporting source and intermediate data tables. |

The consolidated notebook identifies the project coverage period as **2000–2024** and cites Damodaran NYU, World Gold Council, Artprice, Liv-ex, Knight Frank, PWCC, PSA, TCGPlayer/MTGGoldfish, and StockX among its source materials.

## Reproducing the Analysis

1. Create a virtual environment and install the packages in the repository root with `pip install -r requirements.txt`.
2. Launch `jupyter notebook notebooks/collectibles_investment_analysis.ipynb` from the repository root.
3. Run cells in order. The notebook reads the committed source snapshot and writes derived tables to `output/`.

## Interpretation Limits

The dataset combines published indices and benchmarks rather than individual-item transactions. Costs such as auction fees, grading, storage, insurance, taxes, and liquidity constraints should be considered when interpreting results. Future refreshes should retain source citations, retrieval dates, and any changes to return methodology.
