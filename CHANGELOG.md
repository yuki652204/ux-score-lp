# Changelog

All notable changes to UX Score LP will be documented here.

## [1.0.0.0] - 2026-05-22

### Added
- インタラクティブデモウィジェットをヒーローセクションに埋め込み: URLを入力して「診断スタート」を押すと2.5秒のローディング後にスコアサークルが0→78にカウントアップし、次元バーが順番に伸びる3ステートアニメーション
- スコアサークル: SVGアーク + `requestAnimationFrame` による ease-out cubic アニメーション
- 「結果URLをコピー」ボタン: `navigator.clipboard` API でモック共有URLを生成・コピー
- 「詳細レポートを受け取る」ボタン: コンタクトセクションへのスムーズスクロール
- 「← 別のURLで試す」リセットリンク
- gstack スキルルーティングルールを `CLAUDE.md` に追加

### Changed
- ヒーローCTA「お問い合わせ・デモ依頼」→「無料で診断してみる →」に変更、デモウィジェットへの直接誘導
- 課題セクションのアイコン: 絵文字（🕐📊🔁）→ カスタムSVGアイコンに置き換え（AIスロップ排除）
- ナビリンクに縦方向パディング追加（タッチターゲット44px確保）
- `@media (prefers-reduced-motion: reduce)` 対応追加、アニメーション全無効化
- アクションボタンから絵文字を除去してプレーンテキストに統一
