# slidev-theme-catppuccin-latte

[Catppuccin Latte](https://github.com/catppuccin/catppuccin) のカラーパレットを使った [Slidev](https://sli.dev) 用のライトテーマです。姉妹テーマに [slidev-theme-catppuccin-mocha](../theme-catppuccin-mocha)（ダーク版）があります。

## インストール

`slides.md` の frontmatter で指定します。

```yaml
---
theme: catppuccin-latte
---
```

ローカルパッケージとして参照する場合は、プレゼンテーション側の `package.json` に以下を追加してください。

```json
{
  "dependencies": {
    "slidev-theme-catppuccin-latte": "file:../packages/theme-catppuccin-latte"
  }
}
```

## カラーパレット

Catppuccin Latte 公式の26色トークンを `--ctp-<name>` という命名規則の CSS カスタムプロパティとして定義しています。

| 変数 | HEX | 用途 |
| --- | --- | --- |
| `--ctp-base` | `#eff1f5` | 背景 |
| `--ctp-mantle` | `#e6e9ef` | cover レイアウトのグラデーション |
| `--ctp-crust` | `#dce0e8` | 予約 |
| `--ctp-surface0` | `#ccd0da` | 予約 |
| `--ctp-surface1` | `#bcc0cc` | h1 下線、code/pre 背景、テーブルヘッダー背景 |
| `--ctp-surface2` | `#acb0be` | 予約 |
| `--ctp-overlay0` | `#9ca0b0` | pre 枠線、cover の補足テキスト |
| `--ctp-overlay1` / `--ctp-overlay2` | `#8c8fa1` / `#7c7f93` | 予約 |
| `--ctp-subtext0` / `--ctp-subtext1` | `#6c6f85` / `#5c5f77` | 予約 |
| `--ctp-text` | `#4c4f69` | 本文の文字色 |
| `--ctp-mauve` | `#8839ef` | プライマリカラー（h1、リストマーカー、テーブル強調） |
| `--ctp-pink` | `#ea76cb` | セカンダリカラー（h2） |
| `--ctp-sky` | `#04a5e5` | h3、リンク、テーブルヘッダー文字 |
| `--ctp-peach` | `#fe640b` | strong（太字） |
| `--ctp-yellow` | `#df8e1d` | em（斜体） |
| `--ctp-green` | `#40a02b` | GoodItem |
| `--ctp-red` | `#d20f39` | BadItem |
| `--ctp-lavender` / `--ctp-blue` / `--ctp-sapphire` / `--ctp-teal` / `--ctp-maroon` / `--ctp-flamingo` / `--ctp-rosewater` | 各公式値 | 予約（未使用、拡張用） |

## コンポーネント

`GoodItem` / `BadItem` を使うと、良い例・悪い例を色分けして表示できます。アイコン表示には `@iconify-json/mdi` が必要です。

```md
<GoodItem>これは良い例です</GoodItem>
<BadItem>これは悪い例です</BadItem>
```
