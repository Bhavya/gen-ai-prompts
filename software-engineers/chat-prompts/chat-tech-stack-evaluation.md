# Tech Stack Evaluation - Chat Prompt

## Purpose
Systematically evaluate and compare technology stacks for new projects or migration decisions, considering technical, business, and team factors.

## Chat Prompt

```
I need help evaluating different technology stack options for my project. Let's systematically compare the alternatives considering technical requirements, team capabilities, and business constraints to make an informed decision.

## Project Context:
- **Project Type**: [New greenfield project, migration, major feature, etc.]
- **Project Scale**: [Small prototype, medium application, large enterprise system]
- **Timeline**: [Development timeline and key milestones]
- **Budget**: [Development budget and operational cost considerations]
- **Business Criticality**: [How critical is this system to business operations?]

## Requirements Analysis:

### Functional Requirements:
[What does the system need to do?]
- **Core Features**: [Primary functionality]
- **Performance Requirements**: [Response time, throughput, scalability needs]
- **Integration Needs**: [External systems, APIs, data sources]
- **User Experience**: [Web, mobile, desktop, API-only]

### Non-Functional Requirements:
- **Scalability**: [Expected growth in users, data, transactions]
- **Availability**: [Uptime requirements, disaster recovery needs]
- **Security**: [Data sensitivity, compliance requirements]
- **Maintainability**: [Long-term maintenance and evolution needs]
- **Portability**: [Cloud provider flexibility, deployment options]

## Team & Organizational Context:

### Current Team Skills:
[What technologies does your team already know?]
- **Programming Languages**: [Current expertise levels]
- **Frameworks**: [Experience with different frameworks]
- **Infrastructure**: [DevOps, cloud, database experience]
- **Learning Capacity**: [Time available for learning new technologies]

### Organizational Factors:
- **Existing Tech Stack**: [What's already in use in your organization?]
- **Technical Standards**: [Any technology preferences or restrictions?]
- **Support Resources**: [Available internal expertise or external support]
- **Hiring Considerations**: [Ease of finding developers for different technologies]

## Technology Stack Options:

### Option 1: [Name your first option]
**Components:**
- **Frontend**: [Technology choice]
- **Backend**: [Framework/language]
- **Database**: [Database technology]
- **Infrastructure**: [Cloud/hosting approach]
- **Additional Tools**: [Monitoring, CI/CD, etc.]

**Reasoning**: [Why are you considering this stack?]

### Option 2: [Name your second option]
**Components:**
- **Frontend**: [Technology choice]
- **Backend**: [Framework/language]
- **Database**: [Database technology]
- **Infrastructure**: [Cloud/hosting approach]
- **Additional Tools**: [Monitoring, CI/CD, etc.]

**Reasoning**: [Why are you considering this stack?]

### Option 3: [Additional options if relevant]
[Continue with additional stack options...]

## Evaluation Criteria:

### Technical Factors:
- **Performance**: How well will each stack handle your performance requirements?
- **Scalability**: Which stack scales best for your growth projections?
- **Security**: What are the security implications of each choice?
- **Ecosystem**: How mature and well-supported is each technology?
- **Integration**: How well does each stack integrate with existing systems?

### Development Factors:
- **Productivity**: Which stack will allow fastest development?
- **Code Quality**: Which promotes better code organization and maintainability?
- **Testing**: How well does each stack support testing practices?
- **Debugging**: How easy is it to troubleshoot issues in each stack?
- **Documentation**: Quality of documentation and learning resources?

### Operational Factors:
- **Deployment**: How complex is deployment and operations for each stack?
- **Monitoring**: What monitoring and observability options are available?
- **Maintenance**: Long-term maintenance requirements and ease?
- **Cost**: Development cost, operational cost, licensing costs?
- **Vendor Lock-in**: How much flexibility do you maintain with each choice?

### Team & Business Factors:
- **Learning Curve**: How quickly can your team become productive?
- **Hiring**: How easy is it to find developers for each technology?
- **Community**: Strength of community support and resources?
- **Future-Proofing**: How likely is the technology to remain relevant?
- **Risk**: What are the risks associated with each choice?

## Specific Concerns:
[Any particular aspects you're unsure about or want to focus on?]
- Performance bottlenecks
- Scalability challenges
- Security considerations
- Team adoption challenges
- Integration complexity
- Long-term maintenance

## Decision Framework:
Please help me:

1. **Comparative Analysis**: Detailed comparison of each stack across all criteria
2. **Scoring Matrix**: Weighted evaluation based on my priorities
3. **Risk Assessment**: Identify and evaluate risks for each option
4. **Recommendation**: Which stack best fits my situation and why?
5. **Implementation Plan**: How to get started with the recommended stack
6. **Mitigation Strategies**: How to address any downsides of the chosen stack

## Success Metrics:
[How will you measure if the technology choice was successful?]
- Development velocity
- System performance
- Team satisfaction
- Operational efficiency
- Business outcomes

Let's make a data-driven decision that sets this project up for long-term success!
```

## Usage Tips
- Be honest about your team's current skill levels and learning capacity
- Include specific performance and scalability requirements with numbers
- Consider both short-term development needs and long-term maintenance
- Factor in your organization's existing technology investments
- Think about hiring and team growth implications

## Example Usage

"I need help evaluating tech stacks for a new customer analytics platform. We expect 50k daily active users, processing 1M events/day, with real-time dashboards and batch reporting. Team has strong Python/Django experience but limited with modern frontend frameworks. Considering: 1) Python/Django + React + PostgreSQL, 2) Node.js + Vue.js + MongoDB, 3) Java Spring + Angular + PostgreSQL. Main concerns are real-time performance requirements and team's ability to deliver quickly while maintaining code quality."