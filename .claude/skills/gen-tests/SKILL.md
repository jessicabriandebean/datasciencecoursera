---
name: gen-tests
description: Generate comprehensive unit tests
command: /gen-tests
model: sonnet
---

## Test Generation Skill

Generate tests for: **$ARGUMENTS**

## Test Coverage Targets

- Happy path scenarios
- Edge cases (null, empty, boundary)
- Error handling
- Async behavior (if applicable)

## Output Format

- Use Jest/Vitest syntax
- Group with describe blocks
- Clear test names explaining behavior
- Include setup/teardown when needed