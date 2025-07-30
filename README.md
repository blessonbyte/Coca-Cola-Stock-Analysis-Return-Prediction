# 🥤 Coca-Cola Stock Analysis & Return Prediction 📈

This project performs a complete analysis of Coca-Cola’s stock performance and return predictions using a multi-platform approach involving **Excel**, **SQL (MySQL)**, and **Python (Kaggle)**.

---

## 🗃️ Data Sources

- **Historical stock data**: Yahoo Finance (Coca-Cola stock prices)
- **Company financial metrics**: Scraped/cleaned from web sources
- **Additional indicators**: Engineered technical indicators and return calculations

---

## 🛠️ Tools & Platforms Used

- **Excel**:  
  - Initial data cleaning  
  - Pivot tables for trend spotting  
  - Manual ratio analysis and summary charts

- **MySQL**:  
  - Structured and stored multiple tables  
  - Performed complex queries and joins  
  - Generated stock summary reports using SQL views

- **Python (Kaggle)**:  
  - Final modeling and analytics  
  - EDA, feature engineering, and machine learning models

---

## 🧱 MySQL Tables Created

## 🗃️ MySQL Tables Created

1. **`stock_price`**  
   - Contains raw historical price data (Open, High, Low, Close, Volume)

2. **`stock_technical_indicators`**  
   - Stores calculated technical indicators (RSI, MACD, Moving Averages)

3. **`fundamental_metrics`**  
   - Holds fundamental analysis data (P/E Ratio, EPS, ROE, Dividend Yield)

4. **`Daily_Return_Classification`**  
   - Labeled dataset for ML (Return Direction: Positive/Negative/Neutral)

5. **`KPI_Comparison`**  
   - Competitive benchmarking table (ROA, ROE, P/E vs competitors)

6. **`Profitability_Metrics`**  
   - Tracks Coca-Cola's financial health (Margins, Quarterly/Yearly trends)

7. **`merged_stock_data`**  
   - Final unified view combining all tables for analysis

---

## 📊 Exploratory Data Analysis (Python)

Performed extensive EDA on combined dataset:

- Daily closing price trends
- Volume spikes and volatility
- Return distribution and histograms
- Correlation heatmaps
- Moving Averages, RSI plots

---

## 🤖 Machine Learning Models for Return Direction Classification

Target: **Predict if Coca-Cola stock will move 'Up' or 'Down' the next day**

### Models Trained:

- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**

### Metrics:
- Accuracy, Precision, Recall, F1-score
- Confusion Matrix
- Cross-validation scores

## 🤖 Machine Learning Model Performance

**Target Classification:** Predict daily return direction (Class 0 = Down, Class 1 = Up)  

| Metric / Class          | Logistic Regression | Random Forest | SVM |
|-------------------------|---------------------|---------------|-----|
| **Accuracy**            | 0.99               | 1.00          | 0.99 |
| **Precision (Class 0)** | 0.99               | 1.00          | 0.99 |
| **Recall (Class 0)**    | 1.00               | 1.00          | 1.00 |
| **F1-Score (Class 0)**  | 0.99               | 1.00          | 0.99 |
| **Precision (Class 1)** | 1.00               | 1.00          | 1.00 |
| **Recall (Class 1)**    | 0.99               | 1.00          | 0.98 |
| **F1-Score (Class 1)**  | 0.99               | 1.00          | 0.99 |
| **Macro Avg F1-Score**  | 0.99               | 1.00          | 0.99 |
| **Support (Total)**     | 3063               | 3063          | 3063 |

### Key Insights:
- 🏆 **Random Forest dominates** with perfect 1.00 scores across all metrics
- 🔍 All models maintain >99% precision/recall for both classes
- ⚖️ **Balanced dataset**: 1577 (Class 0) vs 1486 (Class 1) samples
- ⚠️ *Note: Perfect scores may indicate overfitting - further validation recommended*
  
Each model achieved **notable accuracy**, with **Random Forest** giving the best performance.

---

## 📈 Feature Engineering

- Calculated:
  - Daily Returns
  - Moving Averages (7, 21, 50 days)
  - RSI (14-day)
  - MACD and Signal Line
- Created:
  - `return_direction` = 'Up' or 'Down' based on daily returns
  - Volatility measures


---

## 🎯 Insights

- Coca-Cola stock shows consistent performance and low volatility
- Technical indicators like RSI and Moving Averages correlate well with returns
- Predictive models provide reliable signals for short-term price movements

---

## 🏁 Conclusion

This end-to-end stock analysis project covered data cleaning, technical and fundamental analysis, and classification modeling using multiple tools.  
From **Excel** to **MySQL** to **Python**, it demonstrates a practical, real-world approach to **stock return prediction**.

---

## 🙋‍♂️ Author

This project was completed by **Sam Caleb Blesson** as part of a virtual internship in the domain of Business Analytics.


