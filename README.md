# 情報入門 授業サイト

北星学園大学「情報入門」（2026年度）の授業資料サイト。
MkDocs Material で構築し、GitHub Pages で公開している。

公開URL: https://aonoa68.github.io/joho-nyumon/

## 構成

```
joho-nyumon-site/
├── mkdocs.yml      … サイト設定・ナビゲーション
├── docs/           … 各回の授業資料（Markdown）
│   ├── index.md    … トップページ
│   ├── week02.md 〜 week14.md
│   └── ...
└── README.md
```

## ローカルでプレビュー

```bash
mkdocs serve
# → http://127.0.0.1:8000/ で確認
```

## 公開（更新）

```bash
mkdocs gh-deploy
# → ビルドして gh-pages ブランチに push、GitHub Pages に反映される
```

## 資料を追加・修正するとき

1. `docs/` の Markdown を編集（または新規追加）
2. 新規ページは `mkdocs.yml` の `nav:` にも追記
3. `mkdocs serve` でローカル確認
4. `mkdocs gh-deploy` で公開

## 注意

- このリポジトリは **公開**。学生の個人情報・成績・採点データ・他教員の教材・NDA資料は**絶対に置かない**こと。
- 置いてよいのは「学生に見せる授業資料」のみ。
