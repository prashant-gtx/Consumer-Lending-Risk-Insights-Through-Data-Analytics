# Consumer Lending Risk Insights Through Data-Driven Analytics

## Project Overview
This project provides a comprehensive analysis of consumer lending risk. By leveraging data analytics techniques, it aims to derive actionable insights into applicant behavior, loan characteristics, and potential default risks. The analysis is documented in `Case_Study_Prashant.ipynb` and covers data cleaning, exploratory data analysis (EDA), and statistical modeling.

## Data Sources
The analysis utilizes two primary datasets:
1.  **`credit_risk_applicants.csv`**: Contains detailed information about current loan applicants, including demographics, income, credit amount, and employment history.
2.  **`credit_risk_previous_loans.csv`**: Provides historical data on previous loan applications and their outcomes.

## Methodology

### 1. Data Loading and Cleaning
-   Datasets are loaded using `pandas`.
-   **Missing Value Analysis**: Extensive checks for null values across columns.
-   **Feature Engineering**:
    -   Conversion of `DAYS_EMPLOYED` to `EMPLOYED_YEARS` for better interpretability.
    -   Handling anomalous values (e.g., replacing 365243 in `DAYS_EMPLOYED` with NaN).

### 2. Exploratory Data Analysis (EDA)
-   **Univariate Analysis**: Analyzing distributions of key variables such as:
    -   Income Total
    -   Credit Amount
    -   Annuity Amount
    -   Age (`DAYS_BIRTH` converted to years)
    -   Employment Duration
-   Visualizations using `matplotlib` and `seaborn` (Histograms, Distribution Plots) to identify patterns and outliers.

### 3. Statistical Analysis & Modeling
The project employs various statistical and machine learning libraries to understand risk factors:
-   **Statistical Tests**: `scipy.stats` (T-tests, Chi-square, etc.) and `statsmodels` for hypothesis testing.
-   **Predictive Modeling**: `sklearn` is used for data preprocessing (StandardScaler, LabelEncoder) and model selection (train_test_split), laying the groundwork for risk prediction models.

## Requirements
To run the analysis locally, ensure you have the following Python libraries installed:

```bash
pip install numpy pandas scipy statsmodels matplotlib seaborn scikit-learn
```

## Structure
-   **`Case_Study_Prashant.ipynb`**: The main notebook containing code, analysis, and visualizations.
-   **`Report_Case Study.docx`**: A summary report of findings and recommendations.
-   **`README.md`**: Project documentation.

## Usage
1.  Clone the repository.
2.  Install the required dependencies.
3.  Launch Jupyter Notebook: `jupyter notebook Case_Study_Prashant.ipynb`
4.  Execute the cells sequentially to reproduce the analysis.
