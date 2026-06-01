# Trader Performance vs Market Sentiment Analysis

## Primetrade.ai Data Science Intern Round-0 Assignment

### Objective

The objective of this project is to analyze the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader behavior on Hyperliquid. By combining market sentiment data with historical trading activity, the analysis aims to identify behavioral patterns, performance differences, and actionable trading insights.

### Dataset Overview

#### Dataset 1: Bitcoin Fear & Greed Index

* Date
* Sentiment Classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)

#### Dataset 2: Hyperliquid Historical Trader Data

* Account
* Side
* Size USD
* Closed PnL
* Fee
* Timestamp
* Additional trading attributes

### Methodology

1. Loaded and explored both datasets.
2. Checked for missing values and duplicate records.
3. Converted timestamps to a common daily date format.
4. Merged trading data with sentiment data using date alignment.
5. Created performance and behavioral metrics:

   * Average PnL
   * Win Rate
   * Trade Frequency
   * Trade Size
   * Long/Short Distribution
6. Segmented traders based on trading activity.
7. Applied K-Means clustering to identify trader archetypes.
8. Generated visualizations and extracted actionable insights.

### Key Findings

* Trader profitability was highest during Greed and Extreme Greed periods.
* Average trade sizes increased during optimistic market conditions, indicating higher risk appetite.
* Frequent traders generated significantly higher cumulative profits than infrequent traders.
* Clustering analysis revealed distinct trader groups with different participation and profitability characteristics.

### Strategy Recommendations

#### Strategy 1: Momentum Participation

During Greed and Extreme Greed periods, traders may increase participation and position sizes while maintaining proper risk controls, as profitability tends to be higher during these regimes.

#### Strategy 2: Defensive Risk Management

During Fear and Extreme Fear periods, traders should reduce exposure, focus on high-conviction trades, and apply stricter risk management practices.

### How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter

jupyter notebook
```

Open:

```text
trader_sentiment_analysis.ipynb
```

and run all cells sequentially.
