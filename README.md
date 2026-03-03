# Global HIV Mortality and Prevalance Analysis

This project analyses global HIV prevalence, infection burden, and HIV-related mortality to identify disparities in healthcare effectiveness across countries.

This study does not focus only on total cases or deaths, it also introduces a standardised mortality metric — Deaths per 1000 Infected — to evaluate treatment effectiveness and healthcare system performance.

The analysis supports evidence-based decision-making for global health organisations seeking to prioritise funding, intervention strategies, and treatment expansion.

## Business Problem
Global health organisations must determine:

Which countries experience disproportionately high HIV-related mortality relative to infection levels, and where should healthcare resources be prioritised?

Raw death counts alone do not accurately reflect healthcare system effectiveness. A country with a large infected population will naturally report higher total deaths.

This project addresses that gap by standardizing mortality relative to infection burden.

## Dataset
The dataset includes 193 countries and contains:
- Adult HIV prevalence (%)
- Number of people living with HIV
- Annual HIV-related deaths
- Year of estimate
Source: [Dataset extracted from Kaggle:HIV Prevalance study.csv]

## Tools & Technologies Used
- Python
- Pandas (Data cleaning & transformation)
- NumPy (Numerical processing)
- Matplotlib & Seaborn (Visualisation)
- Google Colab

## Methodologies 
### Data Cleaning and Processing
- Removed encoding inconsistencies
- Converted percentage fields to numeric format
- Standardised numeric columns (removed commas/symbols)
- Handled missing values
- Converted data types for analysis

### Feature Engineering
 #### Deaths per 1000 infected

Deaths per 1000=Total InfectedAnnual Deaths​×1000 

## Exploratory Data Analysis 
- Top 10 countries by prevalence
- Top 10 countries by cases
- Top 10 countries by deaths
- Identification of high-prevalence but low-mortality countries
- Outlier detection

## Correlation Analysis
Measured relationships between:

- Prevalence & deaths
- Cases & deaths

Findings show that while prevalence correlates with deaths, mortality is strongly influenced by healthcare access and treatment infrastructure.

## Key Findings
### 1. High prevalenvce ≠ High Mortality
Countries like South Africa show high prevalence but relatively lower deaths per 1000 infected compared to some lower-prevalence countries — indicating stronger treatment systems.

### 2. Disproportionate Mortality in Some Countries
Several countries with moderate prevalence exhibit high mortality per 1000 infected, suggesting limited access to antiretroviral therapy.

### 3. Cases Strongly Predict Deaths — But Not Perfectly
Correlation analysis shows:

- Strong relationship between total cases and deaths
- Weaker relationship between prevalence percentage and deaths
- This reinforces the importance of healthcare capacity.

## Business Impact 
#### This analysis provides:

- A standardised mortality metric for cross-country comparison
- A method to identify high-risk healthcare systems
- Insights to guide funding prioritization
- A framework for evaluating HIV treatment effectiveness

### The model can support organizations such as:

- World Health Organization
- UNAIDS
- The Global Fund
*As a way of allocating resources strategically.*

## Future Improvements
Integrate healthcare expenditure data
Add GDP per capita for socio-economic analysis
Build an interactive Power BI dashboard
Perform regression modeling for mortality prediction
