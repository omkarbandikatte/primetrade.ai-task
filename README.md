# 📊 Trader Behavior Insights: Market Sentiment vs Performance

## 📌 Problem Statement

The objective of this project is to analyze how **Bitcoin market sentiment** (Fear–Greed Index) influences **trader behavior and performance** on the Hyperliquid platform.
By combining **daily sentiment data** with **trade-level execution data**, this analysis aims to uncover behavioral patterns and derive **actionable trading strategy insights**.

---

## 📂 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset

* Source: Fear–Greed Index
* Granularity: Daily
* Key Columns:

  * `date`
  * `classification` (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

### 2️⃣ Hyperliquid Historical Trader Data

* Granularity: Trade-level
* Key Columns:

  * `Account`
  * `Coin`
  * `Execution Price`
  * `Size USD`
  * `Side` (Buy/Sell)
  * `Timestamp IST`
  * `Closed PnL`
  * `Fee`

---

## 🧪 Methodology

1. Cleaned and standardized timestamps across both datasets
2. Converted trade timestamps to daily granularity
3. Merged trade data with daily sentiment labels using a left join
4. Conducted sentiment-wise performance and behavioral analysis
5. Analyzed trader-level performance across sentiment regimes
6. Visualized distributions and key metrics
7. Derived actionable strategy recommendations

---

## 📊 Key Analyses Performed

* **Profitability Analysis**

  * Average Closed PnL by sentiment
  * Trade win rate by sentiment

* **Risk & Behavior Analysis**

  * Trade size (USD) by sentiment
  * Trading fees as a proxy for activity
  * Buy vs Sell behavior across sentiment regimes

* **Trader-Level Intelligence**

  * Identification of sentiment-agnostic vs regime-dependent traders

---

## 📈 Visualizations Included

* Boxplot: Closed PnL vs Market Sentiment
* Bar Chart: Average Closed PnL by Sentiment
* Histogram: Overall Closed PnL Distribution
* Bar Chart: Average Trade Size (USD) by Sentiment

These visualizations highlight how profitability, volatility, and risk appetite vary across market conditions.

---

## 🧠 Key Insights

* **Extreme Greed** delivers the highest average PnL and win rate, driven by strong market momentum.
* **Fear** regimes show relatively strong performance with larger average trade sizes, suggesting disciplined and high-conviction trading.
* **Greed** phases exhibit increased activity but lower win rates, indicating potential overconfidence.
* **Extreme Fear** and **Neutral** periods show reduced profitability and conviction.
* Buy and sell behavior remains largely balanced, with slight selling bias during Extreme Greed due to profit-taking.
* A subset of traders performs consistently well across all sentiment regimes, indicating adaptive or robust strategies.

---

## 🚀 Actionable Strategy Recommendations

* **Momentum Trading in Extreme Greed**
  Deploy short-term momentum strategies with strict risk controls.

* **High-Conviction Accumulation During Fear**
  Focus on selective trades with moderate leverage and wider stop-loss buffers.

* **Reduced Exposure in Neutral Markets**
  Lower trade frequency and position size to avoid noise-driven losses.

* **Risk Controls During Greed**
  Apply stricter entry criteria and reduced leverage to mitigate volatility.

* **Trader Segmentation**
  Allocate capital preferentially to sentiment-agnostic traders and limit exposure to regime-dependent traders outside optimal conditions.

---

## ⚠️ Limitations & Assumptions

* Sentiment data is daily and may not capture intraday market psychology.
* Leverage and liquidation events were not explicitly modeled.
* Results are based on historical data and may not generalize to future market conditions.

---

## 🏁 Conclusion

Market sentiment plays a significant role in shaping trader behavior and performance.
While Greed-driven markets offer higher upside, they also introduce greater volatility.
Fear regimes, though less aggressive, demonstrate disciplined and conviction-based trading.
Incorporating sentiment awareness into trading systems can meaningfully improve **risk-adjusted returns**.

---

## 🛠️ Tools & Technologies

* Python
* Pandas
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 📁 Project Structure

```
├── task-ds.ipynb
├── README.md
```

---

## 👤 Author

**Omkar Bandikatte**
Junior Data Scientist Applicant – Trader Behavior Insights

