# Online Gaming Behavior — Exploratory Data Analysis (EDA)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243.svg)](https://numpy.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626.svg)](https://jupyter.org/)
[![Excel](https://img.shields.io/badge/Excel-Pivot%20Analysis-217346.svg)](https://www.microsoft.com/en-us/microsoft-365/excel)

A statistical exploratory data analysis of online gaming behavioral patterns among Indian users. This project investigates the interplay between daily gaming duration, in-game financial expenditure, demographic factors, network access conditions, reported health issues, and academic/occupational productivity.

---

## Project Overview & Resume Parity

As highlighted in Raunak Nayak's technical experience:
- **Data Cleaning & Reliability**: Handled missing values, standardized inconsistent categories, eliminated erroneous negative values, and normalized categorical variables across 500 user profiles.
- **Parametric & Non-Parametric Statistics**: Computed mean, median, mode, and skewness for continuous behavioral metrics (gaming duration, monthly expenditure).
- **Impact Assessment**: Built histogram distributions and pivot-based visualizations in Python and Microsoft Excel to evaluate the academic and occupational impacts of excessive gaming.

---

## Dataset Architecture

The analysis evaluates a cohort of **500 users** across 11 core attributes plus derived cohort dimensions:

| Field Name | Data Type | Description | Cleaning / Imputation Strategy |
|---|---|---|---|
| `user_id` | Integer | Unique identifier for each participant | Primary index |
| `age` | Numeric | Age in years (15 – 65) | Coerced to numeric, imputed missing values with median |
| `gender` | Categorical | Male / Female | Standardized short-hand (`M` → `Male`, `F` → `Female`) |
| `region` | Categorical | Urban / Rural / Semi-Urban | Standardized case casing (`URBAN` → `Urban`) |
| `avg_daily_play_hours` | Float | Average time spent gaming per day | Cleaned invalid negative values; imputed via median |
| `preferred_game_type` | Categorical | Battle Royale, Sports, Strategy, Simulation, Puzzle | Standardized nominal categories |
| `uses_public_wifi` | Categorical | Yes / No | Standardized boolean flags (`Y`/`N` → `Yes`/`No`) |
| `monthly_spend_inr` | Float | Monthly in-game purchase spend in INR (₹) | Cleaned negative values; evaluated distribution skew |
| `government_internet_scheme` | Categorical | Yes / No / Don't Know | Standardized categorical values |
| `reported_health_issues` | Categorical | Yes / No | Standardized self-reported physical/mental fatigue flags |
| `academic_or_work_impact` | Ordinal | Low / Medium / Severe | Ranked severity of gaming interference on productivity |
| `Age_Group` | Categorical | `<18`, `18-25`, `26-35`, `36-50`, `50+` | Feature-engineered demographic cohort |

---

## Key Statistical Findings

### 1. Gaming Duration Patterns
- **Mean Daily Play Hours**: **5.38 hours/day**
- **Median Daily Play Hours**: **5.00 hours/day**
- **Mode Daily Play Hours**: **5.00 hours/day**
- **Distribution**: Moderate right skew with peak density between 3.0 and 6.5 hours daily.

### 2. In-Game Spending Behavior
- **Median Monthly Spend**: **₹2,483**
- **Mean Monthly Spend**: **₹2,740**
- **Skewness**: Positive right-tail skewness driven by high-spending enthusiasts ("whales") exceeding ₹6,000/month.

### 3. Occupational & Academic Interference
- Users reporting **> 6 hours of daily gaming** demonstrated a significantly higher probability of reporting **Severe** academic or work productivity disruptions.
- Correlated with higher self-reported health fatigue symptoms (eye strain, posture complaints, sleep cycle disturbances).

---

## Repository Structure

```
online-gaming-eda/
├── .gitignore                               # Root ignore rules for Python & Jupyter artifacts
├── README.md                                # Master repository documentation (this file)
└── online-gaming-eda/                       # Project workspace
    ├── data/
    │   └── online_gaming_behavior_cleaned (1).xlsx  # Multi-sheet workbook (Raw, Cleaned & Excel Pivots)
    ├── notebooks/
    │   └── Online_Gaming_EDA.ipynb          # End-to-end data cleaning, statistics & visualization
    ├── README.md                            # Component documentation
    └── requirements.txt                     # Pinned Python dependencies
```

### Multi-Sheet Excel Structure
The dataset in `data/online_gaming_behavior_cleaned (1).xlsx` features pre-calculated pivot tables:
- `online_gaming_behavior_cleaned `: Master 500-record cleaned dataset.
- `Sheet1`, `Sheet5`, `Sheet6`, `Sheet8`, `Sheet11`: Pivot tables cross-tabulating age groups, game genre preferences, and average monthly spend in INR.

---

## Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/raunaknayak12/online-gaming-eda.git
cd online-gaming-eda/online-gaming-eda
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the Jupyter Notebook
```bash
jupyter notebook notebooks/Online_Gaming_EDA.ipynb
```

The notebook dynamically detects and loads the dataset from relative paths (`../data/` or `./data/`), ensuring reproducible execution across any environment.

---

## Technologies Used

- **Python 3.10+**
- **pandas** — Data cleaning, type coercion, missing value imputation, pivot tables
- **NumPy** — Statistical aggregations, array operations
- **Matplotlib & Seaborn** — Distribution histograms, scatter plots, and correlation heatmaps
- **openpyxl** — Multi-sheet Excel workbook parsing and extraction
- **Microsoft Excel** — Cross-validation pivot tables and summary aggregations

---

## Author & Acknowledgements

- **Author**: Raunak Nayak ([GitHub](https://github.com/raunaknayak12) · [LinkedIn](https://linkedin.com/in/raunak-nayak-5b937732a))
- **Project Type**: Exploratory Data Analysis & Statistical Modeling
