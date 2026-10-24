# gggのポッドキャスト — Podcast Site

gggのポッドキャストをまとめた静的サイト。ビルド不要のプレーンな HTML/CSS で構成されています。
番組ごとにセクションを持ち、現在は次の1番組を配信中です。

- **神椿観測室**（KAMITSUBAKI STUDIO ファンポッドキャスト）
  - `episodes/ep1.mp3` — #1 神椿の現在地、二千二十六年秋（3:14）
  - `episodes/ep2.mp3` — #2 幸祜特集（6:10）

- `index.html` — 番組ハブ＋エピソード一覧ページ（新しい順）
- `style.css` — スタイル
- `feed.xml` — ポッドキャスト用 RSS フィード（enclosure 付き）

## 公開先

- 本番URL: https://podcast.0g0.xyz/（Cloudflare Pages + カスタムドメイン）
- フィード: https://podcast.0g0.xyz/feed.xml
- リポジトリ: https://github.com/g-kari/podcast

## 新しいエピソードの追加手順

1. `episodes/epN.mp3` を追加する。
2. `index.html` の該当番組セクションの先頭にエピソード記事を追加する。
3. `feed.xml` に `<item>` を追加し、`lastBuildDate` を更新する。
4. Cloudflare Pages へデプロイする（Direct Upload または git 連携）。
