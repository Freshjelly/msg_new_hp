# MSG株式会社 公式ホームページ

MSG株式会社の公式コーポレートサイトのソースコードです。
GitHub Pages (プロジェクトページ: https://freshjelly.github.io/msg_new_hp/) で公開されています。

## プロジェクト構成

```
/                       # 配信ルート（GitHub Pages: プロジェクトページ）
├── msg_new_hp_tabs/    # メインサイト（タブ式ニュース版）
│   ├── index.html      # トップページ
│   ├── privacy-policy.html  # プライバシーポリシー  
│   ├── terms-of-service.html # 利用規約
│   ├── css/
│   │   └── styles.css  # メインスタイルシート
│   ├── js/
│   │   ├── scripts.js  # メインJavaScript
│   │   ├── analytics.js     # Google Analytics
│   │   ├── image-optimization.js # 画像最適化
│   │   └── structured-data.js    # 構造化データ
│   ├── assets/
│   │   └── images/
│   │       └── kentame.png      # 健タメ！ロゴ
│   ├── seo/
│   │   ├── robots.txt          # SEO用robots.txt
│   │   └── sitemap.xml         # サイトマップ
│   └── docs/
│       └── DEVELOPMENT.md      # 開発ドキュメント
├── msg_new_hp/         # 旧版サイト（参考用）
└── msg_cpnew/          # 開発用サイト（参考用）
```

## パス設計方針

GitHub Pages（プロジェクトページ）でのリンク切れ防止のため**相対パス（先頭 / を使わない）**に統一しています。

## ナビゲーション・フッターリンク

### ヘッダーナビ
- ホーム: `#hero`（ページ内リンク）
- ビジョン: `#vision`（ページ内リンク）
- 提供する価値: `#what-we-do`（ページ内リンク）
- サービス: `#services`（ページ内リンク）
- メディア: `#media`（ページ内リンク）
- ニュース: `#news`（ページ内リンク）
- 会社概要: `#company`（ページ内リンク）
- お問い合わせ: `#contact`（ページ内リンク）

### フッターリンク
- KampoAI: `#services`（ページ内リンク）
- ロイヤル漢方クラブ: `#services`（ページ内リンク）
- Smart Functional Food: `#services`（ページ内リンク）
- 健タメ！: `#media`（ページ内リンク）
- 会社概要: `#company`（ページ内リンク）
- 採用情報: `#careers`（ページ内リンク）
- ニュース: `#news`（ページ内リンク）
- **プライバシーポリシー**: `./privacy-policy.html`（相対パス）
- **利用規約**: `./terms-of-service.html`（相対パス）

### ポリシーページ
- プライバシーポリシー・利用規約から「ホームへ戻る」: `./index.html`（相対パス）

## 技術仕様

### フロントエンド
- HTML5 (セマンティックマークアップ)
- CSS3 (Flexbox/Grid、レスポンシブデザイン)
- JavaScript (ES6+、バニラJS)
- Lucide Icons（CDN）

### SEO対応
- 構造化データ（JSON-LD）
- Open Graph/Twitter Cards
- サイトマップ（XML）
- robots.txt
- 適切なメタタグ設定

### 機能
- レスポンシブデザイン対応
- スムーススクロール
- モバイルハンバーガーメニュー
- タブ式ニュースセクション
- ActiveCampaignお問い合わせフォーム連携
- Google Analytics 4対応
- 画像遅延読み込み（Lazy Loading）

## 開発・運用

### 開発環境セットアップ
1. リポジトリクローン:
   ```bash
   git clone git@github.com:Freshjelly/msg_new_hp.git
   ```

2. 開発サーバー起動:
   ```bash
   # Live Server等を使用
   # または Python簡易サーバー
   python -m http.server 8000
   ```

3. GitHub Pagesでの動作確認:
   - https://freshjelly.github.io/msg_new_hp/msg_new_hp_tabs/

### 運用方針
- **メインブランチ**: `main` - 本番環境（GitHub Pages自動デプロイ）
- **開発ブランチ**: `feature/*` - 機能開発用
- プルリクエストベースの開発フロー
- リポジトリルートからの配信（`docs/` フォルダを使わない運用）

### デプロイ
GitHub Pagesの自動デプロイにより、`main`ブランチへのpush時に自動的に本番環境に反映されます。

## ライセンス

© 2025 MSG株式会社. All rights reserved.

## お問い合わせ

MSG株式会社  
- ウェブサイト: https://freshjelly.github.io/msg_new_hp/msg_new_hp_tabs/
- Email: contact@msg-corp.co.jp