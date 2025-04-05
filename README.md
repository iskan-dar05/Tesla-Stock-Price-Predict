# 📈 Tesla Stock Price Prediction  

## 📜 Project Overview  
This project aims to predict Tesla's stock closing prices using **Linear Regression**.  
We preprocess historical stock data, engineer new features, and evaluate the model’s performance.  

## 🔍 Dataset  
The dataset contains daily stock prices with the following columns:  
- **Date** → Trading date  
- **Open** → Opening price  
- **High** → Highest price of the day  
- **Low** → Lowest price of the day  
- **Close** → Closing price (📌 Target variable)  
- **Volume** → Number of shares traded  

## 🛠️ Data Preprocessing  
Key preprocessing steps:  
✅ **Dropped unnecessary columns** (`Adj Close`)  
✅ **Created new features** (`MA_10`, `MA_50`, `Prev_Close`)  
✅ **Handled missing values**  
✅ **Split data into training & testing sets**  

## 🔥 Model & Training  
We trained a **Linear Regression Model** to predict the `Close` price using:  
- Features: `Open`, `High`, `Low`, `Volume`, `MA_10`, `MA_50`, `Prev_Close`  
- Target: `Close`  
- **Performance Metrics:**  
  - **R² Score:** Measures model accuracy  
  - **RMSE:** Measures prediction error  

## 📊 Results  
- **Train R² Score:** `0.9997`  
- **Test R² Score:** `0.9998`  
- **No Overfitting Observed** 🚀  

## 📌 Key Findings  
- **Prev_Close is highly correlated** with `Close`, which could inflate performance.  
- **Moving Averages (MA_10 & MA_50)** help capture trends effectively.  

## 📁 Installation & Usage  
### 🔹 **1. Clone the Repository**  
```bash
git clone https://github.com/iskan-dar05/Tesla-Stock-Price-Predict.git
cd Tesla-Stock-Price-Predict


### 🔹 Install Dependencies
```bash
pip install -r requirements.txt



3. Run Jupyter Notebook
jupyter notebook```

