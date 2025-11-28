Stock Sentinel AI 🔍📈

AI-Powered Stock Safety Analysis

Stock Sentinel AI is a lightweight AI system that analyzes multiple stocks and determines which one is safest for long-term investors.
Instead of predicting prices, it focuses on risk, using quantitative risk metrics and AI-style scoring to produce a Safety Score and rank stocks from safest → riskiest.

⭐ Features

📊 Pulls real market data using Yahoo Finance API

🧮 Calculates 6 major risk metrics

🤖 AI-style weighted scoring system

📈 Generates clean visualizations (drawdowns & vol/beta charts)

📝 Outputs results to CSV for further analysis

💻 Simple terminal input for choosing tickers

🔧 Technologies Used

Python 3.9+

pandas — data handling

numpy — numerical operations

matplotlib — visualizations

yfinance — market data API


You will be prompted to enter stock tickers:

Enter stock tickers separated by spaces (e.g. AAPL MSFT NVDA):


Example:

AAPL MSFT NVDA SPY

📘 How It Works
Data Collection

The system downloads daily historical price data using yfinance, automatically including SPY as the benchmark index.

Risk Metrics Calculated

Volatility

Beta vs SPY

Maximum Drawdown

Downside Deviation

% Negative Days

Value-at-Risk (VaR 95%)

Safety Score Algorithm

Standardizes metrics (z-scores)

Inverts “lower is safer” metrics

Combines them using a weighted scoring formula

Produces a final AI Safety Score

📊 Example Output

Files generated in the results/ folder:

metrics_and_scores.csv — full risk table & final safety scores

price_drawdowns.png — how far each stock drops from its peak

vol_vs_beta.png — volatility vs beta scatter plot

📌 Sample Ranking

(Your results may differ depending on dates & tickers)

Rank	Ticker	Safety Score
1	MSFT	Safest
2	AAPL	—
3	SPY	—
4	NVDA	Riskiest
📚 Documentation

See the included CODE_OVERVIEW.md for:

function explanations

algorithm descriptions

project logic

risk calculations

🛠️ Future Improvements

Add neural network models to predict future risk

Integrate news sentiment analysis

Build a web dashboard (Flask/React)

Add more risk factors & machine learning models

🧑‍💻 Author

Noorman Amanuel
AI & Data Science Student

📜 License

This project is open-source under the MIT License.
