# Claude Code Rules for portfolio

## 基本方針
- 開発は必ず Issue ベースで行う
- 作業開始時は `gh issue view <issue-number>` で要件を確認する
- GitHub 操作は必ず `gh` コマンドを使用する

## Branch Rules
- `main` ブランチで直接作業しない
- 作業開始時は必ず作業ブランチを作成する
- ブランチ命名規則: `feat/<issue-number>-<short-description>`

## 作業フロー
- Issue確認 → 調査 → 実装 → 動作確認 の順で進める
- 実装完了後、1 Issue = 1 Commit とする
- PR は、実装と動作確認がすべて完了した後にのみ作成する
- 最後に Draft PR を作成する（本文に `Fixes #<issue-number>` を含める）

## PR Review Handling Rules
- PR にレビューコメントがある場合は、`gh pr view --comments` で内容を確認すること
- レビューコメントに沿って修正を行うこと
- 修正後は必ず動作確認を行うこと
- 修正内容は 1 つのコミットにまとめること
- レビュー対応時は新しい PR を作成せず、既存の PR を更新すること
- 修正後は commit & push し、PR を更新すること
- 変更点と確認手順を PR コメントとして簡潔にまとめて返信すること
- PR には Summary と Test plan を必ず含めること