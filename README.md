# ESPN Cricket Batting Data Analysis

## Project Overview
This project transforms a raw ESPN cricket batting dataset into a structured, analysis-ready format to enable accurate career-level performance analysis. The work focuses on data quality assessment, controlled cleaning, feature engineering, and reproducible analysis using Python and Pandas in a Jupyter Notebook environment.

---

## Project Narrative

### Data Assessment & Structuring
The initial dataset contained valuable historical batting records but presented several structural limitations that would affect analytical accuracy:

- Non-descriptive column names reducing interpretability
- Career information stored as a single text field (`Span`)
- Country identifiers embedded within player names
- Missing values in key performance metrics
- Duplicate player records capable of distorting aggregate results

Addressing these issues was necessary to establish a reliable analytical foundation.

---

### Data Cleaning & Integrity Control
Column names were standardized to improve clarity and maintain consistency across the dataset.  
Missing values in `Balls_Faced` and `Bating_strike_rate` were isolated and replaced only after confirming they represented unavailable historical data rather than data corruption.

Duplicate player records were identified at the individual level and validated before removal. This step prevented inflation of averages and totals, ensuring statistical integrity.

---

### Feature Engineering & Normalization
To support longitudinal and comparative analysis, several derived features were created:

- Split `Span` into `Start_date` and `End_date`
- Engineered `Career_length` as a measurable career-duration metric
- Extracted `Country` into a standalone analytical column
- Normalized batting scores by removing special characters (e.g., `*`)
- Enforced correct data types for numerical consistency

These transformations converted text-heavy fields into structured variables suitable for aggregation and grouping.

---

### Analytical Outcomes
With a clean dataset, the analysis addressed career-oriented performance questions, including:

- Average career length among elite batters
- Average batting strike rate for players with long tenures
- Player distribution across historical eras
- Maximum innings played by country

All results were produced using reproducible Pandas operations to ensure transparency and repeatability.

---

### Business & Analytical Value
This project demonstrates the ability to:

- Evaluate real-world data quality issues
- Apply controlled, non-destructive data cleaning
- Engineer features aligned with analytical objectives
- Prevent statistical bias through data validation
- Convert raw domain-specific data into actionable insights

While the dataset is sports-focused, the workflow reflects production-level data preparation and analysis practices applicable across industries.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Jupyter Notebook

---


## Key Takeaway
The value of this project lies not in the domain, but in the analytical process: transforming imperfect, real-world data into a reliable foundation for insight-driven decision making.
