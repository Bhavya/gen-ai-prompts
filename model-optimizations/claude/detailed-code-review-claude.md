# Detailed Code Review - Claude Optimized

## Purpose
A comprehensive code review prompt optimized for Claude's analytical strengths and structured reasoning approach.

## Claude-Optimized Prompt

```
I need you to conduct a thorough, structured code review. Please analyze the provided code with your characteristic attention to detail and systematic approach.

## Review Framework

Please organize your review using this structured approach:

### 1. Initial Assessment
- **Code Purpose**: What is this code intended to accomplish?
- **Overall Architecture**: How well does the structure support the intended functionality?
- **First Impressions**: What stands out immediately (positive or concerning)?

### 2. Detailed Analysis

#### Security Considerations
- Input validation and sanitization
- Authentication and authorization checks
- Data exposure risks
- Potential vulnerabilities (SQL injection, XSS, etc.)
- Error handling that doesn't leak sensitive information

#### Code Quality & Maintainability
- Readability and clarity of intent
- Naming conventions and consistency
- Code organization and modularity
- Documentation and comments quality
- Adherence to established patterns

#### Performance & Efficiency
- Algorithm complexity analysis
- Resource usage considerations
- Database query optimization opportunities
- Caching strategies
- Potential bottlenecks

#### Best Practices Adherence
- Language-specific idioms and conventions
- Design patterns application
- SOLID principles compliance
- Error handling strategies
- Testing implications

### 3. Risk Assessment
- **Critical Issues**: Must-fix problems (security, bugs, breaking changes)
- **Major Concerns**: Significant issues affecting maintainability or performance
- **Minor Issues**: Style inconsistencies and minor improvements
- **Future Considerations**: Potential issues as the codebase scales

### 4. Constructive Recommendations
For each issue identified:
- **Why it matters**: Explain the reasoning behind the concern
- **Specific suggestion**: Provide actionable improvement recommendations
- **Alternative approaches**: When applicable, suggest multiple solutions
- **Priority level**: Help prioritize fixes based on impact and effort

### 5. Positive Recognition
- Well-implemented patterns or solutions
- Good practices that should be maintained
- Areas where the code demonstrates quality craftsmanship

## Code to Review:
[Paste your code here]

## Additional Context:
- **Project Type**: [Web app, API, library, etc.]
- **Technology Stack**: [Languages, frameworks, databases]
- **Team Context**: [Team size, experience levels, coding standards]
- **Specific Concerns**: [Any particular areas you'd like me to focus on]

Please provide your analysis with the thoroughness and structured reasoning that helps teams improve their code quality systematically.
```

## Why This Works Well with Claude

- **Structured Analysis**: Claude excels at systematic, comprehensive reviews
- **Ethical Considerations**: Natural focus on security and best practices
- **Detailed Reasoning**: Provides thorough explanations for recommendations
- **Risk Assessment**: Strong at evaluating potential issues and their implications
- **Balanced Perspective**: Recognizes both problems and positive aspects

## Usage Tips

1. Provide complete code context when possible
2. Mention specific concerns or requirements
3. Include information about team skill levels and project constraints
4. Ask follow-up questions about specific recommendations
5. Request prioritization of issues based on your situation

## Example Output Structure

Claude will typically provide:
- Comprehensive analysis across all requested dimensions
- Clear prioritization of issues
- Detailed explanations of the reasoning behind each recommendation
- Multiple solution approaches when applicable
- Recognition of well-written code sections