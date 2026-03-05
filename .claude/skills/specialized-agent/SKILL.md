---
name: specialized-agent
description: Run code review and test writing using restricted sub-agents
tools: Task(agent_type:code-reviewer), Task(agent_type:test-writer)
---

# Specialized Agent Skill

Perform a focused review and test generation using restricted sub-agents.

## Workflow

1. Spawn `code-reviewer` agent to review the provided code
2. Spawn `test-writer` agent to generate missing tests
3. Compile results into a unified report

## Instructions

- Only `code-reviewer` and `test-writer` sub-agents may be spawned
- Run both agents in parallel when possible
- Report findings grouped by agent
