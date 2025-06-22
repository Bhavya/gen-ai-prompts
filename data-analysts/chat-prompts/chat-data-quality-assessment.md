# Data Quality Assessment - Chat Prompt

## Purpose
Systematically evaluate and improve data quality to ensure reliable analysis and trustworthy insights for business decisions.

## Chat Prompt

```
I need help conducting a comprehensive data quality assessment to identify issues and implement improvements that ensure reliable analysis. Let's create a systematic approach to evaluating and enhancing data quality.

## Data Context:
- **Data Source**: [Where does this data come from? Database, API, files, etc.]
- **Data Type**: [Customer data, transaction data, web analytics, survey data, etc.]
- **Business Use**: [How is this data used for business decisions?]
- **Data Volume**: [Size of dataset - rows, columns, file size]
- **Update Frequency**: [How often is data refreshed or updated?]

## Data Quality Framework:

### Quality Dimensions:
**Completeness**:
- **Definition**: [Extent to which data is present and not missing]
- **Business Impact**: [How do missing values affect analysis and decisions?]
- **Measurement**: [Percentage of missing values by field and record]

**Accuracy**:
- **Definition**: [Extent to which data correctly represents reality]
- **Business Impact**: [How do inaccurate values affect business outcomes?]
- **Measurement**: [Error rates, validation against source systems]

**Consistency**:
- **Definition**: [Extent to which data is uniform across systems and time]
- **Business Impact**: [How do inconsistencies affect analysis reliability?]
- **Measurement**: [Discrepancies between related fields or systems]

**Validity**:
- **Definition**: [Extent to which data conforms to defined formats and rules]
- **Business Impact**: [How do format violations affect data processing?]
- **Measurement**: [Percentage of values meeting format requirements]

**Timeliness**:
- **Definition**: [Extent to which data is current and up-to-date]
- **Business Impact**: [How does data age affect decision quality?]
- **Measurement**: [Data freshness, lag time from event to availability]

**Uniqueness**:
- **Definition**: [Extent to which records are unique and not duplicated]
- **Business Impact**: [How do duplicates affect counts and analysis?]
- **Measurement**: [Duplicate rate, record matching accuracy]

## Assessment Scope:

### Data Sources to Evaluate:
**Primary Data Source**:
- **Source Name**: [Database, API, file system]
- **Key Tables/Files**: [Most important data entities]
- **Critical Fields**: [Fields essential for business decisions]
- **Data Lineage**: [Where does this data originate?]

**Related Data Sources**:
- [Additional sources that integrate or relate to primary data]
- [Reference data, lookup tables, external data]

### Key Data Elements:
**Critical Business Fields**:
1. **Field Name**: [e.g., Customer ID]
   - **Business Importance**: [Why this field is critical]
   - **Data Type**: [String, integer, date, etc.]
   - **Expected Format**: [Format requirements and rules]
   - **Business Rules**: [Validation rules and constraints]

2. **Field Name**: [e.g., Transaction Amount]
   - **Business Importance**: [Revenue impact, compliance requirements]
   - **Data Type**: [Decimal, currency]
   - **Expected Range**: [Valid value ranges]
   - **Business Rules**: [Must be positive, currency format, etc.]

## Quality Assessment Plan:

### Completeness Analysis:
**Missing Value Assessment**:
- **Field-Level Analysis**: [Missing percentage for each important field]
- **Record-Level Analysis**: [Records with any missing critical values]
- **Pattern Analysis**: [Are missing values random or systematic?]
- **Business Impact**: [Which missing values affect analysis most?]

**Completeness Tests**:
```sql
-- Example: Calculate missing value percentages
SELECT 
    column_name,
    COUNT(*) as total_records,
    COUNT(column_name) as non_null_records,
    (COUNT(*) - COUNT(column_name)) as missing_records,
    ROUND(((COUNT(*) - COUNT(column_name)) * 100.0 / COUNT(*)), 2) as missing_percentage
