# Akab Stock Screener 📉

Akab is a Python-powered stock screener designed for value investors. It identifies undervalued companies using Benjamin Graham's investment principles — including earnings, book value, and intrinsic value vs market price.

🔗 **Launch the Screener**  
[https://your-app-name.streamlit.app](https://your-app-name.streamlit.app)

---

## 🔍 Features

- Screens tickers against 5 Graham-style value criteria:
  - Revenue > $100M
  - Current Ratio > 2
  - Price-to-Book > 1.5
  - Graham Number exists
  - Graham Value exists
- Displays:
  - Share price vs intrinsic value (✅ if undervalued)
  - Emoji indicators for passed/failed checks
  - Excel export of results
- Built with: `Streamlit`, `yfinance`, `pandas`

---

## 🧠 How It Works

- Upload a CSV or type tickers (e.g., AAPL, MSFT)
- Click “Run Screening”
- App fetches financials and flags those that meet criteria
- Results can be downloaded as Excel

---

## 📦 Tech Stack

- Python
- Streamlit
- Yahoo Finance API (via `yfinance`)
- Excel Export (`xlsxwriter`)

---

## 👨‍💻 Author

Built by [Andoh Kwofie Amankwah-Baffo](https://www.linkedin.com/in/andoh-amankwah-baffo), MBA Candidate | Value Investing Enthusiast
