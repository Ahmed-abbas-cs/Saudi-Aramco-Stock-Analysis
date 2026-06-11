# Saudi Aramco Stock Market Performance & Risk Analytics

An end-to-end data science and financial analytics project that builds a robust data pipeline to ingest, clean, and analyze historical trading data for Saudi Aramco (2019 - 2024). The project combines Python for advanced financial feature engineering and statistical risk assessment with an interactive Tableau dashboard for executive decision support.

## Interactive Dashboard Preview
Below is the polished analytical dashboard tracking market trends, liquidity anomalies, and volatility distribution:

![Saudi Aramco Stock Analytics & Risk Dashboard](Saudi%20Aramco%20Stock%20Analytics%20&%20Risk%20Dashboard.png)

---

## Data Pipeline & Methodology

1. **Data Ingestion & Integrity Auditing (Python / Pandas):**
   * Imported historical time-series data from Tadawul.
   * Conducted full data cleansing, verified structural integrity, and resolved zero-volume anomalies.
   * *Data Quality Note:* A known tracking gap exists in mid-2023 raw data, preserved transparently to showcase rigorous data auditing.

2. **Financial Feature Engineering (Python):**
   * Generated short-term trend indicators using a **50-Day Simple Moving Average (SMA_50)**.
   * Implemented long-term baseline indicators using a **200-Day Simple Moving Average (SMA_200)**.
   * Engineered a daily volatility metric utilizing percentage price changes to model historical asset risk.

3. **Visual Intelligence & UI/UX (Tableau):**
   * Developed a combined-axis momentum tracker overlaying closing prices against SMAs.
   * Applied a logarithmic scale to volume charts to expose baseline retail liquidity hidden by institutional anomalies.
   * Built a synchronized percentage-based histogram to map risk distribution models.

---

## Key Insights & Financial Interpretation

### 1. Long-Term Trend & Momentum Analysis
The integration of 50-day and 200-day SMAs effectively filters out short-term market noise, exposing the stock's underlying structural trends. A powerful bullish momentum is visible from late 2021 through mid-2022, culminating in a **historic peak of ~38.5 SAR in May 2022**. This surge was directly triggered by macroeconomic catalysts, notably the global energy supply crunch and Aramco’s record-breaking net income that year. The subsequent downward crossovers in mid-2024 reflect structural price corrections ahead of secondary market capitalizations.

### 2. Liquidity Dynamics & Institutional Catalysts
Applying a logarithmic scale to trading volume uncovers core liquidity patterns typically masked by massive institutional spikes. The pipeline clearly captures two defining milestones in the Saudi capital market: the **landmark Initial Public Offering (IPO) in late 2019**, and the **Secondary Share Offering in June 2024**, which generated a massive liquidity shockwave exceeding 650M shares traded in a single window.

### 3. Volatility Profile & Capital Preservation
The daily returns distribution exhibits a highly concentrated, leptokurtic Gaussian curve tightly centered around 0.0%. This narrow bell-shape mathematically confirms Saudi Aramco's classification as a **classic 'Defensive Asset'**. With a calculated daily standard deviation of **1.11%**, the asset demonstrates exceptional price resilience and minimal exposure to tail-risk (Black Swan events). This makes the stock a reliable financial anchor for institutional portfolios and sovereign funds during broader macroeconomic or cyclical downturns.

---

## Project Structure
* `analysis.ipynb` -> Jupyter Notebook detailing data ingestion, cleaning, and financial calculations.
* `saudi_aramco_enriched_data.csv` -> The final processed dataset ready for BI tools.
* `Saudi Aramco Stock Analytics & Risk Dashboard.png` -> High-resolution export of the Tableau layout.
* `README.md` -> Full analytical report and documentation.

## How to Run
1. Clone this repository: `git clone https://github.com/YOUR_USERNAME/Aramco_Stock_Analysis.git`
2. Install Python dependencies: `pip install pandas matplotlib seaborn`
3. Execute the Jupyter notebook to see data transformations.
4. Open the data source in Tableau to explore the interactive dashboard.
