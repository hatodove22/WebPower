# WebPower

WebPower は HCI/心理統計向けのパワー分析ツールです。GitHub Pages でホストできるスタティックな Web アプリとして構成されており、ブラウザのみで動作します。本プロジェクトの初期コンテンツは **Gemini 3.0 Pro** で生成しました。

## 技術スタック
- **HTML + Tailwind CSS**: コンポーネントのレイアウトとスタイル。
- **PyScript 2024.1.1**: ブラウザ上で Python を実行し、インタラクティブな計算を提供。
- **NumPy / SciPy / statsmodels**: 効果量・検定・パワー計算のコアロジックを Python 側で実装。
- **Matplotlib**: パワーカーブの可視化を描画。

## ローカルでの確認
1. リポジトリをクローンします。
2. `main.html` をブラウザで直接開きます（Python などの追加セットアップは不要です）。

## GitHub Pages 公開手順
1. GitHub 上で本リポジトリを作成し、コードをプッシュします。
2. リポジトリの **Settings › Pages** を開き、Branch に `main`（またはデフォルトブランチ）を選び、`/ (root)` を指定して保存します。
3. 数十秒待つと `https://<your-account>.github.io/<repository>/` で公開されます。トップの `index.html` から `main.html` に即時リダイレクトされます。

## プロジェクト構成
- `index.html`: GitHub Pages 用のエントリーポイント。`main.html` へリダイレクトします。
- `main.html`: アプリ本体。サイドバーから検定種別を選択し、パラメータ入力後に「Calculate」でパワーと必要サンプルサイズを計算・可視化します。

## ライセンス
MIT License。
