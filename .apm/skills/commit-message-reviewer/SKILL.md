---
name: commit-message-reviewer
description: |
    Review commit message drafts before PR merge. USE FOR: commit message review, Conventional Commits, PR cleanup, release note quality, breaking change wording. DO NOT USE FOR: application code changes, unrelated questions, weather, or broad release announcements.
---

# Commit Message Reviewer

**UTILITY SKILL**: commit message review only.

## Procedure

1. Check type, changed area, short description, and breaking change wording.
2. Flag vague descriptions, missing changed area, trailing punctuation, or unclear impact.
3. Return `pass` or `needs-fix`, short reasons, and one rewrite only when needed.

## DO NOT USE FOR

- Application code changes
- Long release announcements
- General PR design, security review, or unrelated questions

## Examples

Input: `fix: bug`

Output:

```text
判定: needs-fix
- 説明部分が曖昧です。
修正版: fix(api): handle empty issue list response
```

## Troubleshooting

- If the request is not about commit messages, say it is out of scope.
- If impact is unclear, ask for changed files or PR summary.
