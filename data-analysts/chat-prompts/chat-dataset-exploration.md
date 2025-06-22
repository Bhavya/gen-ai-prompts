# Dataset Exploration - Chat Prompt

## Purpose
A systematic approach to exploring and understanding new datasets before conducting detailed analysis.

## Chat Prompt

```
I have a new dataset that I need to explore and understand before diving into specific analysis. Let's work through a comprehensive exploratory data analysis (EDA) process to uncover insights and identify potential issues.

## Dataset Context:
- **Source**: [Where did this data come from?]
- **Business Context**: [What business process or domain does this data represent?]
- **Time Period**: [What time range does the data cover?]
- **Size**: [Number of rows and columns, approximate file size]
- **Format**: [CSV, database table, JSON, etc.]

## Data Description:
[Provide a brief description of what each key column represents, or share a data dictionary if available]

## Business Questions:
[What are you ultimately trying to answer with this data?]
- Primary question: [Main analytical objective]
- Secondary questions: [Additional insights you're seeking]

## Exploration Goals:
Please help me systematically explore this dataset by guiding me through:

### 1. Initial Data Assessment
- **Data Structure**: Understanding column types, relationships, and hierarchy
- **Completeness**: Identifying missing values, null patterns, and data gaps
- **Quality Issues**: Spotting inconsistencies, duplicates, and anomalies
- **Sample Review**: Examining representative records to understand data patterns

### 2. Descriptive Statistics
- **Numerical Variables**: Distributions, central tendencies, and spread
- **Categorical Variables**: Frequency distributions and unique values
- **Date/Time Variables**: Time series patterns and seasonality
- **Cross-Variable Relationships**: Correlations and associations

### 3. Data Visualization
- **Distribution Plots**: Histograms, box plots, and density plots for key variables
- **Relationship Analysis**: Scatter plots and correlation matrices
- **Time Series Plots**: Trends and patterns over time
- **Categorical Analysis**: Bar charts and proportion analysis

### 4. Anomaly Detection
- **Outliers**: Statistical outliers and their potential causes
- **Data Consistency**: Inconsistent formats, values, or patterns
- **Business Logic Validation**: Values that don't make business sense

### 5. Feature Assessment
- **Relevance**: Which variables are most relevant to our business questions?
- **Predictive Power**: Which features might be useful for modeling?
- **Data Leakage**: Any variables that might cause analytical issues?
- **Engineering Opportunities**: Potential new features to create

## Current Data Sample:
[If possible, provide a sample of your data - first few rows, column names, or summary statistics]

## Tools Available:
[What tools are you using? Python/Pandas, R, SQL, Excel, Tableau, etc.]

Let's start with a structured exploration plan that will give us a comprehensive understanding of this dataset and prepare us for deeper analysis.
```

## Usage Tips
- Share actual data samples when possible (anonymized if sensitive)
- Be specific about your business domain and context
- Mention any known data quality issues upfront
- Include information about how the data was collected
- Specify your analysis timeline and deliverable requirements

## Expected Exploration Steps
1. **Data Loading and Initial Inspection**
2. **Missing Value Analysis**
3. **Descriptive Statistics Summary**
4. **Distribution Analysis**
5. **Correlation and Relationship Exploration**
6. **Outlier Detection and Investigation**
7. **Data Quality Assessment**
8. **Feature Relevance Evaluation**

## Example Usage

"I have a new dataset of customer support tickets from the past year that I need to explore. The dataset has 50k rows with columns like ticket_id, customer_id, issue_category, priority, resolution_time, satisfaction_score, and created_date.

Business context: We want to understand what drives customer satisfaction and identify opportunities to improve support efficiency.

Main questions: What factors predict customer satisfaction? Which issue types take longest to resolve? Are there seasonal patterns in ticket volume?

I'm using Python/Pandas and have access to the full dataset. Looking to create a comprehensive EDA before building predictive models."