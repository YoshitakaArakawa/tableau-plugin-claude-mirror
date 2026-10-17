# tableau-plugin-claude-mirror

[tableau/tableau-plugin](https://github.com/tableau/tableau-plugin) の Claude 向けビルド済みプラグインの**写し（ミラー）**です。claude.ai の「マーケットプレイスを追加」から入れられるように置いています。ブログで手順を紹介するために、個人で用意しました。

- Salesforce, Inc.／Tableau の公式リポジトリではありません。このリポジトリについてのサポートもありません
- 中身は上流の `dist/claude` ブランチ（上流の GitHub Actions が main から本番版をビルドしたもの）を、ファイルを変えずに写したものです。追加したのは、この README と、ルートの `LICENSE.txt`（上流の `LICENSE.txt` の写し）だけです
- 上流の `dist/claude` は上流リポジトリの既定ブランチではないため、claude.ai には上流の URL を直接追加できません。このリポジトリは、その間をつなぐためのものです。公式の入れ方が用意されたら、そちらを使ってください

## ビルド元

| 項目 | 値 |
|---|---|
| 上流 | https://github.com/tableau/tableau-plugin |
| ビルド元のコミット（main） | `1249e59d57fb1ce51faf0ec614b0c75e8cf65144`（2026-10-15） |
| 写した `dist/claude` のコミット | `684ab277dff80f2a59bc360d01b0db3a76431498`（2026-10-15） |
| プラグインのバージョン | 1.1.0 |
| 接続先の MCP サーバー | `https://mcp.tableau.com`（Tableau がホストする Tableau MCP） |

このリポジトリは自動では更新されません。「自動的に同期」をオンにしていても、届くのはこのリポジトリを更新したときだけです。

## claude.ai での入れ方

Claude の有料プラン（Pro 以上）が必要です。web・デスクトップアプリ・スマホのブラウザで同じ手順です。

1. claude.ai の「カスタマイズ → プラグイン」で「マーケットプレイスを追加」を開き、URL に `YoshitakaArakawa/tableau-plugin-claude-mirror` と入れて同期します
2. 追加されたマーケットプレイスから「Tableau」をインストールします
3. 「コネクタ」で Tableau に接続し、Tableau Cloud のサインイン画面でサインインして許可します
4. 「設定 → 機能」でコード実行をオンにします
5. 新しいチャットを開いて使います

## ライセンス

上流と同じ Apache License 2.0 です（`LICENSE.txt`）。なお上流の `plugin.json` には `"license": "MIT"` とありますが、上流リポジトリが同梱している `LICENSE.txt` は Apache License 2.0 です。このリポジトリは `LICENSE.txt` に従います。

Tableau は Salesforce, Inc. の商標です。
