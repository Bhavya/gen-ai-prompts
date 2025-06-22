# API Design Guide - Chat Prompt

## Purpose
Design well-structured, developer-friendly APIs that follow REST principles and industry best practices.

## Chat Prompt

```
I need help designing a robust, well-structured API that will be easy for developers to use and maintain. Let's work through the API design systematically to ensure it follows best practices and meets our requirements.

## API Context:
- **API Purpose**: [What functionality will this API provide?]
- **Target Users**: [Internal teams, external developers, mobile apps, web apps]
- **Expected Usage**: [Request volume, frequency patterns, performance requirements]
- **Integration Context**: [Part of microservices, standalone service, legacy system modernization]

## Business Requirements:
### Core Functionality:
[List the main features/operations your API needs to support]
- [Operation 1: e.g., Create user accounts]
- [Operation 2: e.g., Process payments]
- [Operation 3: e.g., Generate reports]

### Data Requirements:
- **Data Types**: [What kinds of data will be exchanged?]
- **Data Volume**: [Size of typical requests/responses]
- **Data Sensitivity**: [Any PII, financial, or sensitive data concerns?]
- **Compliance**: [GDPR, HIPAA, PCI, or other regulatory requirements]

## Technical Constraints:
- **Technology Stack**: [Backend language/framework preferences]
- **Authentication**: [API keys, OAuth, JWT, other requirements]
- **Rate Limiting**: [Usage limits, throttling requirements]
- **Versioning Strategy**: [How will you handle API evolution?]
- **Documentation**: [OpenAPI/Swagger, other documentation needs]

## Design Areas for Guidance:

### 1. API Architecture & Patterns
- **REST vs. GraphQL**: Which approach fits better and why?
- **Resource Modeling**: How to structure endpoints and HTTP methods
- **URL Design**: Naming conventions and hierarchical structure
- **HTTP Status Codes**: Appropriate status codes for different scenarios

### 2. Request/Response Design
- **Data Formats**: JSON structure, field naming conventions
- **Pagination**: How to handle large result sets
- **Filtering & Sorting**: Query parameter design for data retrieval
- **Error Handling**: Consistent error response format and messaging

### 3. Security Design
- **Authentication Strategy**: Best approach for your use case
- **Authorization**: Role-based access, scope limitations
- **Input Validation**: Request validation and sanitization
- **Security Headers**: CORS, rate limiting, other protective measures

### 4. Performance & Scalability
- **Caching Strategy**: Response caching, ETags, cache headers
- **Async Operations**: Handling long-running processes
- **Batch Operations**: Efficient bulk data operations
- **Compression**: Response compression and optimization

### 5. Developer Experience
- **Documentation Strategy**: Interactive docs, code examples
- **SDK Considerations**: Language-specific client libraries
- **Testing Support**: Sandbox environments, test data
- **Error Messages**: Helpful, actionable error responses

## Current API Draft:
[If you have any initial endpoint designs, share them here]

### Sample Endpoints:
```
[Example: GET /api/v1/users/{id}]
[Example: POST /api/v1/orders]
```

### Sample Request/Response:
```json
[Provide examples of your current thinking on data structures]
```

## Specific Questions:
1. **Endpoint Structure**: What's the best way to organize these endpoints?
2. **Data Modeling**: How should the request/response objects be structured?
3. **Error Handling**: What's the best approach for consistent error responses?
4. **Versioning**: How should we handle API evolution over time?
5. **Performance**: What optimizations should we build in from the start?
6. **Security**: What security measures are essential for this use case?

Please help me create an API design that is:
- **Intuitive**: Easy for developers to understand and use
- **Consistent**: Follows predictable patterns throughout
- **Scalable**: Can handle growth in usage and features  
- **Secure**: Protects against common API vulnerabilities
- **Well-Documented**: Clear documentation and examples

Let's design an API that developers will actually enjoy using!
```

## Usage Tips
- Share any existing API standards or style guides your organization follows
- Include examples of APIs you admire or want to emulate
- Be specific about authentication and authorization requirements
- Mention integration requirements with existing systems
- Consider both current needs and future expansion plans

## Example Usage

"I need help designing a REST API for our project management SaaS. The API needs to support CRUD operations for projects, tasks, and team members, plus reporting endpoints. Target users are web/mobile apps and potential third-party integrations. Expected load is 1000 requests/minute initially. Need OAuth2 authentication and role-based permissions (admin, manager, member). Looking for guidance on endpoint structure, error handling, and pagination strategy."