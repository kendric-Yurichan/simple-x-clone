# SimpleX

シンプルな X 風 SNS アプリ。Supabase バックエンド + GitHub Pages ホスティング。

## 機能
- メール / パスワードでの会員登録・ログイン
- 280文字以内でのつぶやき投稿
- タイムライン表示（リアルタイム更新）
- 自分の投稿を削除

## セットアップ（ローカル開発）

```bash
cp config.example.js config.js
# config.js を開いて Supabase の URL と anon key を記入
# その後 index.html をブラウザで開く
```

## デプロイ

GitHub Actions が `main` ブランチへの push 時に自動デプロイします。
事前に GitHub Secrets へ以下を設定してください:

| Secret 名          | 内容                        |
|--------------------|----------------------------|
| `SUPABASE_URL`     | Supabase プロジェクト URL   |
| `SUPABASE_ANON_KEY`| Supabase anon (public) key  |
