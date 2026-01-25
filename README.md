# Legal Documents - GitHub Pages

アプリのプライバシーポリシー・利用規約をホスティングするためのリポジトリ。

## セットアップ手順

### 1. 新しいリポジトリを作成

1. GitHubで新しいリポジトリを作成
   - リポジトリ名: `legal` または `policies`
   - Public（GitHub Pages無料利用のため）
   - READMEは追加しない

2. ローカルでこのフォルダの内容をpush

```bash
# このフォルダ（github-pages）に移動
cd docs/legal/github-pages

# Gitリポジトリを初期化
git init
git add .
git commit -m "Initial commit: Legal documents for HabitTracker"

# リモートリポジトリを追加してpush
git remote add origin https://github.com/YOUR_USERNAME/legal.git
git branch -M main
git push -u origin main
```

### 2. GitHub Pagesを有効化

1. リポジトリの **Settings** → **Pages** に移動
2. **Source** で `Deploy from a branch` を選択
3. **Branch** で `main` を選択し、フォルダは `/ (root)` のまま
4. **Save** をクリック

### 3. 公開URLを確認

数分後、以下のURLでアクセス可能になります：

```
https://YOUR_USERNAME.github.io/legal/
https://YOUR_USERNAME.github.io/legal/habittracker/privacy-ja.html
https://YOUR_USERNAME.github.io/legal/habittracker/privacy-en.html
https://YOUR_USERNAME.github.io/legal/habittracker/terms-ja.html
https://YOUR_USERNAME.github.io/legal/habittracker/terms-en.html
```

## 要更新箇所

各HTMLファイル内の以下を実際の情報に置き換えてください：

- `[運営者名]` / `[Operator name]`
- `[メールアドレス]` / `[Email address]`

## ファイル構成

```
.
├── index.html              # アプリ一覧ページ
├── README.md               # このファイル
└── habittracker/           # HabitTracker用
    ├── privacy-ja.html     # プライバシーポリシー（日本語）
    ├── privacy-en.html     # Privacy Policy（英語）
    ├── terms-ja.html       # 利用規約（日本語）
    └── terms-en.html       # Terms of Service（英語）
```

## 新しいアプリを追加する場合

1. 新しいフォルダを作成（例: `newapp/`）
2. 既存のHTMLをコピーして内容を編集
3. `index.html` にリンクを追加
4. commit & push

## ストア提出時のURL

App Store / Google Play に提出する際は以下のURLを使用：

| 項目 | 日本語 | 英語 |
|------|--------|------|
| プライバシーポリシー | `https://USERNAME.github.io/legal/habittracker/privacy-ja.html` | `https://USERNAME.github.io/legal/habittracker/privacy-en.html` |
| 利用規約 | `https://USERNAME.github.io/legal/habittracker/terms-ja.html` | `https://USERNAME.github.io/legal/habittracker/terms-en.html` |

※ストア設定では通常、1言語につき1URLを指定。日本語ストアには日本語URL、英語ストアには英語URLを設定。
