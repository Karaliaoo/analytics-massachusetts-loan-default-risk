Contributors: Kara Liao, Roberto Albornoz, Sai Leela Rahul Pujari, Jungcheng (Leo) Zhu, Sarah Dsouza
Objectives:
* Build a Massachusetts loan-level risk view by combining LendingClub 2019 borrower features with local ACS socioeconomic indicators at the ZIP3 level.
* Quantify how credit quality (FICO, grade) and capacity-to-repay (DTI, term) drive default probability and pricing.
* Test whether community-level conditions (income, age structure) add incremental signal to borrower-level risk.

**Key Findings**:
* Default risk declines monotonically with higher FICO and better grades, and 60-month terms consistently carry higher PD than 36-month terms.
* Interest rates are inversely related to FICO and grade, indicating broadly consistent risk-based pricing.
* Employment length shows weak association with income, while lower local median household income areas exhibit higher delinquency rates.
  
Methods:
* Data Preparation: Cleaned and standardized LendingClub data. Derived key metrics such as Debt-to-Income (DTI), Revolving Balance, and Employment Length.
* Exploratory Data Analysis (EDA): Conducted national-level and Massachusetts-specific EDA through visualizations (violin, heatmap, bar, and correlation plots) to identify relationships between borrower risk factors (FICO, grade, term, purpose) and loan outcomes.
* Integration & Mapping: Joined borrower data with ZIP3-level ACS indicators (income, age, and population metrics) to visualize spatial variation in loan delinquency and median income across Massachusetts.
  
Recommendations:
* Anchor underwriting on FICO and grade, and add term-based PD uplifts to reflect longer exposure.
* Incorporate a simple geographic overlay (ZIP3 median income) as a tie-breaker for borderline files and for portfolio concentration limits.
* Favor smaller amounts and/or shorter terms for riskier grades, and monitor high-DTI pockets within low-income ZIP3s for early-warning signals.
