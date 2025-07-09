<h1 align='center'> Analysis of Eggplant Resistance in Fusarium Wilt | Experimental Data Analysis</h1>

This project presents a detailed data-driven analysis of eggplant genotypes evaluated for resistance against **Fusarium wilt**, a major fungal disease caused by *Fusarium oxysporum*. Using experimental data and robust statistical methods, the project identifies patterns in resistance, evaluates plant performance under disease stress, and supports decision-making in breeding and varietal selection programs.


## Objectives of the Analysis

1. **Determine variation in resistance levels** among different eggplant varieties based on disease incidence and severity.
2. **Analyze agronomic performance traits** (e.g., plant height, days to symptoms, survival rate) to assess the impact of infection.
3. **Statistically compare varieties** using inferential tests to identify significantly resistant genotypes.


## Dataset Description

The dataset is based on controlled experiments conducted to assess Fusarium wilt resistance in multiple eggplant genotypes. Each row represents an observation for a particular replicate of a genotype. The following features are included:

- `Variety`: Name or ID of the eggplant genotype  
- `Resistance Level`: Categorical label indicating resistance status (e.g., Resistant, Susceptible)  
- `Replication ID`: Identifier for replicate/block design to account for variability  
- `Infection Severity (%)`: Severity of wilt symptoms expressed as a percentage  
- `Wilt index`: Composite score rating intensity of wilt (quantitative disease index)  
- `Plant height (cm)`: Measured height of the plant in centimeters  
- `Days to wilt symptoms`: Number of days from planting until wilt symptoms appear  
- `Survival rate (%)`: Percentage of surviving plants at the end of the observation period  
- `Disease incidence (%)`: Percentage of plants showing visible disease symptoms  


## Methodology

This analysis follows a structured pipeline using Python for data cleaning, analysis, and visualization:

### 1. Data Preprocessing
- Checked for missing values, outliers, and inconsistencies.
- Converted categorical variables into standard formats.
- Normalized and transformed percentage-based variables where necessary.

### 2. Exploratory Data Analysis (EDA)
- Summarized key variables using descriptive statistics (mean, std, range).
- Created visual comparisons across varieties.

### 3. Statistical Analysis
- Evaluated homogeneity of varience assumptions with **Levene's tests**.
- Evaluated normality assumptions with **QQ plots** and **Shapiro-Wilk tests**.
- Applied **ANOVA** to test for significant differences across varieties.
- Used **Tukey’s Honest Significant Difference (HSD)** for pairwise comparisons.
- Constructed **Compact Letter Displays (CLD)** to summarize statistically similar groups.

### 4. Interpretation & Recommendation
- Ranked varieties based on resistance and agronomic performance.
- Highlighted genotypes with superior resistance and survival.
- Suggested candidates for further breeding and field validation.


## Key Findings

- Varieties classified as “Resistant” exhibited significantly lower infection severity and higher survival rates.
- Genotypes differed greatly in `Days to Wilt Symptoms`, indicating varied latency responses.
- A few susceptible varieties showed good plant height but poor resistance, suggesting the need for integrated selection criteria.


## 🛠 Tools and Libraries Used

- `pandas`: For data manipulation and wrangling  
- `numpy`: For numerical operations and data transformations  
- `matplotlib`: For basic plotting and custom visualizations  
- `seaborn`: For advanced statistical visualizations  
- `scipy.stats`: For statistical testing and hypothesis analysis  
- `statsmodels`: For ANOVA, Tukey HSD, and post-hoc comparisons  


## Project Structure
```
Analysis-of-Eggplant-Resistance-in-Fusarium-Wilt/
│
├── 📁 Datasets/              # Raw and/or cleaned data
├── 📁 Documents/             # Project background, survey forms, literature, references
├── 📁 Notebooks/             # Jupyter Notebooks for EDA, stats, etc.
├── 📁 Outputs/               # All outputs from analysis
├── 📁 Scripts/               # All reusable code/scripts
├── Analysis of Eggplant Resistance in Fusarium Wilt.ipynb
├── LICENSE
├── README.md
└── requirements.txt
└── __init__.py
```

## Author

This analysis was performed by **Jabulente**, a passionate and dedicated data analyst with a strong commitment to using data to drive meaningful insights and solutions. For inquiries, collaborations, or further discussions, please feel free to reach out via.  


<div align="center">  
    
[![GitHub](https://img.shields.io/badge/GitHub-Jabulente-black?logo=github)](https://github.com/Jabulente)  |  [![LinkedIn](https://img.shields.io/badge/LinkedIn-Jabulente-blue?logo=linkedin)](https://linkedin.com/in/jabulente-208019349)  |  [![Email](https://img.shields.io/badge/Email-jabulente@hotmail.com-red?logo=gmail)](mailto:Jabulente@hotmail.com)  

</div>


## License
This project is licensed under the MIT License. Feel free to use, share, and modify with attribution.

