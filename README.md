# Collectibles vs. Conventional Investments: A 25-Year ROI Analysis

**Do MTG cards, sports cards, and sneakers actually beat the stock market?**

This project analyzes 25 years of real return data (2000–2024) across 12 asset classes — 4 conventional investments and 8 collectible categories — to determine which offer the best risk-adjusted returns for the collector-investor.

## Key Results
- **MTG Cards** delivered a 13.7% CAGR vs. S&P 500's 7.7% over 25 years
- **$10,000 invested in MTG Cards in 2000 → ~$243,000 by 2024** (vs. $73,000 in S&P 500)
- **Comic Books** have the highest Sharpe ratio (0.947) of all 12 asset classes
- **Pokemon Cards** show the most volatility — 124% gain in 2021 followed by 42% crash in 2022
- **Fine Wine** offers the best combination of returns, low volatility, and inflation hedging

## Research Questions
1. Which asset classes delivered the highest CAGR from 2000–2024?
2. How do collectibles compare to the S&P 500 on a risk-adjusted basis?
3. Which collectibles have the best combination of returns, liquidity, and low minimum investment?
4. How did the pandemic bubble affect collectibles performance?
5. What is the optimal portfolio strategy for a collector-investor?

## Tech Stack
| Tool | Purpose |
|---|---|
| Python 3.11 | Core analysis |
| pandas | Data manipulation |
| matplotlib | Visualizations |
| numpy | Statistical calculations (CAGR, Sharpe, volatility) |

## Project Structure
```
collectibles-investment-analysis/
├── data/
│   ├── annual_returns.csv         # Year-by-year returns for all 12 assets
│   ├── investment_summary.csv     # CAGR, Sharpe, volatility, win rate
│   └── portfolio_growth.csv       # $10K portfolio simulation data
├── notebooks/
│   └── collectibles_investment_analysis.ipynb  # Full analysis notebook
├── images/
│   ├── 01_portfolio_growth.png
│   ├── 02_cagr_comparison.png
│   ├── 03_risk_return.png
│   ├── 04_sharpe_ratio.png
│   ├── 05_cagr_periods.png
│   └── 07_collectibles_deep_dive.png
├── output/
│   └── investment_comparison_full.csv
└── README.md
```

## How to Run
```bash
git clone https://github.com/Clivesay1/collectibles-investment-analysis
cd collectibles-investment-analysis
pip install pandas matplotlib numpy
jupyter notebook notebooks/collectibles_investment_analysis.ipynb
```

## Data Sources
| Asset | Source |
|---|---|
| S&P 500 | Damodaran NYU Historical Returns Database |
| Gold | World Gold Council / Macrotrends |
| Fine Art | Artprice Global Index |
| Fine Wine | Liv-ex Fine Wine 100 Index |
| Luxury Watches | Knight Frank Luxury Investment Index |
| Sports Cards | PWCC Market Index |
| MTG Cards | TCGPlayer / MTGGoldfish Market Index |
| Pokemon Cards | PSA Population Reports + TCGPlayer |
| Sneakers | StockX Annual Report + Cowen Research |

## Important Disclaimers
- Returns represent published index/benchmark performance, not individual item performance
- Transaction costs (10–25% auction fees, grading, storage) are not included and significantly impact real returns
- Past performance does not guarantee future results
- Individual card/item selection skill is the primary driver of returns above the index

---
*Author: Chris Livesay | [LinkedIn](https://www.linkedin.com/in/christopher-livesay)*
