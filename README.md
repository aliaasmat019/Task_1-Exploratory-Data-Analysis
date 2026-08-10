# Task_1: Exploratory Data Analysis (EDA)

Exploratory analysis of the **Sample Superstore** dataset to understand its structure, quality, patterns, statistical relationships, and potential data issues before further analysis.

## Objectives

- Ask meaningful questions before analysis
- Explore variables and data types
- Identify patterns, distributions, and anomalies
- Validate relationships using statistics and visualization
- Detect data-quality issues relevant to further analysis

## Dataset

The supplied cleaned dataset contains **9,977 rows and 13 columns** covering sales, quantity, discount, profit, geography, customer segment, shipping mode, and product categories.

The dataset contains no missing values and no exact duplicate rows.

> Note: The file does not contain a date/time variable, so temporal trend analysis is not applicable to this dataset.

## Analysis Performed

### Data Understanding
- Dataset shape and sample records
- Numerical and categorical variables
- Data types and unique values
- Missing-value and duplicate checks

### Descriptive Analysis
- Summary statistics
- Total sales, profit, and quantity
- Average discount and overall profit margin
- Sales and profit distributions
- Category and regional performance

### Statistical Validation
**1. Spearman correlation — Discount vs Profit**  
Tests whether discount and profit have a monotonic relationship.

**2. Kruskal–Wallis test — Profit across Categories**  
Tests whether profit distributions differ across product categories.

### Anomaly Detection
IQR-based outlier detection is applied to numerical variables. Potential outliers are flagged for investigation rather than automatically removed.

## Key Findings

- Sales are concentrated around lower order values with a right-skewed distribution.
- Profit contains both profitable and loss-making orders.
- Discount has a statistically significant negative monotonic relationship with profit.
- Profit distributions differ significantly across product categories.
- Potential outliers exist in numerical variables and should be reviewed before advanced modeling.
- No missing values or exact duplicate rows were found in the supplied cleaned dataset.

## Tools

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook

## Repository Structure

```text
Task-1-EDA/
├── README.md
├── data/
│   └── SampleSuperstore_cleaned.csv
└── notebook/
    └── Task_1_EDA.ipynb
```

## How to Run

1. Open `notebook/Task_1_EDA.ipynb` in Jupyter Notebook, JupyterLab, or VS Code.
2. Make sure the required Python libraries are installed.
3. Run the notebook from top to bottom.

## Conclusion

The analysis provides a structured understanding of the dataset and establishes a reliable foundation for subsequent data analysis, visualization, or machine-learning work.
