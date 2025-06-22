# Performance Optimization - Chat Prompt

## Purpose
Systematic approach to identifying and resolving performance bottlenecks in applications.

## Chat Prompt

```
I need help optimizing the performance of my application. Let's work through this systematically to identify bottlenecks and implement improvements.

## Application Context:
- **Type**: [Web app/API/mobile app/desktop app/etc.]
- **Technology Stack**: [Languages, frameworks, databases, infrastructure]
- **Scale**: [Users, requests per second, data volume, etc.]
- **Performance Issues**: [Specific symptoms: slow load times, high CPU, memory leaks, etc.]

## Current Performance Metrics:
[Share any metrics you have:]
- Response times
- Resource usage (CPU, memory, disk I/O)
- Database query performance
- Error rates
- User experience metrics

## Areas of Concern:
[Check all that apply or add others:]
- [ ] Page/screen load times
- [ ] Database query performance
- [ ] API response times
- [ ] Memory usage/leaks
- [ ] CPU utilization
- [ ] Network requests
- [ ] File I/O operations
- [ ] Third-party service calls

Please help me:

1. **Performance Audit**: Analyze current performance characteristics and identify the most impactful bottlenecks
2. **Measurement Strategy**: Recommend tools and metrics to properly measure performance
3. **Optimization Plan**: Prioritized list of improvements based on impact vs effort
4. **Implementation Guidance**: Specific techniques and code changes for the highest-priority optimizations
5. **Monitoring Setup**: How to track performance improvements and catch regressions

## Code/Configuration Samples:
[Share relevant code snippets, database schemas, or configuration that might be performance-critical]

Let's start by understanding the biggest performance bottlenecks and create a data-driven optimization plan.
```

## Usage Tips
- Include actual performance metrics when possible (response times, memory usage, etc.)
- Share profiling data or performance monitoring screenshots
- Mention your performance targets/requirements
- Describe user-facing symptoms (slow pages, timeouts, etc.)
- Include information about traffic patterns and peak usage

## Common Optimization Areas to Discuss
- Database indexing and query optimization
- Caching strategies (application, database, CDN)
- Code-level optimizations (algorithms, data structures)
- Network optimization (compression, bundling, CDN)
- Resource management (connection pooling, memory management)
- Asynchronous processing and parallelization

## Example Usage

"I need help optimizing the performance of my application. It's a React web app with a Node.js/Express API and PostgreSQL database, serving about 10,000 daily active users. 

Performance issues: Our dashboard page is taking 8-12 seconds to load, and users are complaining. API responses are averaging 2-3 seconds.

Current metrics: Database queries taking 1-5 seconds each, bundle size is 2.5MB, API endpoints averaging 2000ms response time.

Areas of concern: Database query performance, large JavaScript bundle, multiple API calls on page load."