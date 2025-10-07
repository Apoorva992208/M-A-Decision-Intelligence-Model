M&A Decision Intelligence Model

Automated, presentation-ready M&A analysis tool integrating financial metrics, pro-forma projections, and AI-driven insights for acquirer–target deals. Generates Excel workbooks with dashboards, charts, and detailed financial statements.

Features

Automated Financial Data Fetching
Pulls company data (Income Statement, Balance Sheet, Cash Flow, Market Cap, Key Metrics) from Alpha Vantage API.

Dynamic Pro-Forma Modeling
Calculates purchase price, financing structure (cash, debt, stock), revenue/cost synergies, net income, EPS, and leverage projections over multiple years.

AI-Driven Insights
Leverages OpenAI GPT models (or fallback heuristic) to generate actionable M&A recommendations, risk scoring, and concise insights for each deal.

Presentation-Ready Excel Reports
Generates multi-sheet Excel workbooks including:

Raw company data

Summary of financial metrics

Scorecards for acquirer and target

Pro-Forma financial projections

Financing breakdowns

Dashboard with AI insights and Excel-native charts

Single-Deal Focus
Processes one acquirer–target pair at a time for precision and clarity.

Getting Started
Prerequisites

Python 3.10+

Required Python packages:

pip install pandas numpy openpyxl requests python-dotenv tqdm


Optional: OpenAI API access for AI insights

Alpha Vantage API Key for financial data

Setup

Clone the repository:

git clone https://github.com/Apoorva992208/mna-decision-model.git
cd mna-decision-model


Usage

Run the script for a single deal:

python mna_final.py


Example usage inside Python:

from mna_final import run_mna_deal

excel_path = run_mna_deal("INFY", "ACN")  # Acquirer, Target
print("Excel report generated at:", excel_path)

Output

The script generates a presentation-ready Excel workbook with:

Raw financial data

Summary metrics & scorecards

Pro-forma projections

Financing breakdowns

Dashboard with AI insights and charts