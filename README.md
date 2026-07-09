# Stock Comparison Tool

## Research Question
How did a selected group of stocks perform over the same period, and which stock generated the highest total price return?

I built this as my first market-data project to move beyond looking at separate price charts and create a consistent comparison using the same dates and calculation for every stock.

## Data
The notebook downloads historical closing prices from Yahoo Finance through `yfinance`.

The user provides:
- Multiple stock tickers
- A common start date
- A common end date

Using the same period is important because comparing returns from different dates would not be meaningful.

## Methodology
For each valid ticker, the notebook:
1. Downloads historical closing prices.
2. Uses the first and last available prices in the selected period.
3. Calculates total return as `(final price - initial price) / initial price`.
4. Stores the result in a results table.
5. Sorts the stocks from highest to lowest return.
6. Identifies the best and worst performers.
7. Plots total returns in a bar chart.
8. Plots normalised price performance so the price paths can be compared from the same starting point.

## Outputs and Interpretation
The output changes depending on the tickers and dates entered. The notebook displays:
- Total return for every valid stock
- A performance ranking
- The best-performing and worst-performing stock
- A bar chart comparing total returns
- A normalised price chart showing how $1 would have grown in each stock

The result answers a narrow question: which stock increased the most over that specific period. It does not show which stock was the best investment after considering risk.

## Limitations
- Total return is based only on the first and last prices and ignores most of the path taken between them.
- The comparison does not measure volatility, drawdown, or risk-adjusted return.
- It does not control for sector exposure, market beta, or company size.
- Invalid or delisted tickers may return incomplete data.
- The highest historical return does not imply the highest future return.

## What I Learned
This project taught me how to collect user input, loop through several securities, store results, rank observations, and visualise a financial comparison. It also showed me why return alone is an incomplete measure, which motivated my later portfolio-risk project.

## How to Run
1. Install the dependencies:

```bash
pip install -r requirements.txt
```

2. Open `stock_comparison_tool.ipynb` in Jupyter Notebook.
3. Run the cells from top to bottom and enter the tickers and dates when prompted.

## Author
Ping-Hsiang (Wilbert) Lin
