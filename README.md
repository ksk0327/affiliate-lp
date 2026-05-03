# affiliate-lp

初心者女性向けアフィリエイトLP。シンプルなHTML/CSSのみで構成。GitHub Pagesでそのまま公開可能。

---

## ファイル構成

```
affiliate-lp/
  ├ index.html   # メインのLPページ
  ├ style.css    # スタイルシート
  └ README.md    # このファイル
```

---

## GitHub Pagesで公開する手順

1. リポジトリページ →「Settings」タブ
2. 左メニュー「Pages」
3. Source: 「Deploy from a branch」
4. Branch: `main` / `/ (root)` を選択
5. 「Save」

数分後に `https://ksk0327.github.io/affiliate-lp/` で公開される。

---

## アフィリエイトリンクの差し替え方

`index.html` 内の `<!-- ▼ 差し替え箇所 -->` コメントを目印に `href` を書き換える。

差し替え箇所は計4カ所：
- 商品A（NO.1）
- 商品B（NO.2）
- 商品C（NO.3）
- CTAボタン

---

## 商品情報の編集方法

`index.html` の各 `<article class="card">` ブロックを編集する。

| 変更したい内容 | 対象タグ |
|---|---|
| 商品名 | `<h3 class="card__name">` |
| タグ（特徴） | `<span class="tag">` |
| 説明文 | `<p class="card__desc">` |

---

## カスタマイズ

`style.css` 冒頭の `:root` ブロックで色・余白を一元管理。

```css
:root {
  --color-bg: #ffffff;   /* 背景色 */
  --color-text: #1a1a1a; /* 本文色 */
  --color-btn: #1a1a1a;  /* ボタン色 */
  --max-width: 480px;    /* コンテンツ最大幅 */
}
```

---

## 注意事項

- アフィリエイトASPの規約に従って運用すること
- フッターのアフィリエイト表記は必ず残す（景品表示法・ASP規約対応）
- 外部リンクには `rel="noopener noreferrer"` を付与済み（セキュリティ対策）
