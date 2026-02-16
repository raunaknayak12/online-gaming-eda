# Online Gaming Behavior - Exploratory Data Analysis

## 📊 Project Overview
This project performs comprehensive exploratory data analysis (EDA) on online gaming behavior data from India. The analysis covers various aspects of gaming habits, including play time, spending patterns, demographics, and their correlations.

## 📁 Project Structure
```
online-gaming-eda/
│
├── data/                                    # Dataset folder
│   └── online_gaming_behavior_cleaned (1).xlsx
│
├── notebooks/                               # Jupyter notebooks
│   └── Online_Gaming_EDA.ipynb
│
├── README.md                                # Project documentation
├── requirements.txt                         # Python dependencies
└── .gitignore                              # Git ignore file
```

## 📈 Analysis Highlights

The EDA covers:
- **Data Cleaning**: Handling missing values, standardizing categories, converting data types
- **Statistical Analysis**: Distribution of play hours and monthly spending
- **Demographic Analysis**: Age, gender, and regional patterns
- **Behavioral Insights**: Game type preferences, public WiFi usage, internet scheme adoption
- **Impact Assessment**: Health issues and academic/work impact analysis
- **Visualizations**: Distribution plots, correlation analysis

## 🔍 Key Findings

### Dataset Overview
- **500 users** with 11 features
- Features include: user demographics, play time, spending, game preferences, and impact indicators

### Data Quality
- Successfully handled missing values using appropriate imputation strategies
- Standardized categorical values (gender, region, WiFi usage)
- Removed negative/invalid values from numerical columns

### Main Insights
- Average daily play hours: **5.38 hours**
- Median monthly spend: **₹2,483**
- Data shows relatively normal distributions for both metrics

## 🛠️ Technologies Used
- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computing
- **matplotlib** - Data visualization
- **seaborn** - Statistical data visualization
- **openpyxl** - Excel file handling

## 🚀 Getting Started

### Prerequisites
```bash
pip install -r requirements.txt
```

### Running the Analysis
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Open the Jupyter notebook: `jupyter notebook notebooks/Online_Gaming_EDA.ipynb`
4. Run all cells to reproduce the analysis

## 📊 Dataset Information

The dataset contains cleaned online gaming behavior data with the following features:
- `user_id`: Unique identifier
- `age`: User age
- `gender`: User gender
- `region`: Urban/Rural classification
- `avg_daily_play_hours`: Average daily gaming time
- `preferred_game_type`: Favorite game genre
- `uses_public_wifi`: Public WiFi usage indicator
- `monthly_spend_inr`: Monthly gaming expenditure in INR
- `government_internet_scheme`: Participation in government schemes
- `reported_health_issues`: Health impact indicator
- `academic_or_work_impact`: Impact on studies/work

## 📝 License
This project is available for educational and research purposes.

## 🤝 Contributing
Feel free to fork this repository and submit pull requests for any improvements.

## 📧 Contact
For questions or feedback, please open an issue in this repository.

---
**Note**: This is an educational project for learning data analysis and visualization techniques.
