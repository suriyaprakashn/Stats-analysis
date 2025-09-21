# Statistical Analysis Projects

This repository contains two statistical analysis projects:
1. FIFA World Cup Player Dataset Analysis
2. Mobile Network Dataset Analysis

## 📊 Project 1: FIFA World Cup Player Analysis

### Dataset Overview
The dataset contains player information from FIFA World Cup, including:
- Height, Weight, Overall Rating, Potential
- Preferred Foot, Skill Moves, and other attributes

### Analysis Performed

#### a) Central Limit Theorem with Age Population
- Performed CLT with sample size of 200
- Calculated standard error and mean of sampling distribution
- Compared with population mean and standard deviation
- Explanation of why standard error decreases with increased sample size

#### b) Hypothesis Test: Overall Rating > 80
- One-sample t-test to check if average overall rating exceeds 80
- Significance level: α = 0.05

#### c) Preferred Foot vs Potential Analysis
- Statistical test (t-test) to examine foot preference impact on potential
- Graphical analysis (box plots, bar charts)

#### d) Relationship: Overall Rating vs Potential
- Correlation analysis between two continuous variables
- Regression analysis to quantify relationship

#### e) Skill Moves Effect on Overall Rating
- Graphical analysis (grouped visualizations)
- Statistical analysis (ANOVA or t-tests)

### Technical Specifications
- Significance level: 5% (α = 0.05)
- Assumed normal distribution and equal variance
- Used appropriate statistical tests for each analysis

## 📶 Project 2: Mobile Network Analysis

### Dataset Overview
The dataset contains information about:
- Internet usage, calls, and messages across various networks
- Network types and duration metrics

### Analysis Performed

#### a) Confidence Interval for Call Duration
- Calculated 95% and 99% confidence intervals for average call duration
- Compared interval widths and interpreted results

#### b) Network Distribution Analysis
- Statistical test to check if networks are equally distributed
- Chi-square goodness-of-fit test

#### c) Duration Distribution by Network
- Plotted distribution of call duration for each network
- Comparative graphical analysis

#### d) Relationship: Item vs Duration
- Statistical tests to identify relationships
- Detailed explanation of class relationships

#### e) Relationship: Network vs Network Type
- Statistical analysis of categorical variables
- Appropriate tests for association

### Technical Specifications
- Significance level: 5% (α = 0.05)
- Performed tests of normality (Shapiro-Wilk, Kolmogorov-Smirnov)
- Performed tests of variance (Levene's test, Bartlett's test)
- Used appropriate statistical tests based on data characteristics

## 🛠️ Technical Requirements

### Python Libraries Required
```python
# Statistical Analysis
import pandas as pd
import numpy as np
import scipy.stats as stats
from scipy.stats import ttest_ind, ttest_rel, f_oneway, chi2_contingency
from scipy.stats import norm, shapiro, levene

# Data Visualization
import matplotlib.pyplot as plt
import seaborn as sns
from statsmodels.graphics.gofplots import qqplot

# Data Processing
from sklearn.preprocessing import LabelEncoder
from sklearn.impute import SimpleImputer
```

### Installation
```bash
pip install pandas numpy scipy matplotlib seaborn statsmodels scikit-learn
```

## 📁 Project Structure

```
statistical-analysis-projects/
│
│── fifa_world_cup.csv
│── mobile_network.csv
│
├── analysis.ipynb
│
└── README.md
```

## 🧮 Statistical Methods Used

### Hypothesis Testing
- One-sample t-test
- Two-sample t-test
- ANOVA
- Chi-square tests
- Correlation analysis
- Regression analysis

### Diagnostic Tests
- Normality tests (Shapiro-Wilk, Kolmogorov-Smirnov)
- Variance tests (Levene's test, Bartlett's test)
- Goodness-of-fit tests

### Visualization Techniques
- Histograms and density plots
- Box plots and violin plots
- Q-Q plots for normality assessment
- Scatter plots and correlation matrices
- Confidence interval plots

## 📈 Key Findings

### FIFA Dataset
- Central limit theorem demonstration with age data
- Evidence regarding overall rating exceeding 80
- Impact of preferred foot on player potential
- Relationship between overall rating and potential
- Effect of skill moves on overall rating

### Mobile Network Dataset
- Confidence intervals for call duration
- Network distribution patterns
- Duration patterns across different networks
- Relationships between various network metrics

## 📋 How to Run

1. Clone the repository:
```bash
git clone <repository-url>
cd statistical-analysis-projects
```

2. Run the analysis notebooks:
```bash
jupyter notebook notebooks/nalysis.ipynb
```


## 📊 Results Interpretation

All statistical tests were performed with a significance level of α = 0.05. Results include:
- p-values and test statistics
- Confidence intervals
- Effect sizes where appropriate
- Graphical representations
- Practical interpretations

## 🤝 Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 🎯 Future Enhancements

- Additional statistical models
- Machine learning integration
- Interactive dashboards
- Real-time data analysis capabilities
- Expanded dataset incorporation

---

**Note**: This project demonstrates comprehensive statistical analysis techniques applied to real-world datasets. The code and methodologies can be adapted for similar analytical problems in sports analytics and telecommunications domains.
