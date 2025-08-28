# 🗳️ Election Insight  

## 📌 Project Overview  
Election Insight analyzes **Indian state-wise election data (2008–2023)** with a special focus on:  
- Female participation and success rates in elections.  
- Trends and factors contributing to **NOTA (None of the Above)** votes.  

The project combines **data preprocessing, exploratory data analysis (EDA), and machine learning models** to uncover patterns in electoral data.  

---

## 🚀 Key Features  
- **Data Cleaning & Preprocessing**  
  - Removed redundant columns, standardized column names.  
  - Converted elector counts into absolute values (×1000).  
  - Imputed missing values (0 for third gender, median for NOTA).  

- **Exploratory Data Analysis (EDA)**  
  - Missing value heatmaps and correlation matrices.  
  - Female representation trends (stacked bar plots, violin plots).  
  - Scatterplots between electors and success rates.  
  - Trend analysis of NOTA votes across years and states.  

- **Machine Learning Models**  
  - **Gradient Boosting Regressor** → Predicting number of *elected female candidates*.  
    - Best RMSE: **0.85**  
    - Top Features: *Female Contestants*, *Elected Female %*, *Total Elected Candidates*  
  - **Random Forest Classifier** → Classifying NOTA votes (Low/Medium/High).  
    - Accuracy: **90%** (baseline)  
    - PCA variant with top 6 components → Accuracy: **63%**  

---

## 📊 Dataset  
- **Source**: `CLeaned State Wise Data 2008-2013.xlsx`  
- **Features include**:  
  - Elector demographics (Male, Female, Total)  
  - Contestants (Male, Female, Third Gender)  
  - Elected candidates and success rates  
  - Voter turnout percentages  
  - NOTA votes distribution  

---

## ⚙️ Tools & Technologies  
- **Languages**: Python  
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Plotly, Scikit-learn  
- **Techniques**: Data Cleaning, Feature Engineering, Gradient Boosting, Random Forest, PCA, Clustering  

---

## 📂 Repository Structure  

```text
├── CLeaned State Wise Data 2008-2013.xlsx   # State-wise election dataset
├── Election_recheck.ipynb                   # Notebook with preprocessing, EDA & ML
└── README.md                                # Project documentation
