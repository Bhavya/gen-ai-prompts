# Security Review - Chat Prompt

## Purpose
Conduct a comprehensive security assessment of your application to identify vulnerabilities and implement appropriate security measures.

## Chat Prompt

```
I need help conducting a thorough security review of my application to identify vulnerabilities and implement appropriate security measures. Let's systematically assess the security posture and create an improvement plan.

## Application Context:
- **Application Type**: [Web app, API, mobile app, desktop app, etc.]
- **Technology Stack**: [Languages, frameworks, databases, cloud services]
- **User Base**: [Internal users, external customers, public-facing]
- **Data Sensitivity**: [Personal data, financial data, healthcare, etc.]
- **Compliance Requirements**: [GDPR, HIPAA, PCI-DSS, SOC 2, etc.]

## Current Security State:
### Existing Security Measures:
[What security measures are currently in place?]
- **Authentication**: [Method used for user authentication]
- **Authorization**: [Role-based access, permissions system]
- **Data Protection**: [Encryption, hashing, secure storage]
- **Network Security**: [HTTPS, firewalls, VPN]
- **Monitoring**: [Logging, alerting, intrusion detection]

### Known Concerns:
[Any security issues you're already aware of or worried about?]
- Previous security incidents
- Audit findings
- Compliance gaps
- Developer security knowledge gaps

## Security Assessment Areas:

### 1. Authentication & Authorization
- **User Authentication**: How secure is the login process?
- **Session Management**: Are sessions handled securely?
- **Password Policies**: Are password requirements adequate?
- **Multi-Factor Authentication**: Should MFA be implemented?
- **Access Controls**: Are permissions properly enforced?
- **Privilege Escalation**: Can users access unauthorized resources?

### 2. Data Protection
- **Data at Rest**: How is stored data protected?
- **Data in Transit**: Is all communication encrypted?
- **Sensitive Data Handling**: Are passwords, tokens, PII properly secured?
- **Data Backup**: Are backups secure and recoverable?
- **Data Retention**: Is data retention policy secure and compliant?

### 3. Input Validation & Injection Protection
- **SQL Injection**: Are database queries parameterized?
- **Cross-Site Scripting (XSS)**: Is user input properly sanitized?
- **Command Injection**: Are system commands safely executed?
- **File Upload Security**: Are file uploads properly validated?
- **API Input Validation**: Are API inputs thoroughly validated?

### 4. Application Security
- **Cross-Site Request Forgery (CSRF)**: Are CSRF tokens implemented?
- **Security Headers**: Are appropriate HTTP security headers set?
- **Error Handling**: Do error messages leak sensitive information?
- **Logging**: Are security events properly logged?
- **Third-Party Dependencies**: Are dependencies regularly updated for security?

### 5. Infrastructure Security
- **Server Hardening**: Are servers properly configured and patched?
- **Network Segmentation**: Is network access properly restricted?
- **Container Security**: Are containers and images secure?
- **Cloud Security**: Are cloud services properly configured?
- **Secrets Management**: How are API keys and secrets stored?

### 6. DevOps Security
- **Secure CI/CD**: Are build and deploy pipelines secure?
- **Code Repository**: Is source code access properly controlled?
- **Environment Security**: Are dev/staging environments secure?
- **Deployment Security**: Are deployments secure and auditable?

## Threat Modeling:
### Potential Attackers:
[Who might want to attack your system?]
- Opportunistic attackers
- Competitors
- Insider threats
- Nation-state actors
- Hacktivists

### Valuable Assets:
[What would attackers want to access?]
- User data
- Financial information
- Business intelligence
- System access
- Reputation damage

### Attack Vectors:
[How might attackers try to compromise your system?]
- Web application vulnerabilities
- Social engineering
- Physical access
- Supply chain attacks
- Insider threats

## Compliance & Regulatory:
### Applicable Regulations:
[What regulations must you comply with?]
- GDPR (EU data protection)
- CCPA (California privacy)
- HIPAA (healthcare)
- PCI-DSS (payment processing)
- SOX (financial)
- Industry-specific regulations

### Audit Requirements:
[Any upcoming audits or assessments?]

## Code & Architecture Review:
[If possible, share relevant code snippets or architecture details]

```
[Example: Authentication code, database queries, API endpoints]
```

## Specific Security Questions:
1. **Vulnerability Assessment**: What are the most critical security risks?
2. **Compliance Gaps**: What's needed to meet regulatory requirements?
3. **Implementation Priority**: Which security improvements should be tackled first?
4. **Best Practices**: What security practices should be standard for our team?
5. **Monitoring**: What security monitoring should be implemented?
6. **Incident Response**: How should we prepare for security incidents?

Please help me:
- **Identify Vulnerabilities**: Point out specific security weaknesses
- **Prioritize Fixes**: Rank security improvements by risk and impact
- **Implementation Guidance**: Provide specific steps to improve security
- **Best Practices**: Recommend security standards for ongoing development
- **Compliance Mapping**: Ensure we meet relevant regulatory requirements
- **Monitoring Strategy**: Set up appropriate security monitoring and alerting

Let's build a security-first application that protects user data and business assets!
```

## Usage Tips
- Be specific about the types of data your application handles
- Share relevant code snippets (anonymized if necessary)
- Mention any previous security incidents or concerns
- Include information about your team's security experience
- Describe your compliance requirements and audit timeline

## Example Usage

"I need help conducting a security review of our customer portal web application. It's a React/Node.js app with PostgreSQL database, handling customer PII and payment information. Currently using JWT authentication, bcrypt for passwords, and HTTPS everywhere. Main concerns are potential SQL injection in our reporting queries and whether our session management is secure enough for PCI compliance. Team has limited security experience and we have a compliance audit in 6 months."