# PDFリンク集

PDFを `/pdfs/` 配下に増やしていくための、GitHub Pages向けリポジトリ構成です。

## 公開URLのイメージ

GitHub Pagesのプロジェクトサイトの場合：

```text
https://<owner>.github.io/<repository>/pdfs/kakudo-kaidan-memo.pdf
```

独自ドメインを設定した場合：

```text
https://<your-domain>/pdfs/kakudo-kaidan-memo.pdf
```

## 階層

```text
/
├─ index.html
├─ README.md
├─ data/
│  └─ pdfs.json
├─ pdfs/
│  ├─ index.html
│  └─ kakudo-kaidan-memo.pdf
└─ assets/
   └─ images/
      ├─ 01.png
      ├─ 02.png
      └─ ...
```

## PDFを追加する手順

1. PDFを `/pdfs/` に置く
2. ファイル名はURL用に英数字・ハイフン推奨
3. `/data/pdfs.json` に1件追加する
4. `index.html` 側には自動反映される

## pdfs.json の追加例

```json
{
  "title": "資料タイトル",
  "description": "資料の説明",
  "file": "pdfs/sample.pdf",
  "category": "カテゴリ",
  "date": "2026-05-31",
  "tags": ["タグ1", "タグ2"]
}
```

## メモ

- GitHub Pagesでは `index.html` が入口になります。
- `/pdfs/xxx.pdf` のような固定URLでPDFを直接開けます。
- 日本語ファイル名も使えますが、公開URLが長くなるため英数字スラッグ推奨です。
