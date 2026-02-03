# Trade_Sentiment_Analysis_Python

Trader Behavior Insights Based on Market Sentiment

This project analyzes how crypto traders behave under different market sentiments such as Fear, Greed, Extreme Greed, and Extreme Fear. It combines historical trading data from Hyperliquid with the Bitcoin Fear & Greed Index to uncover patterns that can help design smarter trading strategies.

## Folder Structure

├── outputs/
│ └── *.png visualizations (charts and plots)
├── ds_report.pdf 
└── README.md 


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


