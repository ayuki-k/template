# pre-commitの設定
📦 保存方法
下記を ~/.gitmessage.txt に保存
```
# ==== Commit Messages ====

# ==== Commit Messages(Template) ====

# === 📌 基本フォーマット ===
# Tag: [#issue number] message
# [タグ]: (optional #issue番号) 何を・なぜ・どうしたか（過去形で書く）

# --- 例 ---
# ✨ feature: ユーザーダッシュボードに通知バナーを追加した
# 🐛 fix: #123 利用規約の誤字を修正した
# 🔨 refactor: useEffect内の重複ロジックを関数に切り出した

# === 🏷️ タグ一覧（prefix） ===

# ✨ feature:   新機能追加・UI変更・API実装など
# 🐛 fix:       バグ修正・不具合対応
# 🔨 refactor:  構造改善・スタイル整理（機能変更なし）
# 🔧 chore:     ビルド設定・CI/CD・依存パッケージ更新など
# 📚 doc:       ドキュメント・README・コメントの修正
# 🧪 test:      テストの追加・修正・カバレッジ向上

# === 🔔 注意事項 ===

# - 文は必ず「過去形」で書く（何を"した"のか）
# - Why を含めると、履歴が読みやすくなる
# - issueがある場合は #番号 を付ける（例: #42）
# - 1コミット1目的を意識する（小さく区切る）

```

Gitに設定：
```
git config --global commit.template ~/.gitmessage.txt
```

以降、git commit したときにテンプレートがエディタに表示されます。