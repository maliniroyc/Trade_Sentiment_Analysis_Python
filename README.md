# Trade_Sentiment_Analysis_Python

*Data Overview*
--------------
This project analyzes the relationship between trader performance and Bitcoin market sentiment (Fear/Greed). It aims to uncover patterns that can guide trading strategies in Web3 markets.
I analyze trade sentiments using two data sources, both available at the following link: https://docs.google.com/document/d/1ZyM5IBD459ulv1pMM1GYQ3SmMYezrVlygRmp3RRHLCI/edit?tab=t.0

Total Trades Analyzed: 184,263 trades <br>
Sentiment Categories: Extreme Greed, Greed, Neutral, Fear <br>
Data Sources: Historical trader data + Fear & Greed Index <br>

**Tools & Libraries**
------
Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

**Key Steps**
-----------
Data Cleaning:
- Parsed timestamps
- Filtered out erroneous/unusable rows
- Removed trades outside sentiment data range
  
Data Merging:
- Joined trader data with sentiment classification on the date field

Exploratory Data Analysis (EDA):
- Trade volume by sentiment classification
- Average profit/loss under Fear vs Greed conditions

*Key Insights*
--------------    
**Performance by Sentiment:**

Greed > Fear > Extreme Greed > Neutral

- Greed periods show the highest average PnL ($87.89) 

- Fear periods show moderate performance ($50.05) 

- Extreme Greed and Neutral show lower returns

**Win Rate Analysis:**
- No sentiment category exceeds 50% win rate

- Extreme Greed has the highest win rate (49%)

- Neutral periods have the lowest win rate (31.7%)

**Trade Behavior:**
- Traders use larger positions during Extreme Greed ($5,660 avg) 

- Smaller positions during Neutral sentiment ($3,059 avg)

- Trade size correlates with sentiment intensity

**Trading Strategy Implications**
- Optimal Conditions: Greed periods offer best profit potential
- Risk Management: Extreme sentiment may indicate market tops/bottoms
- Position Sizing: Consider adjusting trade size based on sentiment
- Timing: Greed phases might be good for taking profits

**Limitations**
- Data covers limited time period
- Sentiment data might have reporting delays
- Individual trader strategies vary significantly

**Result**
---------
This analysis suggests that market sentiment can be a valuable indicator for timing trades and managing position sizes, though it should be used in conjunction with other technical and fundamental analysis tools.
