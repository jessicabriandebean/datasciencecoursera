---
name: deploy
description: Safe deployment workflow with pre-checks and rollback capability
command: /deploy
---

## Pre-Deployment Checks

- All tests passing
- No uncommitted changes
- Version bumped
- Changelog updated

## Safety Rules

- NEVER deploy on Friday after 3pm
- ALWAYS create a backup before deploying
- REQUIRE manual confirmation for production

## Workflow

1. Run npm test - abort if failing
2. Run npm run build - abort on errors
3. Create git tag with version
4. Push to deployment branch
5. Monitor for errors (5 minutes)
6. Report success or trigger rollback