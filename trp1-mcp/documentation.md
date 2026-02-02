# Documentation

## What you did
- Added comprehensive examples and best practices for agent behavior
- Restructured rules for better clarity and consistency in trigger tool usage
- Defined clear workflow sequences and validation checklists
- Improved MCP performance tracking instructions for AI agent monitoring
- Added a purpose section that will help both the person (that is trying to understand the rules) and ai agent while using the tools

## What worked
- Structured execution sequence with numbered steps makes the workflow clear
- Separate formatting rules for each trigger type (`log_passage_time_trigger` vs `log_performance_outlier_trigger`)
- Pre-response validation checklist ensures compliance
- Common mistakes section helps prevent errors
- Concrete example workflow demonstrates expected behavior
- Clear distinction between silent tracking and user-facing feedback

## What didn't work
- Previous version had repetitive instructions that could confuse the agent
- Overly aggressive formatting (too many emojis and symbols) made it harder to parse
- Lack of structured examples left interpretation ambiguous
- The agent didn't have a purpose section that outlines the goal of the agent

## Insights gained
- AI agents follow instructions better with clear, numbered sequences rather than scattered rules
- Validation checklists improve compliance rates
- Separating "what to do" from "how to format" improves clarity and Providing examples is critical for demonstrating expected behavior
- gpt-5-mini was calling the tools more often than gpt-4o, it was following the instructions better
- There were random errors while calling the tools and connecting to the mcp server throwing 502 server response
```
2026-02-02 13:40:10.345 [info] Connection state: Error 502 status sending message to https://mcppulse.10academy.org/proxy: <html>
<head><title>502 Bad Gateway</title></head>
<body>
<center><h1>502 Bad Gateway</h1></center>
<hr><center>nginx</center>
</body>
</html>
```

## Artifacts created
- `documentation.md` 
- `copilot-instructions-old.md` (original rule file - archived)
- `.github/copilot-instructions.md` (improved rule file with better structure)