FROM your_table
GROUP BY column_name;
```

### Accuracy Analysis:
**Data Validation Tests**:
- **Range Validation**: [Values within expected business ranges]
- **Format Validation**: [Data matches expected patterns]
- **Cross-Reference Validation**: [Comparison with authoritative sources]
- **Business Rule Validation**: [Compliance with business logic]

**Accuracy Metrics**:
- **Error Rate**: [Percentage of records with inaccurate values]
- **Precision**: [Correctness of specific field values]
- **Source Verification**: [Comparison with original data sources]

### Consistency Analysis:
**Internal Consistency**:
- **Field Relationships**: [Do related fields have consistent values?]
- **Temporal Consistency**: [Are values consistent over time?]
- **Format Consistency**: [Consistent formatting across records]

**Cross-System Consistency**:
- **Data Synchronization**: [Consistency between integrated systems]
- **Reference Data**: [Consistency with master data and lookups]
- **Version Control**: [Consistency across different data versions]

**Consistency Tests**:
```sql
-- Example: Check for inconsistent relationships
SELECT 
    customer_id,
    COUNT(DISTINCT country) as country_count,
    COUNT(DISTINCT currency) as currency_count
FROM transactions
GROUP BY customer_id
HAVING COUNT(DISTINCT country) > 1 OR COUNT(DISTINCT currency) > 1;
```

### Validity Analysis:
**Format Validation**:
- **Data Type Checking**: [Correct data types for each field]
- **Pattern Matching**: [Email formats, phone numbers, IDs]
- **Domain Validation**: [Values from predefined lists or ranges]
- **Length Validation**: [Field lengths within specifications]

**Business Rule Validation**:
- **Constraint Validation**: [Business rules and constraints]
- **Logical Validation**: [Logical relationships between fields]
- **Regulatory Compliance**: [Compliance with industry standards]

### Timeliness Analysis:
**Data Freshness**:
- **Update Lag**: [Time from event occurrence to data availability]
- **Processing Delays**: [Delays in data processing pipeline]
- **Refresh Frequency**: [How often data is updated vs. requirements]
- **Historical Coverage**: [Availability of historical data]

**Timeliness Metrics**:
- **Average Data Age**: [How old is the data on average?]
- **Update Frequency**: [Actual vs. required update frequency]
- **Processing Time**: [Time to process and make data available]

### Uniqueness Analysis:
**Duplicate Detection**:
- **Exact Duplicates**: [Identical records across all fields]
- **Near Duplicates**: [Records that are similar but not identical]
- **Business Key Duplicates**: [Duplicates based on business logic]
- **Cross-Source Duplicates**: [Duplicates across different data sources]

**Duplicate Analysis Methods**:
```sql
-- Example: Find potential duplicates
SELECT 
    email,
    COUNT(*) as duplicate_count
