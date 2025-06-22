# Dashboard Requirements - Chat Prompt

## Purpose
A structured approach to gathering requirements and designing effective dashboards that meet stakeholder needs and drive actionable insights.

## Chat Prompt

```
I need to design a dashboard and want to make sure I gather comprehensive requirements before building it. Let's work through a systematic requirements gathering process to create a dashboard that truly serves its intended users and business purpose.

## Dashboard Context:
- **Dashboard Purpose**: [What business problem is this dashboard solving?]
- **Primary Users**: [Who will be using this dashboard most frequently?]
- **Secondary Users**: [Who else might access it occasionally?]
- **Business Domain**: [Sales, marketing, operations, finance, product, etc.]
- **Decision Context**: [What decisions will this dashboard inform?]

## User Analysis:
### Primary Stakeholders:
- **Role/Title**: [Job title and department]
- **Technical Skill Level**: [Non-technical, somewhat technical, very technical]
- **Current Pain Points**: [What challenges are they facing with existing reporting?]
- **Success Criteria**: [How will they measure if this dashboard is successful?]
- **Usage Pattern**: [Daily check-ins, weekly reviews, ad-hoc analysis, etc.]

## Requirements Gathering:

### 1. Business Objectives
- **Key Questions**: What are the top 3-5 questions this dashboard needs to answer?
- **Success Metrics**: What KPIs and metrics are most critical to track?
- **Alert Thresholds**: What values should trigger attention or action?
- **Benchmarking**: What comparisons are important (time periods, targets, competitors)?

### 2. Data Requirements
- **Data Sources**: [What systems/databases contain the needed data?]
- **Data Refresh**: [How often does the data need to be updated?]
- **Historical Range**: [How far back in time do users need to see?]
- **Data Granularity**: [Daily, weekly, monthly aggregation levels needed?]
- **Data Quality**: [Any known issues with data accuracy or completeness?]

### 3. Functional Requirements
- **Key Metrics**: [List the specific metrics/KPIs to display]
- **Filtering Needs**: [What dimensions do users need to filter by?]
- **Drill-Down Capabilities**: [What level of detail exploration is needed?]
- **Export Requirements**: [Do users need to export data or images?]
- **Mobile Access**: [Will this be viewed on mobile devices?]

### 4. Visual Design Preferences
- **Layout Style**: [Executive summary, operational monitoring, analytical exploration]
- **Chart Types**: [Any preferences for specific visualization types?]
- **Color Schemes**: [Brand colors, accessibility considerations]
- **Information Density**: [High-level overview vs. detailed metrics]

### 5. Technical Constraints
- **Platform**: [Tableau, Power BI, custom development, etc.]
- **Performance**: [Expected number of concurrent users, response time requirements]
- **Security**: [Who should have access? Any data sensitivity concerns?]
- **Integration**: [Need to embed in other applications?]

## Current State Assessment:
- **Existing Solutions**: [What reports/dashboards already exist for this area?]
- **Current Gaps**: [What's missing from existing solutions?]
- **User Feedback**: [Any specific complaints or requests from current tools?]

## Sample Questions for Stakeholder Interviews:
Please help me formulate the right questions to ask stakeholders:

1. **Strategic Questions**: [About high-level goals and success criteria]
2. **Tactical Questions**: [About daily usage and specific needs]
3. **Technical Questions**: [About data access and system constraints]
4. **Design Questions**: [About visualization preferences and usability]

## Deliverables Planning:
- **Timeline**: [When does this need to be completed?]
- **Review Process**: [How will stakeholders provide feedback during development?]
- **Training Needs**: [Will users need training on the new dashboard?]
- **Maintenance**: [Who will maintain and update the dashboard ongoing?]

Based on this information, please help me:
1. **Prioritize Requirements**: Which features are must-have vs. nice-to-have
2. **Design Recommendations**: Suggest optimal layout and visualization approaches
3. **Implementation Plan**: Recommend development phases and timeline
4. **Success Metrics**: Define how we'll measure dashboard effectiveness
5. **Risk Mitigation**: Identify potential challenges and mitigation strategies

Let's ensure this dashboard will actually be used and drive the business value we're aiming for.
```

## Usage Tips
- Interview multiple stakeholders to get diverse perspectives
- Ask for specific examples of decisions they need to make
- Understand their current workflow and where the dashboard fits
- Validate requirements with actual data samples when possible
- Consider both immediate needs and future evolution

## Key Requirements Categories
- **Business Requirements**: Goals, success criteria, decision context
- **Functional Requirements**: Features, capabilities, interactions
- **Data Requirements**: Sources, refresh rates, historical needs
- **Technical Requirements**: Platform, performance, security
- **Design Requirements**: Layout, visualizations, user experience

## Example Usage

"I need to design a sales performance dashboard for our regional sales managers. The primary users are 8 regional managers who currently get weekly Excel reports but want real-time visibility.

Business context: We're trying to improve sales forecasting accuracy and help managers identify at-risk deals earlier. Current pain points include stale data, difficulty comparing regions, and no visibility into pipeline health.

Users are moderately technical, familiar with basic dashboards but not advanced analytics. They need daily visibility but detailed weekly reviews. Platform is Tableau with data from Salesforce CRM.

Key questions: Which deals are at risk? How are we tracking against quotas? Which reps need support?"