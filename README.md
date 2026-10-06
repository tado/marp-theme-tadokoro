# marp-theme-tadokoro

Marp 用カスタムテーマ `tadokoro`。

## 使い方（VS Code）

ユーザー設定 `settings.json` に追加:

```json
"markdown.marp.themes": [
  "https://raw.githubusercontent.com/tado/marp-theme-tadokoro/main/tadokoro.css"
]
```

スライドのフロントマター:

```markdown
---
marp: true
theme: tadokoro
paginate: true
---
```

## サンプル

- [example.ja.md](example.ja.md)（日本語）
- [example.en.md](example.en.md)（English）

## 書式

| 書き方 | 表示 |
| --- | --- |
| `> テキスト` | ヒント枠（青） |
| `> > テキスト` | 注意枠（黄） |
| `<!-- _class: bigtxt -->` | 青背景・中央揃えの扉スライド |
| `<kbd>Ctrl</kbd>` | キー表示 |

## Marp CLI

```bash
npx @marp-team/marp-cli slide.md --theme-set path/to/tadokoro.css --pdf
```
