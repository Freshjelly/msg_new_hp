# 開発者向けドキュメント

## 📋 開発環境構築

### 必要な環境
- **ブラウザ**: Chrome 90+, Firefox 88+, Safari 14+, Edge 90+
- **ローカルサーバー**: Python, Node.js, または任意のHTTPサーバー
- **エディタ**: VS Code推奨（拡張機能: Live Server, Prettier）

### 推奨開発環境
```bash
# VS Code拡張機能
- Live Server
- Prettier - Code formatter
- Auto Rename Tag
- CSS Peek
- HTML CSS Support
```

## 🎨 コーディング規約

### HTML
- セマンティックなHTMLタグを使用
- アクセシビリティ（ARIA属性）を考慮
- BEMクラス命名規則を採用

### CSS
- CSS変数を活用した一貫性のあるデザイン
- モバイルファーストアプローチ
- Flexbox/Grid Layoutを積極的に使用

### JavaScript
- ES6+構文を使用
- クラスベースの構造化されたコード
- JSDocコメントによる型情報付与

## 📂 ディレクトリ詳細

### `/css/`
- `styles.css` - メインスタイルシート
- CSS変数による統一されたデザインシステム

### `/js/`
- `scripts.js` - メイン機能（タブ、ナビゲーション等）
- `analytics.js` - Google Analytics統合
- `image-optimization.js` - 画像最適化
- `structured-data.js` - SEO構造化データ

### `/assets/images/`
- 最適化された画像ファイル
- WebP形式推奨（フォールバック付き）

### `/seo/`
- `robots.txt` - 検索エンジンクローラー制御
- `sitemap.xml` - サイトマップ

## 🚀 デプロイメント

### 本番環境チェックリスト
- [ ] Google Analytics IDの設定
- [ ] Open Graph画像の正しいURL
- [ ] robots.txtの設定確認
- [ ] サイトマップの更新
- [ ] パフォーマンステスト実行
- [ ] アクセシビリティテスト実行

### パフォーマンス最適化
```bash
# 画像最適化例
npx imagemin *.{jpg,png} --out-dir=optimized --plugin=imagemin-webp
```

## 🔧 カスタマイズガイド

### カラーパレット変更
`css/styles.css`の`:root`内でCSS変数を変更：

```css
:root {
  --color-primary: #your-color;
  --color-secondary: #your-color;
}
```

### タブコンテンツの追加
1. HTMLにタブトリガーとパネルを追加
2. JavaScriptは自動的に新しいタブを検出

### フォーム送信先変更
`js/scripts.js`内の`handleFormSubmit`メソッドのURL変更：

```javascript
const response = await fetch('your-endpoint.php', {
```

## 📊 アナリティクス設定

### Google Analytics 4
`js/analytics.js`でトラッキングIDを設定：

```javascript
gtag('config', 'YOUR-GA-TRACKING-ID');
```

### カスタムイベント追跡
```javascript
// フォーム送信成功
window.msgAnalytics.trackFormSubmission('contact_form', true);

// タブ切り替え
window.msgAnalytics.trackTabChange('kampo-ai');
```

## 🐛 トラブルシューティング

### よくある問題

**Q: タブが正しく動作しない**
A: `data-tab`と`data-panel`属性が正しく設定されているか確認

**Q: スタイルが反映されない**
A: ブラウザキャッシュをクリアしてファイルパスを確認

**Q: モバイルメニューが開かない**  
A: Lucide IconsのCDNが読み込まれているか確認

## 📈 パフォーマンス目標

- **Lighthouse Score**: 90+
- **First Contentful Paint**: < 1.5s
- **Largest Contentful Paint**: < 2.5s
- **Cumulative Layout Shift**: < 0.1

## 🔄 更新手順

1. 変更をテスト環境で確認
2. パフォーマンステスト実行
3. Git commit & push
4. 本番環境デプロイ
5. 動作確認テスト

---

**連絡先**: 技術的な質問は開発チームまでお問い合わせください。