# sunaru-legal

旅程管理アプリ「SUNARU」のプライバシーポリシーと利用規約を GitHub Pages で公開するためのリポジトリ。

## 公開手順

1. GitHub で `sunaru-legal` リポジトリを新規作成（Public）
2. ローカルで初期化して push：

   ```bash
   cd /Users/NabeMacPro/ClaudeCode/sunaru-legal
   git init -b main
   git add .
   git commit -m "Initial: privacy / terms"
   git remote add origin https://github.com/<your-account>/sunaru-legal.git
   git push -u origin main
   ```

3. GitHub の Settings → Pages → Source: `Deploy from a branch` → Branch: `main` / Folder: `/ (root)` → Save
4. 数分後に `https://<your-account>.github.io/sunaru-legal/` で公開される

## URL（公開後に決定）

- トップ：`https://<your-account>.github.io/sunaru-legal/`
- プラポリ：`https://<your-account>.github.io/sunaru-legal/privacy.html`
- 規約：`https://<your-account>.github.io/sunaru-legal/terms.html`

これらの URL を Play Console（プラポリ欄）とアプリ本体（将来の設定画面リンク）に登録する。

## 更新フロー

本文を直すときは `privacy.md` / `terms.md` を編集して push するだけで Pages が再生成される。
tabi-app 本体側の `docs/legal/*.md` とは独立管理（変更時は両方同期する）。
