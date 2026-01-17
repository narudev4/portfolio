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
- 最後に Draft PR を作成する（本文に `Fixes #<issue-number>` を含める）