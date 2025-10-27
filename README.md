# 📈 TCS Stock Analysis & Interactive Dashboard

This project performs a **comprehensive analysis of historical stock data** for **Tata Consultancy Services (TCS)** from **2002 to 2021**.  

The analysis is conducted using a **Python script**, which generates a detailed **JSON file**.  
This JSON file powers a **standalone, interactive web dashboard** that visualizes the key findings.

---

## 🗂️ 1. About the Datasets

The analysis is built on **three key data files**, located inside the `input_data/` folder:

### **📄 TCS_stock_history.csv**
Contains daily **OHLC (Open, High, Low, Close)** prices and **trading volume** from **August 2002 to September 2021**.

### **📄 TCS_stock_action.csv**
A log of all **corporate actions**, including:
- Dividend payouts  
- Stock split dates and factors  

### **📄 TCS_stock_info.csv**
A key-value file providing detailed **company profile information**, such as:
- Business summary  
- Sector  
- Employee count  

---

## 🎯 2. Project Objectives

The analysis was guided by **five key objectives** to build a complete picture of TCS stock performance:

1. **Analyze Historical Price Trend:**  
   Understand the long-term growth and identify major market shifts.

2. **Identify and Analyze Stock Volatility:**  
   Detect periods of high and low market instability using **30-day rolling volatility**.

3. **Evaluate Trading Volume Trends:**  
   Track **30-day average trading volume** to gauge investor interest and liquidity.

4. **Analyze Impact of Corporate Actions:**  
   Study how **dividends and stock splits** affected the stock and rewarded shareholders.

5. **Forecast Future Price Movements:**  
   Build a **30-day price forecast** using an **ARIMA time-series model**.

---

## 📊 3. Analytical Findings

The analysis script processed the data and produced the following **key findings**:

- **📈 Long-Term Growth:**  
  TCS stock shows a **strong, consistent upward trend** from 2002 to 2021, indicating outstanding historical performance.

- **⚡ Volatility Spikes:**  
  Volatility is not constant — major spikes align with significant market events such as the **2008 Financial Crisis** and the **2020 COVID-19 pandemic**.

- **💰 Increased Liquidity:**  
  Trading volume has grown substantially over time, suggesting **greater investor participation** during volatile market periods.

- **🎁 Shareholder Value:**  
  TCS consistently **rewards shareholders** through regular dividends and multiple **stock splits** (notably in 2006, 2009, and 2018), improving accessibility for retail investors.

- **🔮 Short-Term Forecast:**  
  A **30-day forecast** was generated using an **ARIMA model**, providing short-term directional insight based on past price trends.

---

## ⚙️ 4. Project Workflow (Our Understanding)

This project consists of **two main parts** that work together seamlessly:

---

### **🧮 Part 1: Data Analysis (Python)**

- Run the script `tcs_stock_analysis.py` in an environment such as **Google Colab** or **Jupyter Notebook**.  
- The script:
  - Loads the three `.csv` files from the `input_data/` folder.  
  - Cleans and processes the data (handles dates, missing values, etc.).  
  - Performs all five analyses (volatility, ARIMA forecasting, etc.).  
  - Exports all computed metrics and chart data into one file:
    ```
    output_data/tcs_stock_analysis.json
    ```

---

### **💻 Part 2: Interactive Dashboard (HTML + JavaScript)**

- The dashboard file `index.html` is a **standalone web app** — it runs **entirely in the browser** (no backend needed).  
- When launched:
  - The user uploads the `tcs_stock_analysis.json` file.  
  - JavaScript instantly parses the JSON and renders charts dynamically.  
- Built with:
  - **Chart.js** → for interactive visualizations  
  - **Tailwind CSS** → for responsive, modern styling  

---

## 🚀 5. GitHub Repository

To publish this project on GitHub:

1. Create a new repository, e.g.:
2. Upload all project files following the folder structure shown below.  
3. Your repository will be live at:  
👉 **[https://github.com/VenuOnTech/TCS-Stock-Data](https://github.com/VenuOnTech/TCS-Stock-Data)**

4. *(Optional)* Enable **GitHub Pages** in your repository settings — this allows you to **host your `TCS_Dashboard.html` file live** on the web!

---

## 🗺️ 6. Project Folder Map

Here’s the recommended **folder structure** for the project:

TCS-Stock-Dashboard/  
│  
├── README.md # Project documentation (you are here)  
│   
├── index.html # Interactive web dashboard (Chart.js + Tailwind)  
│  
├── datasets/  
│      ├── TCS_stock_action.csv # Corporate actions data  
│      ├── TCS_stock_history.csv # Daily stock prices and volume  
│      └── TCS_stock_info.csv # Company profile information  
|  
├── images/ # This Folder contains the images which we got after the analysis
|  
├── notebooks/  
│      └── TCS_Stock_Analysis.ipynb # This file contains the data analysis on the datasets  
│  
└── static/  
    └── tcs_stock_analysis.json # Generated JSON output file  


---

## 🧠 7. Key Learnings & Insights

- The TCS stock demonstrates **strong fundamentals** and long-term investor confidence.  
- **ARIMA modeling** offers a reliable short-term trend forecast based on historical data.  
- **Volatility analysis** reveals how major economic events affect investor behavior.  
- The **dashboard integration** showcases how raw analysis can be turned into **interactive business intelligence tools**.

---

## 🧩 8. Technologies Used

| Category | Tools / Libraries |  
|-----------|------------------|  
| **Programming Language** | Python |  
| **Data Analysis** | Pandas, NumPy, Matplotlib, Statsmodels (ARIMA) |  
| **Visualization** | Chart.js |  
| **Styling** | Tailwind CSS |  
| **Web Framework** | HTML, JavaScript |  
| **Environment** | Google Colab / Jupyter Notebook |  

---

## 🏁 Final Thoughts

This project combines **data analysis**, **time-series modeling**, and **interactive visualization** to deliver a clear, data-driven view of TCS stock performance.

It demonstrates how **Python analytics** and **frontend visualization** can work hand-in-hand to provide **real-time, user-driven insights**.

> “Numbers tell a story — dashboards let you see it.” 📊✨
