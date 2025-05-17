# Akab Stock Screener 📉

A value-investing stock screener built using [Streamlit](https://streamlit.io) and [Yahoo Finance](https://finance.yahoo.com/) data.  
This tool applies 7 Benjamin Graham-inspired criteria to evaluate undervalued stocks and includes Graham Number and Graham Value metrics.

---

## ✅ Screening Criteria

The screener selects stocks based on the following 7 rules:

1. **Revenue > $100M**  
2. **Current Ratio > 2**  
3. **Estimated Current Assets - Liabilities > 0**  
4. **Pays Dividends**  
5. **Positive EPS for 5 Years** (at least 4 of last 5 EPS > 0)  
6. **Price ≤ 15 × 3-Year Avg EPS**  
7. **Price-to-Book (P/B) < 1.5**

Stocks that pass each criterion are marked ✅. Failing ones are marked ❌.

---

## 📊 Graham Valuation Metrics

These are provided **in addition to** the 7 criteria:

- **Graham Number**:  
  \[
  \text{Graham Number} = \sqrt{22.5 \times \text{EPS}_{7yr} \times \text{BVPS}}
  \]

- **Graham Value**:  
  \[
  \text{Graham Value} = \text{EPS}_{5yr} \times (8.5 + 2 \times \text{EPS Growth}) \times \left(\frac{4.4}{Y}\right)
  \]

Where:
- `EPS Growth` is estimated from net income history
- `Y` = Current AAA bond yield (defaulted to 4.4%)

✅ A stock is flagged if the current price is **below** either metric.

---

## 📥 How to Use

1. Upload a `.csv` file of tickers **or** manually input tickers (e.g., `AAPL, MSFT, TSLA`)
2. Click **"Run Screener"**
3. View results and download the Excel output

---

## 🛠 Built With

- `Streamlit` – App framework
- `yfinance` – Financial data
- `pandas`, `numpy` – Data processing
- `xlsxwriter` – Excel download

---

## 🌍 Live Demo

👉 [Try it on Streamlit Cloud](https://your-streamlit-link-here)

---

## 📫 Contact

Created by **Andoh Kwofie Amankwah-Baffo**  
📧 [andykwofie.ak@gmail.com]  
🔗 [LinkedIn](https://linkedin.com/in/yourprofile) | [GitHub](https://github.com/Andohkay1/akab-stock-screener)
