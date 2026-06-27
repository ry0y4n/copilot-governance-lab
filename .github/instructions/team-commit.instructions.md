---
applyTo: "**/*"
description: Team commit message review policy for GitHub Copilot customization governance.
---

# Team Commit Instructions

このリポジトリでは、commit message と PR の説明を Conventional Commits に寄せて書きます。

## Commit Message

- 基本形は `type(scope): subject` とする
- 変更範囲が不要な場合は `type: subject` でもよい
- 種別は `feat`、`fix`、`docs`、`test`、`refactor`、`chore` を基本とする
- 説明部分は 72 文字以内を目安にする
- 説明部分の末尾に句点を付けない
- 変更理由や移行注意がある場合は body に書く
- 破壊的変更は `!` または `BREAKING CHANGE:` フッターで明示する

## Review

commit message を提案またはレビューするときは、形式、具体性、影響範囲、破壊的変更の有無を確認する。
