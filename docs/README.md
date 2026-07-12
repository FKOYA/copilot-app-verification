# docs/ について

ここは **LOG.md と Verification-checklist.md に検証結果が溜まってから**、後から見返しやすい形に再構成する場所。検証を始めた直後は空のままでよく、パターンが見えてきた段階でファイルを追加していく(計画書「3. リポジトリ設計」参照)。

`Verification-checklist.md` の「結果」列が埋まってきたら、それらを次のような観点別ファイルに要約・整理するイメージ。

## 想定するファイル例

- `github-integration.md` — Inbox 起点のタスク実行、PR 作成〜レビュー〜マージ、CI 表示の検証結果まとめ(異常系: 権限誤爆・中断時の状態を含む)
- `parallel-sessions.md` — 並列セッションの速度・リソース消費・ブランチ競合の検証結果まとめ
- `scheduled-workflows.md` — スケジュールワークフロー(Issue 自動整理・リリースノート生成など)の設定と安定性の検証結果まとめ
- `comparison.md` — VSCode の Copilot Chat / GitHub.com の Copilot / Claude Code との比較表(差別化仮説との答え合わせ)
- `real-project-findings.md` — Step 4(実プロジェクトでの限定検証)の結果転記。サンドボックスとの挙動差を明記
- `conclusion.md` — Step 5 で書く最終結論(他ツールとの差別化・実開発での活用方法)

## 書き方の目安

各ファイルは LOG.md / Verification-checklist.md という「生データ」への参照(該当 Issue 番号・検証日)を残しつつ、「結局どうだったか」を先に書く。生ログの再掲にしない。
