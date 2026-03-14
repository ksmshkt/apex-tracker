# APEX TRACKER 🎮

Apex Legends の戦績を記録・分析する個人向けWebアプリです。  
インストール不要。ブラウザだけで動作します。

---

## 機能

- **戦績記録** — 日付・ランク・ポイント変動・メモを入力して保存
- **履歴管理** — 全記録の一覧表示・メモ検索・削除
- **グラフ表示** — 累積ポイント推移 / ランク別平均 / 曜日別平均。昇格日を縦線で可視化
- **AI分析** — 試合後のメモをClaudeが解析し、苦手パターン・得意な点・改善アドバイスを自動抽出
- **データ管理** — JSONエクスポート / インポート（複数デバイス間のデータ移行に対応）
- **スマホ対応** — ボトムナビゲーション付きのモバイルフレンドリーなUI

---

## 使い方

### 1. アクセス

```
https://ksmshkt.github.io/apex-tracker/
```

### 2. 戦績を記録する

「記録」タブで日付・ランク・ポイント変動を入力して「RECORD」を押すだけ。  
試合後の気づきや反省をメモ欄に書いておくと、AI分析の精度が上がります。

### 3. AI分析を使う

AI分析機能を使うには **Anthropic の APIキー** が必要です。

1. [console.anthropic.com](https://console.anthropic.com) でアカウントを作成（無料で $5 クレジット付き）
2. 「API Keys」→「Create Key」でキーを発行
3. アプリの「設定」タブにキーを入力して「SAVE」
4. 「AI分析」タブで「ANALYZE」を押すと分析開始

> ⚠️ APIキーはブラウザのLocalStorageにのみ保存されます。外部サーバーには送信されません。

### 4. データのバックアップ・移行

「データ」タブから全記録をJSONファイルとしてエクスポートできます。  
別のデバイスで使いたい場合は、そのJSONファイルをインポートするだけで引き継げます。

---

## データの保存場所

| データ | 保存場所 |
|---|---|
| 戦績記録 | ブラウザの LocalStorage |
| APIキー | ブラウザの LocalStorage |

※ データはブラウザ・デバイスごとに独立しています。デバイス間の同期には手動エクスポート/インポートを使ってください。

---

## 技術スタック

- HTML / CSS / JavaScript（フレームワーク不使用）
- [Chart.js](https://www.chartjs.org/) — グラフ描画
- [Anthropic Claude API](https://www.anthropic.com/) — AI分析
- Google Fonts（Rajdhani / Noto Sans JP）

---

## ローカルで動かす

ファイルをダウンロードしてブラウザで開くだけです。サーバーは不要です。

```bash
# リポジトリをクローン
git clone https://github.com/あなたのユーザー名/apex-tracker.git

# index.html をブラウザで開く
open index.html
```

---

## ライセンス

MIT License

---

## 注意事項

- このアプリは非公式ツールです。Apex Legends および EA / Respawn Entertainment とは無関係です。
- AI分析の利用にかかる API 費用はご自身の Anthropic アカウントに発生します。
