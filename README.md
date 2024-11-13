# stock-market-analysis
This is project 1 for Rutgers AI Bootcamp

## Team Members

- Veena Uppalapati 

- Vas Prabhudesai

---

**Project Question**: Are these companies viable investment opportunities, and can we expect future growth based on an analysis of their financial health metrics and stock market performance?

---

## Project Setup 

### Data Sources

We will be sourcing data from two primary sources:
    - **Alpha Vantage**: This will provide financial information for each ticker, such as Income Statement and Cash Flow data.
    - **yFinance**: The yFinance SDK will be used to retrieve the top 3 companies by sector and obtain historical stock data. 

#### yFinance

1. **Install `yFinance` SDK**
    - Use the following link for reference and installation instructions: [yFinance Reference](https://pypi.org/project/yfinance/)

#### Alpha Vantage

1. **Obtain your your API key from Alpha Vantage:**
    - [Claim your Free API Key](https://www.alphavantage.co/support/#api-key)

2. **Create a `.env` File**
    - Once you have your API key,create `.env` file in the root of you project folder.

3. **Add Your API Key to the `.env` File:**
    - Inside the `.env` file, add the following line, replacing api_key_here with your actual API key:

```makefile
ALPHA_API_KEY=your_api_key_here
```


## Formulas

- **P/E Ratio** = Current Stock price / (Company's income / number of outstanding shares)
- ROIC 
- Net Profit Margin = (Net Income / Total Revenue) * 100

Visualizations
1. 15 graphs : Each shows a relationship between the `stock trend` and financial trend (two line graphs that displays `Free cash flow` and `Net Profit Margin`)


