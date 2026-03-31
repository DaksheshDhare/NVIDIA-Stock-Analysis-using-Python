<div align="center">
  <h1>📈 NVIDIA Stock Analysis (2021-2026)</h1>
  <p><em>A comprehensive exploratory data analysis and feature engineering project on NVIDIA's historical stock performance.</em></p>
  
  ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
  ![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
  ![Jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
</div>

<hr>

## 📖 Overview
This project dives deep into NVIDIA's stock data from **2021 to 2026**. Through rigorous **data cleaning, feature engineering, and exploratory data analysis (EDA)**, we uncover crucial market insights. Whether you are a short-term trader mapping volatility or a long-term investor looking for macro trends, this analysis provides data-backed clarity.

## 📁 Project Structure

| File | Description |
|------|-------------|
| 📊 `NVIDIA.csv` | Historical daily stock dataset containing Open, High, Low, Close, Volume, and Change %. |
| 📓 `NVIDIA.ipynb` | The core Jupyter Notebook containing execution steps for data preparation, EDA, and decision modeling. |

## 🚀 Methodology

### 1️⃣ Data Cleaning & Preparation
- **Temporal Alignment:** Formatted the `Date` column into continuous datetime objects.
- **Data Integrity:** Identified and mitigated missing and duplicate values.
- **Normalization:** 
  - Converted string-based trading `Volume` ("M" for Millions, "B" for Billions) into precise numeric structures.
  - Stripped percentage symbols from the `Change %` column for mathematical operations.

### 2️⃣ Feature Engineering
To better understand price movements beyond basic candlestick metrics, we engineered new indicators:
- 📈 **Daily Return:** Tracked day-to-day percentage shifts in closing price.
- 🔄 **Moving Averages (MA50 & MA200):** Smoothed out long-term and short-term momentum signals.
- 📉 **Volatility:** Measured via 30-day rolling standard deviation of returns.
- 📏 **Intraday Price Range:** Calculated absolute variance between daily Highs and Lows.

### 3️⃣ Exploratory Data Analysis (EDA)
Using `matplotlib` and `seaborn`, we visualized:
- Overall Price Trend Trajectory (2021-2026).
- Crossover points between MA50 & MA200.
- Daily Returns distributions to understand market behavior.
- Volatility fluctuations natively correlated with macroeconomic events.
- Feature Correlation Heatmaps indicating variable dependencies.

---

## 💡 Key Insights & Strategic Decisions

> **Long-Term Outlook: Strong Upward Trend 📈**
> Consistent year-over-year gains make NVDA an excellent candidate for a *Buy & Hold* portfolio.

> **Momentum Indicators: The Golden Crossover 💠**
> The 50-day moving average staying fundamentally above the 200-day average confirms extreme bullish momentum.

> **Trading Opportunities: Volatility Clusters ⚡**
> High intraday activity presents lucrative localized swings, perfect for short-term and swing traders.

> **Risk Mitigation: Heavy Fluctuations 🛡️**
> Due to the inherent high-risk/high-reward profile, implementing tight *stop-losses* and maintaining diversified portfolios remains necessary.

---

## ⚙️ Getting Started

### Prerequisites
Ensure you have the required Python libraries installed:
```bash
pip install pandas numpy matplotlib seaborn
```

### Execution
1. Clone the repository or ensure `NVIDIA.csv` is in the same directory as the notebook.
2. Open `NVIDIA.ipynb` in [Jupyter Notebook](https://jupyter.org/), [JupyterLab](https://jupyter.org/), or [VS Code](https://code.visualstudio.com/).
3. Run the cells sequentially to reproduce the visualizations and insights.

<hr>
<p align="center"><i>Data insights driven by quantitative analysis and historical trends.</i></p>
