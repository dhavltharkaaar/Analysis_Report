# Analysis_Report

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
### Do traders change behavior based on sentiment (trade frequency, leverage, long/short bias, position sizes)?
![Answer 1 Screenshot](https://github.com/dhavltharkaaar/Analysis_Report/blob/main/images/pivot.PNG)

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

