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
- **データ管理** — JSONエクスポート / インポート（複数デバイス間のデータ移行に対応）
- **スマホ対応** — ボトムナビゲーション付きのモバイルフレンドリーなUI

### 使い方

#### 1. アクセス

```
https://ksmshkt.github.io/apex-tracker/
```

#### 2. 戦績を記録する

「記録」タブで日付・ランク・ポイント変動を入力して「RECORD」を押すだけ。
試合後の気づきや反省をメモ欄に書いておけば、履歴から後で見返せます。

#### 3. データのバックアップ・移行

「データ」タブから全記録をJSONファイルとしてエクスポートできます。
別のデバイスで使いたい場合は、そのJSONファイルをインポートするだけで引き継げます。

### データの保存場所

| データ | 保存場所 |
|---|---|
| 戦績記録 | ブラウザの LocalStorage |

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
- **Data Management** — JSON export / import for cross-device data migration
- **Mobile Friendly** — Responsive UI with bottom navigation for smartphone use

### How to Use

#### 1. Access

```
https://ksmshkt.github.io/apex-tracker/
```

#### 2. Record your stats

Open the「Record」tab, enter the date, rank, and point change, then hit「RECORD」.
Writing memos about your session lets you look back on them later from History.

#### 3. Backup & Migration

Export all records as a JSON file from the「Data」tab.
To use on another device, simply import the JSON file.

### Data Storage

| Data | Storage |
|---|---|
| Stats records | Browser LocalStorage |

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
- Google Fonts (Rajdhani / Noto Sans JP)

---

## License

MIT License

---

## Disclaimer

- This is an unofficial fan-made tool. Not affiliated with Apex Legends, EA, or Respawn Entertainment.

---

## Author

[@ksmshkt](https://github.com/ksmshkt)
