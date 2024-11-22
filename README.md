# stock-market-analysis
This is project 1 for Rutgers AI Bootcamp

## Table of Contents
- [Team Members](#team-members)
- [Project Structure](#project-structure)
- [Project Setup](#project-setup)
- [Visualization](#visualizations)
- [Formulas](#formulas)

## Team Members

- Veena Uppalapati 

- Vassudeo Prabhudesai

---



**Project Question**: Are these companies viable investment opportunities, and can we anticipate future growth based on an analysis of their financial health metrics and long-term stock market performance?

[Link to the Presentation](https://docs.google.com/presentation/d/1jm3VIDY-nqCR6jQcDC8Q5CWNv46OxdVCQqXErMCp5y4/edit#slide=id.g2d5c37a4785_1_530)


## Project Structure

```bash
stock-market-analysis
├── output/                          # Directory containing PNG images of visualizations
├── additional-research.ipynb        # Jupyter Notebook analyzing 5-day period stock data
├── stock-market-analysis.ipynb      # Main project file analyzing yearly stock data
├── stock-data-tool                  # This is the code for the interactive tool that generates historical stock data for closing prices
```


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
---

## Visualizations

1. **Historical data trends**
This section provides insights into the historical performance of the company through two visualizations:
    - **Graph 1: Yearly Historical Data (Regular Scale)**
        Displays the trends in yearly data on a standard linear scale to highlight overall patterns and changes.
    - **Graph 2: Yearly Historical Data (Logarithmic Scale)**
        Uses a logarithmic scale to visualize data with large variations, making it easier to identify relative changes and trends.


2. **Forecasting with prophet**
Forecasted trends using Prophet for key company metrics:
    - **Graph 3: LLY Forecasted Trend**
        Predicts the future trends for LLY based on historical data.
    - **Graph 4: NVDA Forecasted Trend**
        Displays the projected trends for NVDA, aiding in future investment planning.


3.  **Visualizations for Company Financials**
Bar charts showcasing the company's performance across critical financial metrics:
    - **Graph 5: Free Cash Flow (FCF)**
    Highlights the cash generated after accounting for operating expenses and capital expenditures, offering insights into the company's liquidity and financial health.
    - **Graph 6: Net Profit Margin**
    Depicts the percentage of revenue remaining as profit after expenses, demonstrating the company's profitability.
    - **Graph 7: Return on Investment (ROI)**
    Reflects the efficiency of the company's investments in generating returns, providing a comprehensive view of performance.

---

## Formulas

- **Free Cash Flow (FCF)** = (Operating Cash Flow - Capital Expenditures) * 100
- **Return of Investment (ROI)** = ((Net Income - Capital Expenditures ) / Capital Expenditures) * 100
- **Net Profit Margin (%)** = (Net Income / Total Revenue) * 100



