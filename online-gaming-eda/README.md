# Online Gaming Behavior — Exploratory Data Analysis (EDA)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243.svg)](https://numpy.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg)](https://jupyter.org/)
[![Excel](https://img.shields.io/badge/Excel-Pivot%20Analysis-217346.svg)](https://www.microsoft.com/en-us/microsoft-365/excel)

Comprehensive exploratory data analysis (EDA) on online gaming behavior patterns from an Indian user cohort (500 records).

---

## Project Highlights

- **Data Cleaning**: Handled missing values, standardized nominal and binary categories, imputed numerical outliers using median/mode strategies.
- **Parametric & Non-Parametric Statistics**: Computed mean, median, mode, and skewness for daily play hours and monthly in-game spending.
- **Impact Assessment**: Visualized the correlation between intensive gaming duration, self-reported health problems, and work/academic disruptions.
- **Excel Pivot Cross-Validation**: Analyzed demographic cohorts and spending tiers across multiple Excel pivot sheets.

---

## Key Metrics & Findings

- **Total Cohort Size**: 500 users, 11 core attributes + derived `Age_Group`
- **Average Daily Play Hours**: **5.38 hours** (median: 5.0 hours, mode: 5.0 hours)
- **Median Monthly Spend**: **₹2,483** (mean: ₹2,740, right-skewed distribution)
- **High-Impact Threshold**: Gamers playing > 6 hours/day exhibit marked increases in Severe productivity impact and health fatigue complaints.

---

## Workspace Structure

```
online-gaming-eda/
├── data/
│   └── online_gaming_behavior_cleaned (1).xlsx  # 500-record dataset + Excel pivot tables
├── notebooks/
│   └── Online_Gaming_EDA.ipynb                  # Data cleaning and exploratory analysis notebook
├── README.md                                    # Documentation
└── requirements.txt                             # Pinned Python dependencies
```

---

## Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Launch Jupyter
jupyter notebook notebooks/Online_Gaming_EDA.ipynb
```

---

## Technologies Used

- **Python 3.10+**
- **pandas**, **NumPy**, **Matplotlib**, **Seaborn**, **openpyxl**, **Microsoft Excel**

---

## Author

- **Raunak Nayak** ([GitHub](https://github.com/raunaknayak12) · [LinkedIn](https://linkedin.com/in/raunak-nayak-5b937732a))
