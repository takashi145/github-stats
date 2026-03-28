# GitHub Stats

自分の公開リポジトリの使用言語割合を集計し、`langs.json` を自動更新します。
（フォークしたリポジトリや Organization のリポジトリは対象外です）

## セットアップ

1. このリポジトリをフォーク
2. Actions タブで GitHub Actions を有効化

毎週日曜に自動実行されます。実行スケジュールを変更したい場合は [`.github/workflows/update-langs.yml`](.github/workflows/update-langs.yml) の `cron` を編集してください。

## 出力

`langs.json` に言語名と割合（%）が多い順で保存されます。

```json
[
  { "lang": "Python", "percent": 45.2 },
  { "lang": "TypeScript", "percent": 30.1 }
]
```
