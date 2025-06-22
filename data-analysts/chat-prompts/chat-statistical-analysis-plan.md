# Statistical Analysis Plan - Chat Prompt

## Purpose
Design a rigorous statistical analysis approach to answer business questions with confidence and generate actionable insights from data.

## Chat Prompt

```
I need help designing a comprehensive statistical analysis plan to answer specific business questions with rigor and confidence. Let's create a systematic approach that ensures valid conclusions and actionable insights.

## Analysis Context:
- **Business Question**: [What specific question are you trying to answer?]
- **Decision Context**: [What decision will this analysis inform?]
- **Stakeholder Audience**: [Who will use these results? Technical level?]
- **Timeline**: [When do you need results? How much time for analysis?]
- **Impact Level**: [How critical is this analysis to business decisions?]

## Research Objectives:

### Primary Question:
**Main Hypothesis**: [What is your primary hypothesis or assumption to test?]
- **Null Hypothesis (H0)**: [Statement of no effect or no difference]
- **Alternative Hypothesis (H1)**: [Statement of the effect you expect to find]
- **Expected Outcome**: [What result do you anticipate and why?]

### Secondary Questions:
[Additional questions that support or extend the primary analysis]
1. **Question 2**: [Supporting analysis question]
2. **Question 3**: [Additional exploratory question]
3. **Question 4**: [Segmentation or subgroup analysis]

### Success Criteria:
- **Statistical Significance**: [What p-value threshold will you use? (0.05, 0.01, etc.)]
- **Practical Significance**: [What size effect would be meaningful for business?]
- **Confidence Level**: [What confidence level do you need for conclusions?]
- **Decision Framework**: [How will results inform specific actions?]

## Data Overview:

### Data Sources:
**Primary Dataset**:
- **Source**: [Where does this data come from?]
- **Time Period**: [Date range and data collection period]
- **Sample Size**: [Number of observations/records]
- **Update Frequency**: [How often is data refreshed?]

**Supplementary Data**:
- **External Data**: [Third-party data, industry benchmarks, economic indicators]
- **Historical Data**: [Past data for trends and comparisons]
- **Control Data**: [Comparison groups or baseline measurements]

### Key Variables:

**Dependent Variables** (Outcomes you're measuring):
- **Variable 1**: [Primary outcome measure]
  - **Type**: [Continuous, categorical, binary, count]
  - **Distribution**: [Normal, skewed, etc.]
  - **Scale**: [Units of measurement]
  - **Business Meaning**: [What this represents in business terms]

**Independent Variables** (Factors that might influence outcomes):
- **Variable 1**: [Primary predictor or treatment]
  - **Type**: [Continuous, categorical, binary]
  - **Values**: [Range or categories]
  - **Business Meaning**: [What this represents]

**Control Variables** (Factors to account for):
- [Variables that might confound results and need to be controlled]

**Segmentation Variables**:
- [Dimensions for subgroup analysis - demographics, behavior, etc.]

## Statistical Methodology:

### Analysis Approach:
**Primary Analysis Method**:
- [ ] **Descriptive Analysis**: [Summary statistics, distributions, trends]
- [ ] **Comparison Tests**: [t-tests, chi-square, ANOVA]
- [ ] **Correlation Analysis**: [Pearson, Spearman correlation]
- [ ] **Regression Analysis**: [Linear, logistic, multiple regression]
- [ ] **Time Series Analysis**: [Trend analysis, seasonality, forecasting]
- [ ] **Experimental Analysis**: [A/B testing, randomized controlled trials]

**Specific Statistical Tests**:
[Based on your data type and research questions]
- **Test 1**: [Specific test for primary hypothesis]
  - **Assumptions**: [Statistical assumptions to verify]
  - **Sample Size Requirements**: [Minimum sample size needed]
  - **Expected Power**: [Statistical power calculation]

### Analysis Plan Structure:

**Phase 1: Exploratory Data Analysis**
- **Data Quality Assessment**: [Missing values, outliers, data integrity]
- **Descriptive Statistics**: [Central tendencies, distributions, variability]
- **Visualization**: [Key charts and graphs for understanding data]
- **Assumption Testing**: [Testing statistical assumptions for planned analyses]

**Phase 2: Primary Analysis**
- **Hypothesis Testing**: [Main statistical tests for primary questions]
- **Effect Size Calculation**: [Magnitude of effects, not just significance]
- **Confidence Intervals**: [Range estimates for key parameters]
- **Sensitivity Analysis**: [How robust are results to different assumptions?]

**Phase 3: Secondary Analysis**
- **Subgroup Analysis**: [Results across different segments]
- **Interaction Effects**: [How factors combine to influence outcomes]
- **Robustness Testing**: [Alternative analytical approaches]
- **Practical Significance**: [Business interpretation of statistical results]

## Sample Size & Power Analysis:

### Power Calculation:
**Required Inputs**:
- **Effect Size**: [Minimum meaningful difference to detect]
- **Statistical Power**: [Probability of detecting effect if it exists (typically 80%)]
- **Significance Level**: [Type I error rate (typically 5%)]
- **Variability**: [Expected variance in the data]

**Sample Size Requirements**:
- **Minimum Sample Size**: [For adequate statistical power]
- **Current Sample Size**: [What you actually have available]
- **Power Analysis**: [What effect size can you detect with current sample?]
- **Sample Size Justification**: [Why this sample size is adequate]

### Data Collection Considerations:
- **Sampling Method**: [Random, stratified, convenience sampling approach]
- **Bias Prevention**: [How to minimize selection and measurement bias]
- **Data Quality**: [Ensuring accurate and complete data collection]

## Assumptions & Limitations:

### Statistical Assumptions:
**Key Assumptions to Test**:
- **Normality**: [Are continuous variables normally distributed?]
- **Independence**: [Are observations independent of each other?]
- **Homoscedasticity**: [Equal variance across groups]
- **Linearity**: [Linear relationship between variables]

**Assumption Testing Plan**:
- **Testing Methods**: [Specific tests for each assumption]
- **Remedial Actions**: [What to do if assumptions are violated]
- **Alternative Approaches**: [Non-parametric or robust alternatives]

### Analysis Limitations:
**Data Limitations**:
- **Missing Data**: [How will you handle missing values?]
- **Sample Bias**: [Potential biases in data collection]
- **Temporal Limitations**: [Time period constraints]
- **Measurement Limitations**: [Accuracy and precision constraints]

**Analytical Limitations**:
- **Causation vs. Correlation**: [Can you establish causation?]
- **Confounding Variables**: [Unmeasured factors that might affect results]
- **Generalizability**: [How broadly do results apply?]
- **Statistical Power**: [What effects might you miss?]

## Data Analysis Workflow:

### Step-by-Step Process:
**Data Preparation**:
1. **Data Import & Cleaning**: [Loading data, handling missing values]
2. **Variable Creation**: [Derived variables, transformations]
3. **Data Validation**: [Checking data quality and consistency]
4. **Outlier Treatment**: [Identifying and handling extreme values]

**Exploratory Analysis**:
1. **Descriptive Statistics**: [Summary measures for all variables]
2. **Data Visualization**: [Histograms, scatter plots, box plots]
3. **Correlation Matrix**: [Relationships between variables]
4. **Assumption Checking**: [Testing statistical assumptions]

**Primary Analysis**:
1. **Hypothesis Testing**: [Main statistical tests]
2. **Effect Size Calculation**: [Practical significance measures]
3. **Confidence Intervals**: [Uncertainty quantification]
4. **Model Diagnostics**: [Checking model fit and assumptions]

### Tools & Software:
**Analysis Platform**:
- [ ] **R/RStudio**: [For comprehensive statistical analysis]
- [ ] **Python**: [pandas, scipy, statsmodels, scikit-learn]
- [ ] **SQL**: [For data extraction and preparation]
- [ ] **Excel**: [For simple analyses and stakeholder communication]
- [ ] **Specialized Tools**: [SPSS, SAS, Stata for specific analyses]

## Results Interpretation:

### Statistical Interpretation:
**Significance Testing**:
- **P-value Interpretation**: [What do different p-values mean?]
- **Multiple Comparison Correction**: [Adjusting for multiple tests]
- **Confidence Interval Interpretation**: [Range of plausible values]
- **Effect Size Interpretation**: [Practical importance of findings]

**Model Results**:
- **Coefficient Interpretation**: [What do model parameters mean?]
- **Model Fit Assessment**: [How well does model explain data?]
- **Prediction Accuracy**: [How accurate are model predictions?]
- **Variable Importance**: [Which factors matter most?]

### Business Translation:
**Practical Implications**:
- **Business Impact**: [What do results mean for business decisions?]
- **Action Items**: [Specific actions suggested by analysis]
- **Risk Assessment**: [Uncertainty and potential risks]
- **ROI Estimation**: [Expected return on suggested actions]

## Quality Assurance:

### Validation Methods:
**Results Validation**:
- **Cross-Validation**: [Testing model performance on holdout data]
- **Sensitivity Analysis**: [How sensitive are results to assumptions?]
- **Replication**: [Can results be reproduced with different samples?]
- **Peer Review**: [Having colleagues review methodology and results]

**Error Prevention**:
- **Code Review**: [Having analysis code reviewed for errors]
- **Data Verification**: [Double-checking data accuracy]
- **Method Verification**: [Confirming appropriate statistical methods]
- **Results Checking**: [Verifying calculations and interpretations]

## Reporting & Communication:

### Analysis Report Structure:
**Executive Summary**:
- **Key Findings**: [Main results in business terms]
- **Recommendations**: [Specific actions based on results]
- **Confidence Level**: [How certain are we about conclusions?]
- **Next Steps**: [Follow-up analysis or actions needed]

**Technical Details**:
- **Methodology**: [Statistical methods used]
- **Assumptions**: [Key assumptions and validation]
- **Limitations**: [What the analysis cannot tell us]
- **Technical Appendix**: [Detailed results for technical audience]

### Visualization Strategy:
- **Key Charts**: [Most important visualizations for understanding]
- **Statistical Graphics**: [Confidence intervals, effect size plots]
- **Business Dashboards**: [Metrics and KPIs for ongoing monitoring]

## Specific Guidance Needed:

1. **Method Selection**: Which statistical methods are most appropriate for my data and questions?
2. **Sample Size**: Is my sample size adequate for reliable conclusions?
3. **Assumption Testing**: How should I test and handle violated assumptions?
4. **Business Translation**: How do I translate statistical results into business insights?
5. **Quality Assurance**: What validation steps should I include?
6. **Communication**: How should I present results to non-technical stakeholders?

Let's design a statistical analysis that generates reliable, actionable insights for your business decisions!
```

## Usage Tips
- Clearly define your research questions before diving into analysis methods
- Always test statistical assumptions and use appropriate alternatives when violated
- Calculate effect sizes along with p-values to assess practical significance
- Include confidence intervals to communicate uncertainty in results
- Plan for validation and sensitivity analysis to ensure robust conclusions

## Example Usage

"I need help designing a statistical analysis to determine whether our new onboarding process improves user retention. We have 6 months of data with 10k users split between old and new onboarding flows. Primary question: Does the new process increase 30-day retention rates? Secondary questions: Which user segments benefit most? Are there differences in feature adoption? Need to present results to executive team in 2 weeks with confidence level for rollout decision."