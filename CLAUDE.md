# inspection-form — Claude Code メモリー

LIFF で使う点検・日報系の HTML フォーム群（`*.html`）のリポジトリ。

---

## 運用ルール

### git
- 作業開始時に `git pull` し、作業終了時にコミットして push する（1コミット1目的）
- AIエージェントの作業は作業ブランチで行う。main への反映と本番へのデプロイは、人間が確認してから行う

### シークレット
- APIキー・トークンなどはコード（HTML / JS）に書かず、`.gitignore` で除外された設定ファイルに置く
- 現在の `.gitignore` は `.wrangler/` のみを除外している。`.env` などの設定ファイルを作るときは、先に `.gitignore` に追加する
