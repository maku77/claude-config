---
allowed-tools: Bash(git status:*), Bash(git diff:*), Bash(git log:*), Bash(git branch --show-current:*)
description: "Generate an appropriate git commit message based on the current code changes and create the commit."
---

## Context

- Current git status: !`git status`
- Current git diff (including staged and unstaged changes): !`git diff HEAD`
- Current branch: !`git branch --show-current`
- Recent commit logs: !`git log --oneline -10`

## Your task

Based on the above diff, generate a suitable git commit message
following a conventional format (e.g., Conventional Commits),
and execute a single git commit using that message.

Do not include additional Co-Authors or metadata in the commit message like the following (behave as if `"includeCoAuthoredBy": false` is set):

```
🤖 Generated with [Claude Code](https://claude.ai/code)

Co-Authored-By: Claude <noreply@anthropic.com>
```

After committing, display the latest commit message using `git log HEAD...HEAD~1`.

## Additional instructions

$ARGUMENTS

