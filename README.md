# Trader Behavior Insights Based on Market Sentiment

## Overview
This project analyzes how market sentiment (Fear vs Greed) impacts trader behavior and performance on the Hyperliquid trading platform.  
The goal is to uncover behavioral patterns and translate them into actionable trading strategies.

## Datasets
1. **Bitcoin Market Sentiment (Fear/Greed)**
   - Daily sentiment classification (Fear, Greed)
2. **Hyperliquid Historical Trader Data**
   - Trade-level data including account, timestamp, size, leverage, and closed PnL

---

## Project Structure
├── Market Sentiment Analysis.ipynb
├── data/
│ ├── trader_data.csv
│ └── sentiment_data.csv
├── outputs/
│ ├── pnl_by_sentiment.png
│ ├── behavior_by_sentiment.png
│ └── segment_analysis.png
├── README.md


## Project Objective

To explore how trader behavior (profitability, volume, trade direction, risk) aligns with overall crypto market sentiment. Key questions include:

- Do traders earn more in Greed than Fear?
- Is there more risk-taking in certain sentiments?
- Are there predictable behavior patterns?


## Datasets Used

1. **Hyperliquid Trader Data**
   - Fields: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Closed PnL`, `Timestamp`, etc.

2. **Bitcoin Fear & Greed Index**
   - Fields: `Date`, `Classification` (Fear, Greed, Extreme Greed, etc.)


## Key Steps

- Cleaned and formatted timestamp columns
- Merged both datasets by date
- Performed exploratory data analysis (EDA)
- Created visualizations to compare behavior across sentiments

How to Run

Place datasets in the data/ folder

Open the notebook:

jupyter notebook "Market Sentiment Analysis.ipynb"

Run all cells from top to bottom

Generated charts will be saved in the outputs/ directory

## Visuals & Insights

- Boxplot of Closed PnL across sentiments
<img width="1000" height="600" alt="closed_pnl_by_sentiment" src="https://github.com/user-attachments/assets/e1fe7193-af72-4355-904b-859d3111b483" />

- Buy vs Sell trade volume
  <img width="1000" height="600" alt="buy_sell_by_sentiment" src="https://github.com/user-attachments/assets/708777d9-cdbe-4e86-a2bd-dd0d0d992292" />

- % of High-Risk Trades in each sentiments
  <img width="800" height="500" alt="high_risk_trades" src="https://github.com/user-attachments/assets/2810b142-7bf6-4f93-8b31-446b7fed7673" />

- Top Performing Traders chart
  <img width="1000" height="500" alt="top_10_traders" src="https://github.com/user-attachments/assets/81d19922-febc-41f6-9b28-11ff4c03924e" />

- Weekly trend of average PnL
  <img width="1000" height="500" alt="pnl_weekly_trend" src="https://github.com/user-attachments/assets/4b151829-7717-4849-aafe-593c7452b266" />
  The weekly average PnL chart shows sharp drawdowns during Fear regimes, highlighting elevated downside risk compared to Greed periods.

All visuals are saved in the `outputs/` folder.


## Final Report

See `ds_report.pdf` for a detailed summary of:
- Cleaning steps
- Charts
- Insights
- Final conclusions


## Tools Used

- Python (Pandas, Matplotlib, Seaborn)
- Jupyter Notebook
- GitHub
- Google Docs (for PDF report)

## Methodology

1. We analyzed the relationship between market sentiment (Fear vs Greed) and trader behavior using Hyperliquid historical trade data combined with a Bitcoin Fear & Greed Index.
2. Trade-level data was cleaned, timestamps were normalized, and metrics were aggregated to a daily trader level.
3. Key performance and behavioral metrics were computed and aligned with daily sentiment labels.
4. We then compared performance across sentiment regimes and segmented traders by leverage, frequency, and consistency.

## Key Insights (Backed by Charts & Tables)

*Insight 1: Performance differs significantly by sentiment*

- Traders achieve higher average PnL and win rates during Greed days

- Fear days show lower median PnL, indicating higher drawdown risk

*Insight 2: Trader behavior changes with sentiment*

- Trade frequency, leverage, and position size increase during Greed

- Fear days trigger defensive behavior (lower leverage, fewer trades)

*Insight 3: Risk impacts segments unevenly*

- High-leverage traders outperform during Greed but suffer large losses during Fear

- Consistent winners maintain stable performance across sentiment regimes

## Strategy Recommendations (Actionable Output)

*Strategy 1: Sentiment-Aware Risk Control*

During Fear days, reduce leverage and trade frequency for high-leverage or high-frequency traders to limit drawdowns.

*Strategy 2:Greed-Regime Stability Exploitation*

During Greed days, allow higher leverage and increased trade frequency only for traders with historically high win rates.

## Conclusion

Market sentiment plays a critical role in shaping trader behavior and profitability.
Incorporating sentiment awareness into risk management and strategy design can meaningfully improve trading outcomes, particularly during volatile market regimes.
