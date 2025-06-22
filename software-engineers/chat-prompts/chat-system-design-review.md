# System Design Review - Chat Prompt

## Purpose
Get comprehensive feedback on system architecture and design decisions for scalable, maintainable software systems.

## Chat Prompt

```
I need help reviewing a system design to ensure it's scalable, maintainable, and follows best practices. Let's work through the architecture systematically to identify potential issues and improvements.

## System Overview:
- **System Purpose**: [What problem does this system solve?]
- **Scale Requirements**: [Expected users, requests/second, data volume]
- **Performance Requirements**: [Response time, availability, throughput expectations]
- **Budget/Resource Constraints**: [Infrastructure budget, team size, timeline]

## Current Architecture:

### High-Level Components:
[Describe the main components and their responsibilities]
- **Frontend**: [Technology stack, responsibilities]
- **Backend Services**: [Microservices, APIs, business logic]
- **Database Layer**: [Database choices, data models]
- **Infrastructure**: [Cloud provider, deployment strategy]
- **External Dependencies**: [Third-party services, APIs]

### Data Flow:
[Describe how data moves through your system]
1. [User action/request]
2. [Processing steps]
3. [Data storage/retrieval]
4. [Response/output]

### Technology Stack:
- **Languages**: [Programming languages used]
- **Frameworks**: [Web frameworks, libraries]
- **Databases**: [SQL/NoSQL choices and why]
- **Infrastructure**: [Cloud services, containers, orchestration]
- **Monitoring**: [Logging, metrics, alerting]

## Specific Areas for Review:

### Scalability Concerns:
- **Horizontal Scaling**: How will this handle increased load?
- **Database Scaling**: Sharding, replication, or partitioning strategies
- **Bottlenecks**: Where are the likely performance constraints?
- **Caching Strategy**: What and where to cache for optimal performance

### Reliability & Availability:
- **Failure Modes**: What happens when components fail?
- **Redundancy**: How is high availability achieved?
- **Data Consistency**: How do you handle distributed data consistency?
- **Disaster Recovery**: Backup and recovery strategies

### Security Architecture:
- **Authentication/Authorization**: How are users and services authenticated?
- **Data Protection**: Encryption at rest and in transit
- **Network Security**: Firewalls, VPNs, network segmentation
- **Compliance**: Any regulatory requirements (GDPR, HIPAA, etc.)

### Maintainability:
- **Code Organization**: Service boundaries and separation of concerns
- **Testing Strategy**: Unit, integration, and end-to-end testing
- **Deployment Pipeline**: CI/CD, rollback strategies
- **Monitoring/Observability**: How do you track system health?

## Current Challenges:
[Any specific problems you're already aware of or concerned about]

## Questions for Review:
1. **Architecture Soundness**: Are the component boundaries and responsibilities well-defined?
2. **Scalability Assessment**: Will this architecture handle expected growth?
3. **Technology Choices**: Are the technology decisions appropriate for the use case?
4. **Risk Identification**: What are the biggest risks and how can they be mitigated?
5. **Best Practices**: What industry standards or patterns should be applied?
6. **Future Evolution**: How easily can this system evolve as requirements change?

Please provide:
- **Strengths**: What's working well in this design
- **Concerns**: Potential issues or areas of risk
- **Recommendations**: Specific improvements or alternatives
- **Implementation Priority**: Which changes should be tackled first

Let's ensure this system will be robust, scalable, and maintainable for the long term.
```

## Usage Tips
- Include architecture diagrams or sketches if possible
- Be specific about scale requirements and constraints
- Mention any compliance or regulatory requirements
- Share information about your team's expertise and preferences
- Include context about existing systems this needs to integrate with

## Example Usage

"I need help reviewing the system design for our new e-commerce platform. We expect 10k daily active users initially, growing to 100k+ within 2 years. Current design uses React frontend, Node.js microservices, PostgreSQL for transactions, Redis for caching, and AWS infrastructure. Main concerns are handling flash sales traffic spikes and ensuring PCI compliance for payments."