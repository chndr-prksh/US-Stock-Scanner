US Stock Scanner 📊🇺🇸

A Python-based US stock market scanner that computes technical indicators for thousands of US-listed stocks (NYSE, NASDAQ) and automatically publishes the results to Google Sheets for easy filtering, discovery, and analysis.

Built for traders, investors, and analysts who want a scalable, automated technical screening system with a simple spreadsheet-based interface.

🚀 Key Features
	•	📈 Scans thousands of US stocks (NYSE & NASDAQ)
	•	🧮 Calculates a comprehensive set of technical indicators
	•	☁️ Pushes live results to Google Sheets
	•	🔍 Easy scanning using filters, sorting & conditional formatting
	•	⚡ Fully automated Python pipeline
	•	🧩 Modular & extensible indicator framework


📉 Technical Indicators Covered

The scanner supports a broad range of indicators, including:

Trend Indicators
	•	SMA (Simple Moving Average)
	•	EMA (Exponential Moving Average)
	•	MACD
	•	ADX

Momentum Indicators
	•	RSI
	•	Stochastic Oscillator
	•	Rate of Change (ROC)

Volatility Indicators
	•	Bollinger Bands
	•	Average True Range (ATR)

Volume Indicators
	•	Volume SMA / EMA
	•	On-Balance Volume (OBV)

(Indicators are modular and can be customized per strategy.)

⸻

🧠 How the Scanner Works
	1.	Pulls historical OHLCV data for US stocks
	2.	Cleans and normalizes the data using Pandas
	3.	Computes technical indicators via Python TA libraries
	4.	Aggregates results into a structured table
	5.	Pushes the output to Google Sheets using the Sheets API
	6.	Google Sheets acts as a live technical scanner dashboard

⸻

📊 Google Sheets as the UI Layer

Google Sheets is used as the front-end for:
	•	Filtering stocks by RSI, trend, volatility, etc.
	•	Sorting by indicator values or signal strength
	•	Creating custom watchlists
	•	Applying conditional formatting
	•	Sharing scans with collaborators

This approach keeps the system powerful yet accessible to non-technical users.

⸻

🛠️ Tech Stack
	•	Python 3.x
	•	Pandas / NumPy
	•	Technical Analysis libraries (TA-Lib / pandas-ta)
	•	Google Sheets API
	•	Google Cloud Service Account

⸻

📂 Project Structure

├── data/
│   └── historical_prices/
├── indicators/
│   ├── trend.py
│   ├── momentum.py
│   └── volatility.py
├── sheets/
│   └── sheets_client.py
├── scanner.py
├── universe.py
├── config.py
├── requirements.txt
└── README.md


⸻

⚙️ Setup Instructions

1️⃣ Clone the Repository

git clone https://github.com/yourusername/us-stock-scanner.git
cd us-stock-scanner

2️⃣ Install Dependencies

pip install -r requirements.txt

3️⃣ Configure Google Sheets API
	•	Create a Google Cloud project
	•	Enable Google Sheets API
	•	Create a Service Account
	•	Download the credentials JSON file
	•	Share your Google Sheet with the service account email

Update config.py with:
	•	Google Sheet ID
	•	Credentials file path

⸻

▶️ Running the Scanner

python scanner.py

After execution, the Google Sheet will contain up-to-date technical indicators for all scanned US stocks.

⸻

📌 Use Cases
	•	Daily US market scanning
	•	Momentum & breakout discovery
	•	Swing & positional trading
	•	Portfolio screening
	•	Strategy research & validation

⸻

🔮 Planned Enhancements
	•	⏰ Scheduled scans (cron / Airflow)
	•	🟢 Buy / Sell / Hold signal generation
	•	📬 Alerts via Email, Slack, or Telegram
	•	📊 Strategy-based scanners
	•	🌐 Optional web dashboard

⸻

⚠️ Disclaimer

This project is for educational and research purposes only and does not constitute financial advice. Trading involves risk.

⸻

⭐ Contributing

Contributions and feature requests are welcome. Please open an issue or submit a pull request.

⸻

📄 License

MIT License

⸻

If this project helps you, consider giving it a ⭐ on GitHub!
