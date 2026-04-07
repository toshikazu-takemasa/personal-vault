# personal-vault

portal-app（個人プロファイル）のデータリポジトリ。

## 構造

```
vault/
  diary/        日記 (YYYY-MM-DD.md)
  knowledge/    ナレッジ・学習記録
  config.json   クイックリンク・チェックリスト設定
```

## portal-app との連携

portal-app の個人プロファイル設定:

| 項目 | 値 |
|---|---|
| `github_repo` | `toshikazu-takemasa/personal-vault-` |
| `github_branch` | `main` |
| `diary_path` | `vault/diary` |
| `config_path` | `vault/config.json` |

## データ形式

- **日記**: `vault/diary/YYYY-MM-DD.md`（Markdown）
- **ナレッジ**: `vault/knowledge/タイトル.md`（Markdown）
- **設定**: `vault/config.json`（portal-app の PortalConfig 型に準拠）
