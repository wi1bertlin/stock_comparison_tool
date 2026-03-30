# Stock Comparison Tool

## Overview
This project is a Python-based tool that compares the performance of multiple stocks over a selected time period. It calculates the total return for each stock and identifies the best performer.

The goal is to demonstrate basic financial data analysis using real market data.

---

## Features
- Input multiple stock tickers  
- Download historical data using yfinance  
- Calculate total return for each stock  
- Rank stocks by performance  
- Identify the best performing stock  
- Visualize results using a bar chart  

---

## How It Works
The program:
1. Takes user input for stock tickers and date range  
2. Downloads historical closing prices  
3. Calculates total return:  
   (Final Price - Initial Price) / Initial Price  
4. Stores and compares results  
5. Displays performance and ranking  

---

## Example Output
AAPL: 12.34%  
TSLA: 18.56%  
NVDA: 35.12%  

Best performing stock: NVDA  

---

## Technologies Used
- Python  
- yfinance  
- matplotlib  

---

## How to Run

1. Install required libraries:

    pip install yfinance matplotlib

2. Run the notebook:

    stock_comparison_tool.ipynb

3. Enter stock tickers and dates when prompted  

---

## Key Learning
This project shows how to work with financial data, perform basic analysis, and compare multiple assets.

It also demonstrates that performance can vary significantly across stocks over the same time period.

---

## Author
Ping-Hsiang (Wilbert) Lin
