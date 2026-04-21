# Online Investor Attention, Trading Volume, and Stock Returns

## 1. Problem & User
This project examines whether online investor attention is associated with stock trading activity and stock returns. It is designed for beginner-level finance and business students who want to understand or are interested in how alternative data can be used in a simple Python-based financial analysis project.

## 2. Data
This project uses two main data sources:

- **Google Trends**
  - Source: Google Trends
  - Access date: 2026-04-16
  - Key fields: monthly search interest for selected stock-related search terms

- **WRDS CRSP**
  - Source: WRDS CRSP database
  - Access date: 2026-04-18
  - Key fields: stock ticker, date, trading volume, stock return, price

The selected stocks in this project are NVIDIA (NVDA), AMD, Tesla (TSLA), JPMorgan (JPM), and Palantir (PLTR).

## 3. Methods
The main Python steps in this project are:

- Load and clean Google Trends data
- Retrieve stock market data from WRDS CRSP
- Prepare and align the datasets into a comparable monthly format
- Merge investor attention data with stock trading data
- Conduct descriptive analysis
- Visualise patterns using charts
- Perform correlation analysis
- Run simple regression models to test the relationship between investor attention, trading volume, and stock returns

## 4. Key Findings
- Higher online investor attention is associated with higher trading volume.
- The relationship between investor attention and stock returns is weaker than the relationship with trading volume.
- Investor attention appears to be more useful for explaining market activity than explaining return performance.
- The results suggest that online search behaviour may capture investor interest, but it does not necessarily predict returns clearly in this small sample.

## 5. How to run
1. Download or clone this repository.
2. Make sure the Google Trends CSV files remain inside the `data` folder (The reading path specified in the code is a relative path, e.g. data/nvda_trends.csv.).
3. Install the required Python libraries listed in `requirements.txt`.
4. Open `Notebook.ipynb` from the repository root in Jupyter Notebook.
5. If you want to reproduce the WRDS extraction step, use your own WRDS account credentials.
6. Run the notebook from top to bottom.

## 6. Product Link / Demo
- **GitHub Repository:** https://github.com/xuewenxi857-droid/xjtlu_acc102_individual-assignment-project
- **Demo Video:** [Insert your demo video link]

## 7. Limitations & Next Steps
This project has several limitations. First, the sample includes only five stocks, so the findings may not generalise to the wider market. Second, Google Trends provides relative search interest rather than absolute search volume. Third, the analysis uses simple statistical methods and does not control for many other market factors.

For future improvement, the project could include a larger stock sample, a longer time period, additional control variables, and more advanced models to test whether investor attention has predictive value under different market conditions.
