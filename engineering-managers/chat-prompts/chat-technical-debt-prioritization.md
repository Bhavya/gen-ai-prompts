# Technical Debt Prioritization - Chat Prompt

## Purpose
Systematically assess and prioritize technical debt to balance new feature development with maintaining a healthy codebase.

## Chat Prompt

```
I need help prioritizing our technical debt backlog and creating a strategy that balances new feature development with maintaining a healthy, sustainable codebase. Let's develop a systematic approach to technical debt management.

## Codebase Context:
- **Application Type**: [Web app, API, mobile app, distributed system, etc.]
- **Technology Stack**: [Languages, frameworks, infrastructure]
- **Codebase Age**: [How old is the system? Major evolution points?]
- **Team Size**: [Number of developers working on this codebase]
- **Development Velocity**: [Current sprint capacity, delivery frequency]

## Current Technical Debt Inventory:
### Known Issues:
[List the technical debt items you're aware of - be as specific as possible]

**Code Quality Issues:**
- [Example: Legacy authentication module with poor error handling]
- [Example: 2000-line controller class that needs refactoring]
- [Example: Inconsistent API response formats across endpoints]

**Infrastructure/Architecture Issues:**
- [Example: Database performance problems with large tables]
- [Example: Monolithic service that should be split]
- [Example: Outdated deployment process causing release delays]

**Dependencies & Security:**
- [Example: Outdated libraries with known vulnerabilities]
- [Example: Custom-built solutions that could use standard libraries]
- [Example: Missing automated testing in critical paths]

**Process & Tooling:**
- [Example: Manual deployment steps prone to errors]
- [Example: Insufficient monitoring and alerting]
- [Example: Inconsistent code review standards]

## Business Impact Assessment:

### Development Velocity Impact:
- **Feature Development Speed**: How is technical debt slowing down new features?
- **Bug Fix Complexity**: Are bugs taking longer to fix due to code complexity?
- **Onboarding Time**: How does technical debt affect new developer productivity?
- **Testing Efficiency**: Are tests slow, brittle, or insufficient?

### Business Risk Assessment:
- **Production Stability**: Which debt items pose risk to system availability?
- **Security Vulnerabilities**: Any debt items creating security risks?
- **Scalability Limitations**: What prevents the system from scaling?
- **Compliance Issues**: Any debt affecting regulatory compliance?

### Customer Impact:
- **Performance Issues**: Which debt items affect user experience?
- **Feature Limitations**: What prevents delivering customer value?
- **Support Burden**: Which issues create excessive support tickets?

## Prioritization Framework:

### 1. Impact vs. Effort Matrix
For each debt item, help me assess:
- **Business Impact**: (High/Medium/Low) - Effect on users, development speed, business goals
- **Implementation Effort**: (High/Medium/Low) - Time, complexity, risk to implement
- **Risk Level**: (High/Medium/Low) - What happens if we don't address this?
- **Dependencies**: What other work depends on or blocks this item?

### 2. Categorization Strategy
**Must Fix (High Priority):**
- Security vulnerabilities
- Production stability risks
- Major development blockers

**Should Fix (Medium Priority):**
- Performance improvements
- Developer productivity enhancements
- Maintainability improvements

**Nice to Fix (Low Priority):**
- Code style inconsistencies
- Minor refactoring opportunities
- Optimization for edge cases

### 3. Strategic Alignment
- **Roadmap Alignment**: Which debt items support upcoming features?
- **Team Growth**: Which improvements help onboard new team members?
- **Technology Strategy**: Which debt aligns with technology modernization goals?

## Resource Allocation Strategy:

### Development Capacity Planning:
- **Current Sprint Capacity**: [Story points or hours per sprint]
- **Technical Debt Budget**: [What percentage should go to debt vs. features?]
- **Dedicated Time**: [Should there be dedicated debt sprints or ongoing allocation?]
- **Team Member Assignment**: [Who has the right skills for different debt items?]

### Implementation Approaches:
- **Boy Scout Rule**: Small improvements during regular feature work
- **Dedicated Sprints**: Focused technical debt reduction periods
- **Background Tasks**: Debt work during low-activity periods
- **Paired Development**: Debt reduction while building new features

## Stakeholder Communication:

### Executive Communication:
- **Business Case**: How to explain technical debt value to non-technical stakeholders?
- **ROI Demonstration**: How to show return on investment for debt reduction?
- **Risk Communication**: How to convey technical risks in business terms?
- **Timeline Planning**: How to integrate debt work into project timelines?

### Team Communication:
- **Priority Transparency**: How to help team understand prioritization decisions?
- **Progress Tracking**: How to measure and communicate debt reduction progress?
- **Motivation**: How to keep team engaged with debt work alongside feature development?

## Measurement & Tracking:

### Success Metrics:
- **Development Velocity**: Sprint velocity, feature delivery time
- **Code Quality**: Test coverage, code complexity metrics, review feedback
- **System Health**: Performance metrics, error rates, uptime
- **Developer Experience**: Onboarding time, survey feedback, retention

### Progress Tracking:
- **Debt Inventory**: How to maintain and update the technical debt backlog?
- **Completion Tracking**: How to measure progress on debt reduction?
- **Impact Assessment**: How to validate that debt reduction improves outcomes?

## Specific Decisions Needed:

1. **Prioritization**: Which 3-5 debt items should we tackle first?
2. **Resource Allocation**: What percentage of sprint capacity should go to technical debt?
3. **Implementation Strategy**: Should we do dedicated debt sprints or integrate into feature work?
4. **Team Assignment**: Who should lead different categories of debt reduction?
5. **Timeline**: What's a realistic timeline for addressing high-priority debt?
6. **Success Criteria**: How will we know if our debt reduction efforts are successful?

## Constraints & Considerations:
- **Deadline Pressures**: [Any upcoming deadlines affecting prioritization?]
- **Team Skills**: [Are there skill gaps that affect what debt can be tackled?]
- **Budget Constraints**: [Any budget limitations for tools or infrastructure improvements?]
- **Stakeholder Pressure**: [Pressure for new features vs. debt reduction?]

Please help me create a systematic approach to technical debt that:
- **Prioritizes effectively** based on business impact and team capacity
- **Communicates value** to stakeholders in business terms  
- **Integrates smoothly** with feature development work
- **Shows measurable progress** and return on investment
- **Prevents debt accumulation** through improved processes

Let's turn our technical debt from a burden into a manageable, strategic investment in our platform's future!
```

## Usage Tips
- Be specific about technical debt items with concrete examples
- Quantify impact where possible (performance numbers, time costs, bug frequency)
- Consider both immediate pain and long-term strategic goals
- Include information about upcoming features that might be affected
- Balance perfectionism with pragmatic business needs

## Example Usage

"I need help prioritizing technical debt for our 3-year-old Node.js/React e-commerce platform. Main issues: 1) Database queries taking 3-5 seconds on product pages, 2) Monolithic backend service that's hard to scale, 3) Test suite takes 45 minutes to run, 4) Deployment requires 2 hours of manual steps, 5) Legacy payment integration causing 5% transaction failures. Team of 6 developers, currently spending 80% time on features, 20% on bugs/maintenance. Pressure from business to deliver new checkout flow in 8 weeks, but technical debt is slowing everything down."