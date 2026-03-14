# Analysis_Report

## Merged Dataset Link

You can access the full dataset used for this analysis [here](https://drive.google.com/drive/folders/1U5-wxppdOlS675JOJnJBvtIZEACllmgJ?usp=drive_link).


---


# Setup Guide: Anaconda Navigator & Jupyter Notebook

This guide explains how to install **Anaconda Navigator** and activate **Jupyter Notebook** for Python development.

---

## 📦 Step 1: Download and Install Anaconda

1. Go to the [Anaconda Distribution page](https://www.anaconda.com/products/distribution).
2. Download the installer for your operating system:
   - **Windows**: `.exe` installer
   - **macOS**: `.pkg` or `.sh` installer
   - **Linux**: `.sh` installer
3. Run the installer and follow the setup instructions.
   - On Windows, check **"Add Anaconda to my PATH environment variable"** if prompted.
   - On macOS/Linux, run the installer via terminal if using `.sh`.

---

## 🚀 Step 2: Launch Anaconda Navigator

- After installation, open **Anaconda Navigator**:
  - **Windows**: Search for *Anaconda Navigator* in the Start Menu.
  - **macOS/Linux**: Run `anaconda-navigator` from terminal.

---

## 📓 Step 3: Activate Jupyter Notebook

### Option A: Using Anaconda Navigator
1. In Anaconda Navigator, locate **Jupyter Notebook**.
2. Click **Launch**.
3. A browser window will open at `http://localhost:8888`.

### Option B: Using Terminal/Command Prompt
1. Open terminal (macOS/Linux) or Anaconda Prompt (Windows).
2. Run:

   ```bash
   jupyter notebook
   ```bash
   jupyter notebook
---

### Key insights

#### Q1. Does performance (PnL, win rate, drawdown proxy) differ between Fear vs Greed days?
![Answer 1 Screenshot](https://github.com/dhavltharkaaar/Analysis_Report/blob/main/images/summary.PNG)

### Key Insights
- **Fear days outperform Greed days** across most metrics (PnL, win rate, trade size, trade count).  
- Traders appear more active and take larger positions when sentiment is fearful.  
- **Drawdown proxy:** Higher win rate and average PnL suggest lower drawdown risk on Fear days compared to Greed days.  

👉 **Conclusion:** 
Market performance is stronger on **Fear days**, while Greed days still yield profits but with smaller trades, fewer executions, and lower win rates.
---
### Q2. Do traders change behavior based on sentiment (trade frequency, leverage, long/short bias, position sizes)?
![Answer 2 Screenshot](https://github.com/dhavltharkaaar/Analysis_Report/blob/main/images/pivot.PNG)

## Key Insights

**Higher activity in emotional markets**  
Total realized PnL is highest during **Fear** and **Extreme Greed**, indicating that traders are likely **closing more positions and realizing profits during volatile sentiment phases**.

**Short bias during fear**  
Profits from **closing short positions are higher during Fear**, suggesting traders benefit more from **bearish trades when market sentiment is negative**.

**Long bias during greed**  
Closing **long positions generates strong PnL during Greed**, indicating traders may **ride bullish momentum before exiting positions**.

**Profit-taking in Extreme Greed**  
A sharp rise in **Sell activity during Extreme Greed** suggests traders **begin distributing or locking in profits when the market becomes highly optimistic**.

**Liquidation pressure in bullish markets**  
Short liquidations appear during **Greed**, implying that some traders maintain **bearish positions during rallies and get squeezed when prices continue rising**.

**Limited position flipping**  
Direct **Long → Short** or **Short → Long** transitions contribute relatively little PnL, suggesting traders **typically close positions before opening the opposite direction rather than immediately flipping**.

---

**Conclusion**  
Trader behavior appears sentiment-dependent, with bearish trades performing better during fearful markets and profit-taking increasing as markets move into extreme optimism.

---
## Charts

![Classification](https://github.com/dhavltharkaaar/Analysis_Report/blob/main/images/piechart.PNG)

## Key Insights

**Fear dominates trading activity**  
Fear accounts for **29.3% of trades**, indicating cautious investor behavior and a tendency for traders to react strongly during uncertain market conditions.

**Bullish sentiment presence**  
**Greed and Extreme Greed together represent 42.7% of trades**, suggesting an overall **bullish sentiment bias** across the market.

**Low neutral participation**  
Only **17.8% of trades occur during Neutral sentiment**, implying that most traders operate under **emotionally driven market conditions rather than balanced sentiment**.

**Balanced psychological tension**  
The distribution between **Fear (39.4%) and Greed (42.7%)** is relatively close, highlighting a **continuous tug-of-war between pessimism and optimism in market psychology**.

---
![Average PnL by Sentiments](https://github.com/dhavltharkaaar/Analysis_Report/blob/main/images/avgpnlbysentiment.PNG)

## Average PnL by Market Sentiment

The bar chart compares **average Profit and Loss (PnL)** across five market sentiment classifications:

- **Extreme Greed** → Highest average PnL (~68), showing trades are **most profitable in this sentiment regime**.
- **Fear** → Second highest (~54), indicating **strong profitability despite cautious market sentiment**.
- **Greed** → Moderate average PnL (~43), **lower than Fear and Extreme Greed**.
- **Extreme Fear** → Lower average PnL (~35), reflecting **weaker trading performance**.
- **Neutral** → Similar to Extreme Fear (~34), also among the **least profitable sentiment conditions**.

### Key Takeaway

Profitability tends to be **highest during Extreme Greed and Fear**, while **Neutral and Extreme Fear environments generate the lowest average returns**.

This suggests that **trading opportunities improve when market sentiment becomes polarized**, whereas **balanced or indecisive market conditions tend to produce weaker average profits**.

---

![Average Trade by Sentiment](https://raw.githubusercontent.com/dhavltharkaaar/Analysis_Report/main/images/avgtradebysentiment.PNG)

## Average Trade Size by Market Sentiment

The chart compares **average trade size** across different market sentiment conditions:

- **Fear** → Highest average trade size (~7,800), indicating traders commit **larger positions during fearful market conditions**.
- **Greed** → Second highest (~5,700), showing **strong but slightly smaller commitments compared to Fear**.
- **Extreme Fear** → Moderate (~5,300), suggesting **cautious yet still meaningful position sizes**.
- **Neutral** → Lower (~4,800), reflecting **more balanced and moderate trade sizes**.
- **Extreme Greed** → Smallest average trade size (~3,100), indicating traders tend to **reduce position sizes when optimism becomes excessive**.

### Key Takeaway

Traders tend to **place their largest bets during Fear**, possibly reflecting **higher conviction or opportunistic positioning during downturns**.

In contrast, **Extreme Greed corresponds with smaller trade sizes**, suggesting **greater caution, diversification, or profit protection when markets become overly optimistic**.

Overall, **trade size varies significantly with sentiment**, highlighting how **market emotions influence position sizing decisions**.
