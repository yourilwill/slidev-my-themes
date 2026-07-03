# slidev-theme-catppuccin-mocha

[Catppuccin Mocha](https://github.com/catppuccin/catppuccin) のカラーパレットを使った [Slidev](https://sli.dev) 用のダークテーマです。

## インストール

`slides.md` の frontmatter で指定します。

```yaml
---
theme: catppuccin-mocha
---
```

ローカルパッケージとして参照する場合は、プレゼンテーション側の `package.json` に以下を追加してください。

```json
{
  "dependencies": {
    "slidev-theme-catppuccin-mocha": "file:../packages/theme-catppuccin-mocha"
  }
}
```

## カラーパレット

Catppuccin Mocha 公式の26色トークンを `--ctp-<name>` という命名規則の CSS カスタムプロパティとして定義しています。

| 変数 | HEX | 用途 |
| --- | --- | --- |
| `--ctp-base` | `#1e1e2e` | 背景 |
| `--ctp-mantle` | `#181825` | cover レイアウトのグラデーション |
| `--ctp-crust` | `#11111b` | 予約 |
| `--ctp-surface0` | `#313244` | GoodItem/BadItem のアイコン背景 |
| `--ctp-surface1` | `#45475a` | h1 下線、code/pre 背景、テーブルヘッダー背景 |
| `--ctp-surface2` | `#585b70` | 予約 |
| `--ctp-overlay0` | `#6c7086` | pre 枠線、cover の補足テキスト |
| `--ctp-overlay1` / `--ctp-overlay2` | `#7f849c` / `#9399b2` | 予約 |
| `--ctp-subtext0` / `--ctp-subtext1` | `#a6adc8` / `#bac2de` | 予約 |
| `--ctp-text` | `#cdd6f4` | 本文の文字色 |
| `--ctp-mauve` | `#cba6f7` | プライマリカラー（h1、リストマーカー、テーブル強調） |
| `--ctp-pink` | `#f5c2e7` | セカンダリカラー（h2） |
| `--ctp-sky` | `#89dceb` | h3、リンク、テーブルヘッダー文字 |
| `--ctp-peach` | `#fab387` | strong（太字） |
| `--ctp-yellow` | `#f9e2af` | em（斜体） |
| `--ctp-green` | `#a6e3a1` | GoodItem |
| `--ctp-red` | `#f38ba8` | BadItem |
| `--ctp-lavender` / `--ctp-blue` / `--ctp-sapphire` / `--ctp-teal` / `--ctp-maroon` / `--ctp-flamingo` / `--ctp-rosewater` | 各公式値 | 予約（未使用、拡張用） |

## コンポーネント

`GoodItem` / `BadItem` を使うと、良い例・悪い例を色分けして表示できます。アイコン表示には `@iconify-json/mdi` が必要です。

```md
<GoodItem>これは良い例です</GoodItem>
<BadItem>これは悪い例です</BadItem>
```
