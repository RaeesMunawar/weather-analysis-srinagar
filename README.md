# Weather Data Analysis – Srinagar (1991–2020)

## 📌 Project Overview
This project analyzes the **long-term climatological data** of **Srinagar city** for the period **1991–2020**, based on official data published by the Indian Meteorological Department (IMD).  

The aim is to **understand seasonal climate patterns**, visualize temperature and rainfall distributions, and identify the **hottest, coldest, wettest, and driest months**.

---

## 📊 Dataset
- **Source**: IMD Climatological Tables (1991–2020)  
- **Format**: Data was originally in PDF, extracted manually and cleaned into Excel/CSV.  
- **Columns included**:
  - `Month` (Jan–Dec, Annual)
  - `Daily_Min_C` (°C)
  - `Daily_Max_C` (°C)
  - `Rainfall_mm` (mm)
  - `Rainy_Days` (days)
  - `Hail` (events)
  - `Thunder` (events)
  - `Fog` (events)
  - `Squall` (events)

---

## ⚙️ Tools & Libraries
- **Python 3**
- [Pandas](https://pandas.pydata.org/) → Data cleaning & analysis  
- [NumPy](https://numpy.org/) → Numerical computations  
- [Matplotlib](https://matplotlib.org/) → Data visualization  

---

## 🔎 Steps Performed
1. **Data Cleaning**
   - Converted the climatological table into a structured CSV.
   - Standardized column names and ensured numeric types.

2. **Exploratory Data Analysis (EDA)**
   - Summary statistics (`describe()`)
   - Checked for missing values
   - Basic insights on seasonal temperature and rainfall

3. **Visualization**
   - Line plot of **mean daily minimum & maximum temperatures**
   - Bar chart of **monthly rainfall**

4. **Extreme Analysis**
   - Identified hottest, coldest, wettest, and driest months using NumPy.

---

## 📈 Results (1991–2020, Srinagar)
- **Hottest Month** → **July (30.0 °C)**  
- **Coldest Month** → **January (-1.9 °C)**  
- **Wettest Month** → **March (104.6 mm)**  
- **Driest Month** → **October (21.8 mm)**  

---

## 📂 Project Structure
```
weather-analysis/
│
├── data/
│   └── Srinagar Dataset.xlsx
│   └── srinagar_climatology_cleaned.csv
│
├── outputs/
│   └── srinagar_temp_trend.png
│   └── srinagar_rainfall_bar.png
│   └── srinagar_extremes_summary.csv
│
├── analyze_srinagar.py        # Main analysis script
└── README.md                  # Project documentation
```

---

## ▶️ How to Run
1. Clone this repository or copy the project folder.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib openpyxl
   ```
3. Run the analysis script:
   ```bash
   python analyze_srinagar.py --input "data/Srinagar Dataset.xlsx"
   ```
4. Outputs will be saved in the `outputs/` folder:
   - `srinagar_temp_trend.png`
   - `srinagar_rainfall_bar.png`
   - `srinagar_extremes_summary.csv`

---

## 📌 Future Work
- Add time-series analysis for trends across decades.  
- Compare Srinagar with other cities (Jammu, Gulmarg).  
- Build interactive dashboards (Plotly, Streamlit).  

---

## 🙌 Acknowledgements
Data sourced from **Indian Meteorological Department (IMD)** Climatological Tables (1991–2020).  
