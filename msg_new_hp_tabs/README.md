# MSG株式会社 コーポレートサイト

## 🌐 プロジェクト概要
MSG株式会社の公式コーポレートサイトです。東洋医学×西洋医学×AIの融合により、健康の未来をデザインすることをミッションとしています。

### 🎯 ミッション
「Personal Health, Shared Future」をコンセプトに、誰もが健やかに生きられる社会の創造を目指しています。

## 📂 ディレクトリ構造

```
msg_new_hp_tabs/
├── 📄 index.html              # メインページ（タブ機能付き）
├── 📄 privacy-policy.html     # プライバシーポリシー
├── 📄 terms-of-service.html   # 利用規約
├── 🎨 styles.css              # スタイルシート
├── 🔧 scripts.js              # メインJavaScript（タブ機能含む）
├── 📊 analytics.js            # Google Analytics統合
├── 🖼️ image-optimization.js   # 画像最適化処理
├── 📋 structured-data.js      # 構造化データ（SEO用）
├── 📁 assets/                 # アセットファイル
│   └── images/
│       └── kentame.png        # 健タメロゴ
└── 📁 seo/                    # SEO関連ファイル
    ├── robots.txt             # クローラー設定
    └── sitemap.xml            # サイトマップ
```

## 🚀 主な機能

### 1. **タブ式ナビゲーション**
- スムーズなタブ切り替えによる事業紹介
- レスポンシブ対応のタブレイアウト
- アクセシビリティ対応（キーボードナビゲーション）

### 2. **事業紹介セクション**
- **KampoAI**: 東洋医学×AIによる健康相談サービス
- **ロイヤル漢方クラブ**: 個別化漢方医療の提供
- **Smart Functional Food**: 機能性食品の開発・販売

### 3. **SEO最適化**
- 構造化データ実装
- Open Graph & Twitter Card対応
- サイトマップ自動生成
- メタタグ最適化

### 4. **パフォーマンス最適化**
- 画像遅延読み込み（Lazy Loading）
- 最適化されたCSS/JS
- CDN活用による高速配信

## 🛠️ 技術スタック

| カテゴリー | 技術 |
|-----------|------|
| フロントエンド | HTML5, CSS3, Vanilla JavaScript |
| アイコン | Lucide Icons (CDN) |
| アナリティクス | Google Analytics 4 |
| SEO | Schema.org構造化データ |
| レスポンシブ | Flexbox, Grid Layout |

## 📱 対応デバイス

- ✅ デスクトップ（1920px〜）
- ✅ ラップトップ（1024px〜）
- ✅ タブレット（768px〜）
- ✅ スマートフォン（320px〜）

## 🔧 セットアップ方法

### 1. リポジトリのクローン
```bash
git clone -b feature/optimized-site-with-tabs https://github.com/Freshjelly/msg_new_hp.git
cd msg_new_hp
```

### 2. ローカルサーバーでの実行
#### Python使用の場合
```bash
python -m http.server 8000
# ブラウザで http://localhost:8000 にアクセス
```

#### Node.js使用の場合
```bash
npx http-server -p 8000
# ブラウザで http://localhost:8000 にアクセス
```

## 📊 Google Analytics設定

`analytics.js`内のトラッキングIDを自社のIDに変更してください：

```javascript
// analytics.js 内
gtag('config', 'YOUR-GA-TRACKING-ID');
```

## 🔍 SEO設定

### サイトマップ更新
`seo/sitemap.xml`を定期的に更新し、Google Search Consoleに送信してください。

### robots.txt設定
`seo/robots.txt`でクローラーのアクセス制御を行っています。必要に応じて編集してください。

## 📋 今後の改善予定

- [ ] 多言語対応（英語・中国語）
- [ ] ダークモード実装
- [ ] お問い合わせフォームのバックエンド統合
- [ ] ブログセクションの追加
- [ ] ニュースレター購読機能

## 📞 お問い合わせ

**MSG株式会社**
- 📍 所在地: 東京都渋谷区恵比寿南1-5-5 JR恵比寿ビル11F
- 📧 メール: info@msg-corp.co.jp
- 🌐 ウェブサイト: https://msg-corp.co.jp

## 📝 ライセンス

Copyright © 2025 MSG株式会社. All rights reserved.

---

最終更新日: 2025年8月11日