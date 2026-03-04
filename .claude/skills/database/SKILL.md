---
name: db-migrate
description: Safely handle database migrations with backup verification and rollback planning
---
Safety Rules

ALWAYS backup before migrating
NEVER drop tables in production
Review generated SQL before execution

Workflow

Check current migration status
Generate migration file
Review the changes
Ask for confirmation
Run migration
Verify success

:::

:::accordion{title="PR Review Skill" type="tip"}
```markdown
---
name: pr-review
description: Thoroughly review pull requests for quality, security, and best practices
---

# PR Review Skill

Checklist

 Code quality and readability
 Test coverage
 Security implications
 Performance impact
 Documentation updates

 Output Format

Provide feedback in this format:

Critical issues (must fix)
Suggestions (should consider)
Good practices observed

:::

# Database Migration Skill
# Database
##Instructions

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