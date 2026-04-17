# ルーティントラッカー PWA

## ファイル構成

```
routine-tracker/
├── index.html      ← メインアプリ
├── manifest.json   ← PWA設定
├── sw.js           ← オフライン対応
├── icon-192.png    ← アプリアイコン（要作成）
└── icon-512.png    ← アプリアイコン（要作成）
```

---

## 公開手順（GitHub Pages）

### 1. アイコンを用意する
- https://svgtopng.com/ でアイコンSVGをPNGに変換
- `icon-192.png`（192×192px）と `icon-512.png`（512×512px）を用意

### 2. GitHubにアップロード
1. https://github.com にアクセス・ログイン
2. 右上の「＋」→「New repository」
3. Repository name: `routine-tracker`（任意）
4. Public を選択 → 「Create repository」
5. 「uploading an existing file」をクリック
6. このフォルダの全ファイルをドラッグ＆ドロップ
7. 「Commit changes」をクリック

### 3. GitHub Pages を有効にする
1. リポジトリの「Settings」タブ
2. 左メニュー「Pages」
3. Source: 「Deploy from a branch」
4. Branch: `main` / `/ (root)` を選択 → 「Save」
5. 数分後に `https://ユーザー名.github.io/routine-tracker/` で公開！

---

## iPhoneでホーム画面に追加する方法

1. SafariでアプリのURLを開く
2. 下部の「共有」ボタン（四角＋矢印）をタップ
3. 「ホーム画面に追加」をタップ
4. 「追加」をタップ

→ ホーム画面にアイコンが追加され、アプリとして起動できます！

---

## 特徴
- オフラインでも動作（Service Worker対応）
- データはスマホ・PCのブラウザに保存
- ダークモード自動対応
