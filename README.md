# Crypto Sentiment vs Trader Behavior Analysis

## Objective

Analyze how market sentiment (Fear/Greed Index) impacts trader behavior and performance on Hyperliquid.
The goal is to uncover patterns that can inform **data-driven trading strategies**.

---

## Dataset

We used two datasets:

1. **Bitcoin Market Sentiment (Fear/Greed Index)**

   * Columns: Date, Classification (Fear, Greed, etc.)

2. **Historical Trader Data (Hyperliquid)**

   * Includes: account, symbol, execution price, size, side, timestamp, closed PnL, etc.

---

## Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/Tanujk01/crypto-sentiment-analysis.git
cd crypto-sentiment-analysis
```

### 2. Install dependencies

```bash
pip install pandas numpy matplotlib seaborn plotly
```

---

## How to Run

### Option 1: Jupyter Notebook

```bash
jupyter notebook
```

* Open `notebook.ipynb`
* Run all cells step by step

##  Data Preparation

* Loaded both datasets using pandas
* Checked for missing values and duplicates
* Converted timestamps to datetime format
* Aligned both datasets on **daily level**
* Merged datasets on `date`

---

## Metrics 

* Daily PnL
* Win Rate
* Average Trade Size
* Number of Trades per Day
* Long/Short Ratio

## Analysis Performed

### 1. Sentiment vs Performance

* Compared **PnL and win rate** across Fear, Greed, and Neutral conditions

### 2. Behavioral Analysis

* Trade frequency
* Trade size variation
* Long vs short bias

### 3. Trader Segmentation

* High Activity vs Low Activity traders
* Compared performance across sentiment conditions

## Key Insights

* Highest PnL observed during **Extreme Fear**, indicating strong contrarian opportunities
* Win rate highest during **Extreme Greed**, suggesting trend-following works better
* Traders tend to **overtrade during Fear**, reducing efficiency
* **Low activity traders outperform high-frequency traders** in Greed markets

## Strategy Recommendations

### 1. Contrarian Strategy in Fear Markets

* Enter during Fear phases
* Use smaller position sizes
* Avoid overtrading
* Focus on high-quality setups

### 2. Low-Frequency Strategy in Greed Markets

* Trade less but with higher conviction
* Follow trend (momentum-based trades)
* Avoid excessive entries/exits

## Tech Stack

* Python
* Pandas
* Seaborn & Matplotlib

## Author
Tanuj

---
