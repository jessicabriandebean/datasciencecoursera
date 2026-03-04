---
name: testing
description: What this skill does and when Claude should use it (max 200 chars - critical for auto-invocation)
---

# Testing
#Instructions

When this skill is invoked:

Do this first
Then do this
Finally do this

##:::accordion{title="SKILL.md Required vs Optional Fields" type="info"}
**Required fields:**
- `name`: Human-friendly name (max 64 characters)
- `description`: What the skill does (max 200 characters) - Claude uses this to decide when to invoke

**Optional fields:**
- `dependencies`: Software packages required (e.g., "python>=3.8")
:::