FROM customers
GROUP BY email
HAVING COUNT(*) > 1;
```

## Data Profiling:

### Statistical Profiling:
**Descriptive Statistics**:
- **Central Tendency**: [Mean, median, mode for numerical fields]
- **Variability**: [Standard deviation, range, quartiles]
- **Distribution Shape**: [Skewness, kurtosis, histogram analysis]
- **Outlier Detection**: [Values outside normal ranges]

**Categorical Analysis**:
- **Value Frequency**: [Most and least common values]
- **Cardinality**: [Number of unique values]
- **Value Distribution**: [Spread of categorical values]
- **Unexpected Values**: [Values not in expected lists]

### Pattern Analysis:
**Data Patterns**:
- **Common Formats**: [Typical patterns in text fields]
- **Seasonal Patterns**: [Time-based patterns in data]
- **Growth Patterns**: [Trends in data volume and values]
- **Anomaly Patterns**: [Unusual patterns that need investigation]

## Quality Issues Identification:

### Common Data Quality Issues:
**Completeness Issues**:
- [ ] Missing required fields
- [ ] Incomplete records
- [ ] NULL values in critical fields
- [ ] Empty strings vs. NULL values

**Accuracy Issues**:
- [ ] Out-of-range values
- [ ] Incorrect data types
- [ ] Calculation errors
- [ ] Transcription errors

**Consistency Issues**:
- [ ] Conflicting data across systems
- [ ] Different formats for same data
- [ ] Inconsistent naming conventions
- [ ] Temporal inconsistencies

**Validity Issues**:
- [ ] Invalid formats (emails, dates, IDs)
- [ ] Values outside allowed ranges
- [ ] Constraint violations
- [ ] Referential integrity issues

### Root Cause Analysis:
**Issue Classification**:
- **Data Entry Errors**: [Manual input mistakes]
- **System Integration Issues**: [Problems in data transfer]
- **Process Issues**: [Flawed data collection processes]
- **Technical Issues**: [System bugs, hardware problems]

**Impact Assessment**:
- **Business Impact**: [How issues affect business decisions]
- **Analysis Impact**: [How issues affect data analysis accuracy]
- **Operational Impact**: [How issues affect day-to-day operations]
- **Compliance Impact**: [Regulatory or audit implications]

## Quality Improvement Plan:

### Immediate Actions:
**Critical Issues** (Fix immediately):
1. **Issue**: [Description of critical quality issue]
   - **Impact**: [Business impact of this issue]
   - **Solution**: [Specific steps to fix]
   - **Timeline**: [When to implement fix]
   - **Owner**: [Who is responsible for fix]

2. **Issue**: [Another critical issue]
   - [Same structure]

### Medium-Term Improvements:
**Process Improvements**:
- **Data Validation Rules**: [Implement validation at data entry]
- **Quality Monitoring**: [Set up ongoing quality monitoring]
- **Data Governance**: [Establish data stewardship processes]
- **Training**: [Train staff on data quality importance]

### Long-Term Strategy:
**Systematic Improvements**:
- **Data Architecture**: [Improve data architecture for quality]
- **Master Data Management**: [Implement MDM for consistency]
- **Automated Quality Checks**: [Build automated quality monitoring]
- **Quality Culture**: [Build organization-wide quality awareness]

## Monitoring & Maintenance:

### Quality Metrics Dashboard:
**Key Quality Indicators**:
- **Completeness Score**: [Percentage of complete records]
- **Accuracy Score**: [Percentage of accurate values]
- **Consistency Score**: [Consistency across systems]
- **Timeliness Score**: [Data freshness metrics]

**Monitoring Frequency**:
- **Daily**: [Critical quality checks for operational data]
- **Weekly**: [Comprehensive quality review]
- **Monthly**: [Quality trend analysis and reporting]
- **Quarterly**: [Full quality assessment and improvement planning]

### Quality Alerts:
**Alert Thresholds**:
- **Completeness**: [Alert when missing values exceed X%]
- **Accuracy**: [Alert when error rates exceed X%]
- **Timeliness**: [Alert when data age exceeds X hours]
- **Volume**: [Alert for unexpected data volume changes]

## Specific Guidance Needed:

1. **Assessment Prioritization**: Which quality dimensions should I focus on first?
2. **Testing Strategy**: What specific tests should I run for my data type?
3. **Tool Selection**: What tools are best for automated quality assessment?
4. **Issue Prioritization**: How should I prioritize quality issues for fixing?
5. **Monitoring Setup**: How to establish ongoing quality monitoring?
6. **Success Metrics**: How to measure improvement in data quality?

## Current State:
- **Known Issues**: [Any quality issues you're already aware of]
- **Previous Assessments**: [Any prior data quality work done]
- **Current Tools**: [Tools currently used for data management]
- **Resource Constraints**: [Time, budget, or skill limitations]

Let's create a comprehensive data quality assessment that ensures your analysis is built on a foundation of reliable, trustworthy data!
```

## Usage Tips
- Start with business-critical data fields and expand from there
- Automate quality checks where possible for ongoing monitoring
- Document quality issues and improvement actions for accountability
- Involve business stakeholders in defining quality requirements
- Establish regular quality review processes to maintain improvements

## Example Usage

"I need help assessing data quality for our customer database that feeds our analytics dashboard. We have 500k customer records from our CRM, e-commerce platform, and support system. Main concerns: duplicate customers across systems, missing contact information affecting marketing campaigns, and inconsistent customer categorization. Need to identify issues, prioritize fixes, and set up ongoing monitoring. Results will inform customer segmentation analysis and marketing automation setup."