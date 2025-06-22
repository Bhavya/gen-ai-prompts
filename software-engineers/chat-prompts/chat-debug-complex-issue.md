# Debug Complex Issue - Chat Prompt

## Purpose
A structured approach to debugging complex technical issues with systematic problem-solving.

## Chat Prompt

```
I need help debugging a complex issue in my application. Please help me work through this systematically.

## Issue Description:
[Describe the problem you're experiencing]

## Current Behavior:
[What is actually happening]

## Expected Behavior:
[What should be happening instead]

## Environment:
- Technology stack: [Your tech stack]
- Environment: [Development/staging/production]
- Recent changes: [Any recent code changes, deployments, or configuration updates]

## What I've Already Tried:
[List debugging steps you've already taken]

Please help me:
1. **Analyze the symptoms** - What might be causing this behavior?
2. **Generate hypotheses** - What are the most likely root causes?
3. **Design experiments** - What specific tests can we run to isolate the issue?
4. **Create a debugging plan** - Step-by-step approach to identify and fix the problem
5. **Prevent recurrence** - How can we avoid this issue in the future?

Please ask clarifying questions to better understand the issue, and let's work through this methodically.
```

## Usage Tips
- Be as specific as possible about symptoms and error messages
- Include relevant code snippets, logs, or stack traces
- Mention any patterns you've noticed (timing, frequency, conditions)
- Share what debugging tools you have available

## Follow-up Questions to Expect
- Can you reproduce the issue consistently?
- What logging/monitoring data do you have access to?
- Have you checked for resource constraints (memory, CPU, disk, network)?
- Are there any error messages in logs or browser console?
- When did this issue first appear?

## Example Usage

"I need help debugging a complex issue in my application. My Node.js API is intermittently returning 500 errors, but only during high traffic periods. The current behavior is that about 5% of requests fail with 'Database connection timeout' errors. Expected behavior is that all requests should complete successfully or fail gracefully. 

Environment: Node.js with Express, PostgreSQL database, running on AWS ECS. Recent changes: We upgraded from PostgreSQL 12 to 14 last week.

What I've already tried: Increased connection pool size, added retry logic, checked database logs (no obvious issues), monitored CPU/memory (within normal ranges)."