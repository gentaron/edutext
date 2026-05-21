<div align="center">

# EDU Text

**Eternal Dominion Universe — Story & Lore Text Repository**

[English](#english) · [日本語](#日本語)

</div>

[![License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)]()

---

## 日本語

### 概要

EDU Text は Eternal Dominion Universe（EDU）のストーリー・世界観テキストの集中管理リポジトリ。キャラクターの物語、歴史、世界設定をプレーンテキストで保存し、他の EDU サイト（laylaland, irisworlds 等）から直接参照されるコンテンツソース。ビルドシステムやコードは含まず、純粋なテキストコンテンツのみで構成される。

### 収録内容

| カテゴリ | ファイル例 | 説明 |
|---------|-----------|------|
| **キャラクターストーリー** | `LAYLA.txt`, `LAYLA_JP.txt`, `IRIS_1.txt`–`IRIS_4.txt` | Layla, Iris, Jen, Myu, Gentaro, Diana, Jun 等の物語 |
| **世界観・歴史** | `worldedu.txt`, `unified-history.txt`, `eduuni.txt` | E16 連星系の統一歴史と世界設定 |
| **キャラクター統計** | `laylastats.txt`, `kateclaudiaandlilliesteiner.txt` | キャラクターのステータスデータ |

### ファイル命名規則

- **日本語**: `ファイル名.txt`（例: `LAYLA_JP.txt`）
- **英語**: `ファイル名_EN.txt`（例: `IRIS_1_EN.txt`）
- または `_JP` / `_EN` サフィックスで言語を区別

### 利用方法

他リポジトリからの参照例（laylaland `story.html`）:

```html
<script>
fetch('https://raw.githubusercontent.com/gentaron/edutext/main/LAYLA.txt')
  .then(res => res.text())
  .then(text => { /* ストーリーを表示 */ });
</script>
```

### Contributing

新しいストーリーや lore を追加する場合：

1. テキストファイル（`.txt`）を作成
2. 日本語版と英語版の両方を用意（`_JP` / `_EN` サフィックス）
3. UTF-8 エンコードで保存
4. `main` ブランチにコミット

---

## English

### Overview

EDU Text is the central content repository for story and lore text files of the Eternal Dominion Universe (EDU). It stores character stories, history, and worldbuilding in plain text format, consumed directly by other EDU sites (laylaland, irisworlds, etc.) via raw GitHub URLs. No code or build system — purely text content.

### Content Categories

| Category | Examples | Description |
|----------|----------|-------------|
| **Character Stories** | `LAYLA.txt`, `IRIS_1.txt`–`IRIS_4.txt` | Stories for Layla, Iris, Jen, Myu, Gentaro, Diana, Jun, etc. |
| **World & History** | `worldedu.txt`, `unified-history.txt` | Unified history and world settings of the E16 binary star system |
| **Character Stats** | `laylastats.txt` | Character status data |

### Naming Convention

- **Japanese**: `filename_JP.txt` (e.g., `LAYLA_JP.txt`)
- **English**: `filename_EN.txt` (e.g., `IRIS_1_EN.txt`)

### Consumers

- [gentaron/laylaland](https://github.com/gentaron/laylaland) — Fetches `LAYLA.txt` / `LAYLA_JP.txt` for story reader
- [gentaron/edu](https://github.com/gentaron/edu) — Main EDU application

---

## Related Repositories

| Repo | Description |
|------|-------------|
| [gentaron/edu](https://github.com/gentaron/edu) | Main EDU application |
| [gentaron/image](https://github.com/gentaron/image) | Character artwork |
| [gentaron/laylaland](https://github.com/gentaron/laylaland) | Layla character site (consumer) |
| [gentaron/irisworlds](https://github.com/gentaron/irisworlds) | Iris character site (consumer) |
| [gentaron/eurekaspace](https://github.com/gentaron/eurekaspace) | EDU encyclopedia site |

## License

[MIT](LICENSE)
