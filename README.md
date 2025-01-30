# Crypto VWAP & OHLC Analysis

## 📌 Project Overview

This project is a Python-based analysis tool for cryptocurrency trading data. It focuses on calculating the **Volume-Weighted Average Price (VWAP)** and analyzing **Open, High, Low, and Close (OHLC)** price statistics.

## 🚀 Features

- Fetch cryptocurrency data using an API
- Compute **VWAP** for market trend analysis
- Generate **OHLC** statistics
- Standard deviation calculations for price volatility
- Data visualization for insights

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Requests (for API calls)

## 📂 File Structure

```
├── Projet_Python_Rodner_Rigoni.ipynb  # Jupyter Notebook with full analysis
├── data/                              # Folder for raw data (if applicable)
├── README.md                          # Documentation
```

## 🔧 Installation & Usage

### Prerequisites

Make sure you have **Python 3.x** installed along with the required dependencies:

```sh
pip install pandas numpy matplotlib requests
```

### Running the Notebook

1. Clone the repository:
   ```sh
   git clone https://github.com/jcrigoni/Crypto-VWAP-STD-OHLC.git
   ```
2. Navigate to the project folder:
   ```sh
   cd Crypto-VWAP-STD-OHLC
   ```
3. Open the Jupyter Notebook:
   ```sh
   jupyter notebook Projet_Python_Rodner_Rigoni.ipynb
   ```

## 📊 Methodology

1. **Data Retrieval**: Fetching live or historical cryptocurrency price data.
2. **VWAP Calculation**: Computing VWAP to analyze market trends.
3. **OHLC Analysis**: Studying Open, High, Low, and Close price movements.
4. **Standard Deviation**: Measuring volatility to assess market risk.
5. **Visualization**: Plotting price trends for better insights.

## 📌 Example Code Snippet

```python
import pandas as pd

def calculate_vwap(df):
    df['VWAP'] = (df['Close'] * df['Volume']).cumsum() / df['Volume'].cumsum()
    return df
```

## 📢 Contributors

- **Rodner Simon-Pierre**
- **Rigoni Jean-Christophe**

## 📜 License



This project is licensed under the MIT License.

---

Feel free to contribute by opening a pull request or reporting issues!

