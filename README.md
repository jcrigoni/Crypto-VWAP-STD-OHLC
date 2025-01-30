Crypto VWAP & OHLC Analysis

📌 Project Overview

This project is a Python-based analysis tool for cryptocurrency trading data. It focuses on calculating the Volume-Weighted Average Price (VWAP) and analyzing Open, High, Low, and Close (OHLC) price statistics.

🚀 Features

Fetch cryptocurrency data using an API

Compute VWAP for market trend analysis

Generate OHLC statistics

Standard deviation calculations for price volatility

Data visualization for insights

🛠 Technologies Used

Python

Pandas

NumPy

Matplotlib

Requests (for API calls)

📂 File Structure

├── Projet_Python_Rodner_Rigoni.ipynb  # Jupyter Notebook with full analysis
├── data/                              # Folder for raw data (if applicable)
├── README.md                          # Documentation

🔧 Installation & Usage

Prerequisites

Make sure you have Python 3.11 installed along with the required dependencies:

pip install pandas numpy matplotlib requests

Running the Notebook

Clone the repository:

git clone https://github.com/jcrigoni/Crypto-VWAP-STD-OHLC.git

Navigate to the project folder:

cd Crypto-VWAP-STD-OHLC

Open the Jupyter Notebook:

jupyter notebook Projet_Python_Rodner_Rigoni.ipynb

📊 Methodology

Data Retrieval: Fetching live or historical cryptocurrency price data.

VWAP Calculation: Computing VWAP to analyze market trends.

OHLC Analysis: Studying Open, High, Low, and Close price movements.

Standard Deviation: Measuring volatility to assess market risk.

Visualization: Plotting price trends for better insights.

📌 Example Code Snippet

import pandas as pd

def calculate_vwap(df):
    df['VWAP'] = (df['Close'] * df['Volume']).cumsum() / df['Volume'].cumsum()
    return df

📢 Contributors

Rigoni
Rodner

📜 License

This project is licensed under the MIT License.

Feel free to contribute by opening a pull request or reporting issues!
