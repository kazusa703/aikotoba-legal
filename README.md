# aikotoba Legal Documents

aikotobaアプリの利用規約・プライバシーポリシーです。

## ファイル構成

```
├── terms.html      # 利用規約（HTML）
├── privacy.html    # プライバシーポリシー（HTML）
├── terms.md        # 利用規約（Markdown）
├── privacy.md      # プライバシーポリシー（Markdown）
└── README.md       # このファイル
```

## GitHub Pagesでの公開方法

1. GitHubでリポジトリを作成（例: `aikotoba-legal`）

2. ファイルをアップロード
   ```bash
   git init
   git add .
   git commit -m "Add legal documents"
   git branch -M main
   git remote add origin https://github.com/あなたのユーザー名/aikotoba-legal.git
   git push -u origin main
   ```

3. GitHub Pagesを有効化
   - リポジトリの Settings → Pages
   - Source: Deploy from a branch
   - Branch: main / root
   - Save

4. 公開URL
   ```
   https://あなたのユーザー名.github.io/aikotoba-legal/terms.html
   https://あなたのユーザー名.github.io/aikotoba-legal/privacy.html
   ```

## アプリでの設定

`SettingsView.swift` のURLを更新：

```swift
Link("利用規約", destination: URL(string: "https://あなたのユーザー名.github.io/aikotoba-legal/terms.html")!)

Link("プライバシーポリシー", destination: URL(string: "https://あなたのユーザー名.github.io/aikotoba-legal/privacy.html")!)
```

## カスタマイズ

### メールアドレスの設定

`privacy.html` と `privacy.md` の以下の部分を実際のメールアドレスに置き換えてください：

```
[お問い合わせ用メールアドレス]
```

### 会社名・サービス名

必要に応じて「当社」を会社名に変更してください。

## ライセンス

このドキュメントは aikotoba アプリ専用です。
