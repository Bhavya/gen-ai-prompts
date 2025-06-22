# A/B Test Analysis - Chat Prompt

## Purpose
A comprehensive approach to analyzing A/B tests, determining statistical significance, and drawing actionable conclusions from experimental data.

## Chat Prompt

```
I need help analyzing an A/B test to determine if we have a statistically significant result and what actionable conclusions we can draw. Let's work through this analysis systematically to ensure we make the right business decision.

## Experiment Overview:
- **Test Name/Hypothesis**: [What are you testing and what do you expect to happen?]
- **Primary Metric**: [Main success metric you're measuring]
- **Secondary Metrics**: [Additional metrics you're tracking]
- **Test Duration**: [How long has the test been running?]
- **Traffic Split**: [What percentage of users see each variant?]

## Experimental Design:
- **Control Group (A)**: [Description of the control experience]
- **Treatment Group (B)**: [Description of the test variation]
- **Randomization Method**: [How were users assigned to groups?]
- **Sample Size Planning**: [Was there pre-test power analysis done?]

## Current Results:
[Please share your current data - can be raw numbers or summary statistics]

### Control Group (A):
- **Users**: [Number of users in control]
- **Primary Metric Value**: [Conversion rate, average value, etc.]
- **Secondary Metrics**: [Other important measurements]

### Treatment Group (B):
- **Users**: [Number of users in treatment]
- **Primary Metric Value**: [Conversion rate, average value, etc.]
- **Secondary Metrics**: [Other important measurements]

## Analysis Requirements:

### 1. Statistical Significance Testing
- **Hypothesis Testing**: Proper null and alternative hypothesis setup
- **Statistical Test Selection**: Choose appropriate test (t-test, chi-square, etc.)
- **Significance Level**: Determine p-value and confidence intervals
- **Effect Size**: Calculate practical significance and magnitude of difference
- **Power Analysis**: Assess if we have sufficient sample size

### 2. Data Quality Assessment
- **Sample Ratio Mismatch**: Verify traffic split is as expected
- **Bias Detection**: Check for selection bias or confounding factors
- **Novelty Effects**: Consider if results might be influenced by newness
- **Seasonal Patterns**: Account for any time-based effects

### 3. Business Impact Analysis
- **Practical Significance**: Is the difference meaningful for business?
- **Confidence Intervals**: What's the range of likely true effects?
- **Risk Assessment**: What's the downside if we're wrong?
- **Implementation Considerations**: Cost/complexity of rolling out changes

### 4. Recommendations
- **Decision Framework**: Ship, iterate, or abandon based on results
- **Next Steps**: Follow-up tests or analysis needed
- **Monitoring Plan**: What to watch after implementation
- **Learning Documentation**: Key insights for future tests

## Additional Context:
- **Business Constraints**: [Budget, timeline, technical limitations]
- **Risk Tolerance**: [How conservative vs. aggressive should we be?]
- **Historical Context**: [How does this compare to previous tests?]
- **Stakeholder Needs**: [Who needs to approve this decision?]

## Specific Questions:
[Any particular aspects of the analysis you want to focus on or concerns you have]

Let's analyze this data thoroughly to make a confident, data-driven decision about whether to implement this change.
```

## Usage Tips
- Provide raw data or detailed summary statistics when possible
- Be clear about your business context and decision timeline
- Mention any external factors that might have influenced results
- Include information about your technical implementation
- Share your confidence level requirements for making decisions

## Key Analysis Components
- **Statistical significance testing**
- **Effect size calculation**
- **Confidence interval estimation**
- **Power analysis validation**
- **Multiple comparison adjustments (if testing multiple metrics)**
- **Segmentation analysis (if relevant)**

## Common Test Types Covered
- Conversion rate tests (proportions)
- Revenue/value tests (continuous metrics)
- Engagement tests (counts, time-based metrics)
- Multi-variant tests (more than 2 groups)
- Sequential tests (ongoing monitoring)

## Example Usage

"I need help analyzing an A/B test on our checkout page. We tested a simplified checkout flow vs. our current 3-step process.

Hypothesis: Simplified checkout will increase conversion rate
Primary metric: Checkout completion rate
Test duration: 3 weeks

Results so far:
Control (3-step): 2,847 users, 18.2% conversion rate
Treatment (simplified): 2,901 users, 21.7% conversion rate

Secondary metrics show reduced cart abandonment but slightly lower average order value. Need to determine if this is significant enough to implement and what the business impact would be."