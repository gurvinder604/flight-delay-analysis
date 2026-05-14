# ✈️ US Flight Delay Root Cause Analysis

> End-to-end data analysis identifying the root causes and financial impact of US flight delays across 18 major airlines — built using Python and Power BI on 3 million real flight records.

---

## 📊 Dashboard Preview

| Overview | Airline Performance | Root Cause Analysis |
|---|---|---|
| *Screenshot coming* | *Screenshot coming* | *Screenshot coming* |

---

## 🔍 Project Summary

| Item | Detail |
|---|---|
| **Dataset** | BTS Airline On-Time Performance Data (2019–2023) |
| **Records analysed** | 2,992,928 flights |
| **Airlines covered** | 18 major US carriers |
| **Tools used** | Python, Pandas, Seaborn, Matplotlib, Power BI |
| **Project duration** | 4 days |

---

## 💡 Key Findings

1. **$978.1M** in estimated carrier delay costs identified across 18 airlines
2. **Late Aircraft propagation** is the #1 delay cause — 36.5% of all delays (194,789 flights)
3. **JetBlue Airways** has the highest delay rate at **27%** — more than 1 in 4 flights arrives late
4. **SkyWest Airlines** has the highest financial impact at **$165.9M** — driven by high flight volumes
5. **June** is the worst month for delays at **23%** delay rate — summer travel congestion
6. **September** is the best month at just **13%** delay rate
7. **Weather accounts for only 3.8%** of delays — far less than public perception suggests
8. **Aspen, CO** has the highest airport delay rate at **26.7%** — mountain geography impact
9. **Sunday in June** is the single worst combination — **24.5%** delay rate

---

## 📁 Project Structure

```
flight-delay-analysis/
├── data/
│   ├── raw/                    # Original dataset (not uploaded — 614MB)
│   ├── clean/                  # Cleaned CSV after Python processing
│   └── processed/              # Summary Excel files for Power BI
│       ├── monthly_summary.xlsx
│       ├── airline_summary.xlsx
│       ├── cause_summary.xlsx
│       ├── airport_summary.xlsx
│       └── heatmap_summary.xlsx
├── notebooks/
│   ├── 01_data_cleaning.ipynb  # Data loading, cleaning, feature engineering
│   └── 02_EDA.ipynb            # Exploratory analysis, charts, financial impact
├── charts/                     # 6 PNG charts exported from Python
│   ├── 01_delay_rate_by_airline.png
│   ├── 02_monthly_delay_trend.png
│   ├── 03_delay_cause_breakdown.png
│   ├── 04_worst_airports.png
│   ├── 05_delay_heatmap.png
│   └── 06_financial_impact.png
├── powerbi/
│   └── flight_delay_dashboard.pbix
├── dashboard_screenshots/
├── README.md
└── requirements.txt
```

---

## 🛠️ Tools & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat)

---

## 📈 Charts

### 1. Delay Rate by Airline
JetBlue (27%) and Frontier (26%) have the highest delay rates. Endeavor Air is the best performer at 13%.

### 2. Monthly Delay Trend
Clear summer peak in June/July with a sharp September dip. December shows a secondary spike driven by holiday travel.

### 3. Root Cause Breakdown
Late Aircraft (36.5%) and Carrier issues (33.7%) account for 70% of all delays. Weather is only 3.8%.

### 4. Top 10 Worst Airports
Aspen (26.7%) tops the list. Newark (23.3%) is the only major hub in the top 10 — chronic airspace congestion.

### 5. Delay Heatmap — Day vs Month
Sunday in June peaks at 24.5%. Tuesday in September is the best combination at just 10%.

### 6. Financial Impact by Airline
SkyWest leads at $165.9M despite a lower delay rate — pure volume effect. Top 4 airlines account for 59% of total costs.

---

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn openpyxl
```

### Steps
```bash
# 1. Clone the repo
git clone https://github.com/gurvinder604/flight-delay-analysis.git
cd flight-delay-analysis

# 2. Download dataset
# Get flights_sample_3m.csv from:
# kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023
# Place in data/raw/

# 3. Run notebooks in order
# Open Jupyter or VS Code
# Run 01_data_cleaning.ipynb first
# Then run 02_EDA.ipynb

# 4. Open Power BI dashboard
# Open powerbi/flight_delay_dashboard.pbix in Power BI Desktop
```

---

## 📊 Power BI Dashboard

3-page interactive dashboard built in Power BI Desktop:

| Page | Content |
|---|---|
| **Overview** | 4 KPI cards (3M flights, 534K delayed, 17.7% rate, $978M cost) + Monthly trend line chart + Month slicer |
| **Airlines** | Delay rate by airline (bar) + Carrier delay cost by airline (bar) |
| **Root Causes** | Delay cause donut chart + Flight count by cause + Day vs Month heatmap matrix |

---

## 🏢 Business Recommendations

1. **Address Late Aircraft cascading** — build buffer time into turnaround schedules, especially in summer
2. **JetBlue and Frontier need urgent reliability improvements** — both above 25% delay rate
3. **Newark requires systemic congestion management** — only major hub in the top 10 worst airports
4. **Increase schedule buffer in June and July** — delay rates 40% above annual average
5. **Weather preparedness focus is misaligned** — only 3.8% of delays are weather-caused; focus on internal operations instead

---

## 👤 About

**Gurvinder Singh (Gary)**
Data Analyst | Python | SQL | Power BI

- 🎓 BSc Computer Science (2:1) — University of West London
- 💼 LinkedIn: [linkedin.com/in/gurvindersingh-garry](https://linkedin.com/in/gurvindersingh-garry)
- 🐙 GitHub: [github.com/gurvinder604](https://github.com/gurvinder604)

---

## 📄 Data Source

Bureau of Transportation Statistics (BTS) — US Airline On-Time Performance Data  
Available via Kaggle: [Flight Delay and Cancellation Dataset 2019-2023](https://www.kaggle.com/datasets/patrickzel/flight-delay-and-cancellation-dataset-2019-2023)

> ⚠️ Raw data files are not included in this repository due to file size (614MB). Download from the Kaggle link above and place in `data/raw/`.

---

*Built as part of a data analyst portfolio — completed May 2026*
