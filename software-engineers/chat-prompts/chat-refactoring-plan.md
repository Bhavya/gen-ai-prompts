# Refactoring Plan - Chat Prompt

## Purpose
Create a systematic plan for refactoring legacy code or improving existing codebase structure while minimizing risk and maintaining functionality.

## Chat Prompt

```
I need help creating a systematic refactoring plan for improving our codebase. Let's develop a safe, incremental approach that improves code quality while minimizing risk and maintaining system functionality.

## Codebase Context:
- **Technology Stack**: [Languages, frameworks, libraries being used]
- **Codebase Size**: [Lines of code, number of files, modules]
- **Age & History**: [How old is the code? Major changes over time?]
- **Team Familiarity**: [How well does the current team know this code?]
- **Business Criticality**: [How mission-critical is this system?]

## Current State Assessment:
### Code Quality Issues:
[What specific problems are you seeing?]
- [ ] Code duplication
- [ ] Large, complex functions/classes
- [ ] Tight coupling between components
- [ ] Inconsistent naming and style
- [ ] Poor error handling
- [ ] Missing or outdated documentation
- [ ] Performance bottlenecks
- [ ] Security vulnerabilities
- [ ] Difficult to test code
- [ ] Technical debt from quick fixes

### Pain Points:
- **Development Velocity**: [How do code issues slow down development?]
- **Bug Frequency**: [Are code quality issues causing bugs?]
- **Onboarding Difficulty**: [Hard for new developers to understand?]
- **Testing Challenges**: [Is the code difficult to test?]
- **Deployment Risks**: [Are deployments risky due to code complexity?]

## Refactoring Goals:
### Primary Objectives:
[What are your main goals? Rank by importance]
- [ ] Improve code readability and maintainability
- [ ] Reduce technical debt
- [ ] Improve performance
- [ ] Better error handling and logging
- [ ] Increase test coverage
- [ ] Simplify deployment process
- [ ] Better separation of concerns
- [ ] Modernize technology stack

### Success Metrics:
- **Quality Metrics**: [How will you measure improvement?]
- **Performance Targets**: [Any specific performance goals?]
- **Developer Experience**: [How should this improve development?]

## Constraints & Requirements:
- **Timeline**: [When does this need to be completed?]
- **Resource Allocation**: [How much development time is available?]
- **Business Continuity**: [System availability requirements during refactoring]
- **Budget**: [Any budget constraints for tooling or infrastructure?]
- **Risk Tolerance**: [How conservative should the approach be?]

## Code Areas for Refactoring:
### High-Priority Areas:
[Which parts of the code need the most attention?]
1. **Area 1**: [e.g., User authentication module]
   - **Issues**: [Specific problems]
   - **Impact**: [Effect on system/development]
   
2. **Area 2**: [e.g., Database access layer]
   - **Issues**: [Specific problems]
   - **Impact**: [Effect on system/development]

### Dependencies & Interactions:
[How do these areas interact with each other and the rest of the system?]

## Refactoring Strategy Planning:

### 1. Risk Assessment & Mitigation
- **High-Risk Areas**: Which refactoring changes pose the most risk?
- **Safety Measures**: What safeguards should be in place?
- **Rollback Plans**: How to quickly revert if issues arise?
- **Testing Strategy**: What tests are needed before/during/after refactoring?

### 2. Incremental Approach
- **Phase Planning**: How to break refactoring into manageable phases?
- **Delivery Strategy**: Continuous deployment vs. big-bang releases?
- **Feature Flags**: Should feature toggles be used during refactoring?
- **Backward Compatibility**: What compatibility needs to be maintained?

### 3. Team Coordination
- **Code Freeze Periods**: Any times when code changes should be limited?
- **Review Process**: How should refactored code be reviewed?
- **Knowledge Sharing**: How to ensure team understands changes?
- **Documentation Updates**: What documentation needs updating?

### 4. Monitoring & Validation
- **Performance Monitoring**: How to track system performance during changes?
- **Error Monitoring**: How to catch issues introduced by refactoring?
- **User Impact**: How to monitor user-facing effects?
- **Success Validation**: How to confirm refactoring goals are met?

## Code Samples:
[If possible, share examples of problematic code areas]

```
[Example of code that needs refactoring]
```

## Specific Questions:
1. **Prioritization**: Which areas should be tackled first and why?
2. **Approach**: What refactoring techniques are most appropriate?
3. **Risk Management**: How to minimize disruption during refactoring?
4. **Testing**: What testing approach ensures safe refactoring?
5. **Timeline**: What's a realistic timeline for this refactoring effort?

Please help me create a refactoring plan that:
- **Minimizes Risk** while making meaningful improvements
- **Provides Clear Steps** that the team can follow systematically
- **Maintains System Stability** throughout the refactoring process
- **Delivers Measurable Value** in terms of code quality and developer productivity
- **Fits Within Constraints** of time, resources, and business requirements

Let's turn this legacy code into something the team can be proud to work with!
```

## Usage Tips
- Share specific examples of problematic code when possible
- Be realistic about time and resource constraints
- Include information about your current testing coverage
- Mention any upcoming features or deadlines that might affect timing
- Consider both technical and business priorities when planning

## Example Usage

"I need help creating a refactoring plan for our 3-year-old Node.js API that's become difficult to maintain. The main issues are a 2000-line controller file, no separation between business logic and data access, and inconsistent error handling. We have 60% test coverage but tests are slow and brittle. Team of 4 developers, need to maintain 99.9% uptime, and have a major feature launch in 3 months. Want to improve maintainability without disrupting the roadmap."