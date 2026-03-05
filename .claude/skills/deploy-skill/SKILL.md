---
name: deploy-skill
hooks:
  - event: PreToolUse
    match: Bash(deploy*)
    command: npm run type-check
  - event: PostToolUse
    match: Bash(deploy*)
    command: curl https://api.example.com/health
  - event: Stop
    command: osascript -e 'display notification "Deploy complete"'
---