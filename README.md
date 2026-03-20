# APEX TRACKER 🎮

🇯🇵 [日本語](#日本語) | 🌏 [English](#english)

---

## 日本語

Apex Legends の戦績を記録・分析する個人向けWebアプリです。
インストール不要。ブラウザだけで動作します。

### 機能

- **戦績記録** — 日付・ランク・ポイント変動・メモを入力して保存
- **履歴管理** — 全記録の一覧表示・メモ検索・削除
- **グラフ表示** — 累積ポイント推移 / ランク別平均 / 曜日別平均。昇格日を縦線で可視化
- **AI分析** — 試合後のメモをClaudeが解析し、苦手パターン・得意な点・改善アドバイスを自動抽出
- **データ管理** — JSONエクスポート / インポート（複数デバイス間のデータ移行に対応）
- **スマホ対応** — ボトムナビゲーション付きのモバイルフレンドリーなUI

### 使い方

#### 1. アクセス

```
https://ksmshkt.github.io/apex-tracker/
```

#### 2. 戦績を記録する

「記録」タブで日付・ランク・ポイント変動を入力して「RECORD」を押すだけ。
試合後の気づきや反省をメモ欄に書いておくと、AI分析の精度が上がります。

#### 3. AI分析を使う

AI分析機能を使うには **Anthropic の APIキー** が必要です。

1. [console.anthropic.com](https://console.anthropic.com) でアカウントを作成（無料で $5 クレジット付き）
2. 「API Keys」→「Create Key」でキーを発行
3. アプリの「設定」タブにキーを入力して「SAVE」
4. 「AI分析」タブで「ANALYZE」を押すと分析開始

> ⚠️ APIキーはブラウザのLocalStorageにのみ保存されます。外部サーバーには送信されません。

#### 4. データのバックアップ・移行

「データ」タブから全記録をJSONファイルとしてエクスポートできます。
別のデバイスで使いたい場合は、そのJSONファイルをインポートするだけで引き継げます。

### データの保存場所

| データ | 保存場所 |
|---|---|
| 戦績記録 | ブラウザの LocalStorage |
| APIキー | ブラウザの LocalStorage |

※ データはブラウザ・デバイスごとに独立しています。デバイス間の同期には手動エクスポート/インポートを使ってください。

### ローカルで動かす

```bash
git clone https://github.com/ksmshkt/apex-tracker.git
open index.html
```

---

## English

A personal web app for tracking and analyzing your Apex Legends ranked stats.
No installation required — runs entirely in the browser.

### Features

- **Stats Recording** — Log date, rank, point changes, and session memos
- **History Management** — Browse all records, search memos, and delete entries
- **Charts** — Cumulative points graph / average by rank / average by day of week. Promotion dates visualized with vertical markers
- **AI Analysis** — Claude analyzes your session memos to extract weak points, strengths, and improvement tips
- **Data Management** — JSON export / import for cross-device data migration
- **Mobile Friendly** — Responsive UI with bottom navigation for smartphone use

### How to Use

#### 1. Access

```
https://ksmshkt.github.io/apex-tracker/
```

#### 2. Record your stats

Open the「Record」tab, enter the date, rank, and point change, then hit「RECORD」.
Writing memos about your session improves the accuracy of AI analysis.

#### 3. Use AI Analysis

AI analysis requires an **Anthropic API key**.

1. Create an account at [console.anthropic.com](https://console.anthropic.com) (free $5 credit included)
2. Go to「API Keys」→「Create Key」
3. Enter your key in the app's「Settings」tab and click「SAVE」
4. Open the「AI Analysis」tab and press「ANALYZE」

> ⚠️ Your API key is stored only in your browser's LocalStorage and is never sent to any external server.

#### 4. Backup & Migration

Export all records as a JSON file from the「Data」tab.
To use on another device, simply import the JSON file.

### Data Storage

| Data | Storage |
|---|---|
| Stats records | Browser LocalStorage |
| API key | Browser LocalStorage |

Note: Data is stored per browser and device. Use manual export/import to sync across devices.

### Run Locally

```bash
git clone https://github.com/ksmshkt/apex-tracker.git
open index.html
```

---

## Tech Stack

- HTML / CSS / JavaScript (no framework)
- [Chart.js](https://www.chartjs.org/) — Chart rendering
- [Anthropic Claude API](https://www.anthropic.com/) — AI analysis
- Google Fonts (Rajdhani / Noto Sans JP)

---

## License

MIT License

---

## Disclaimer

- This is an unofficial fan-made tool. Not affiliated with Apex Legends, EA, or Respawn Entertainment.
- API usage fees for AI analysis are charged to your own Anthropic account.

---

## Author

[@ksmshkt](https://github.com/ksmshkt)
