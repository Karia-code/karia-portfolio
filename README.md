# 🌟 Karia Portfolio

> 專業的雙語個人作品集網站，展示技術實力與設計美學

[![網站狀態](https://img.shields.io/website?url=https%3A%2F%2Fkaria.store)](https://karia.store)
[![部署狀態](https://api.netlify.com/api/v1/badges/YOUR_SITE_ID/deploy-status)](https://app.netlify.com/sites/YOUR_SITE_NAME/deploys)

## 🚀 網站預覽

**在線訪問**: [karia.store](https://karia.store)

### 主要特色
- 🌍 **雙語支持** - 中文/英文無縫切換
- 💰 **多幣別顯示** - USD/TWD 自動轉換
- 📱 **響應式設計** - 完美適配所有設備
- ✨ **現代 UI** - Glassmorphism 設計風格
- 🎨 **動畫效果** - 流暢的交互體驗
- 💾 **偏好記憶** - 語言選擇自動保存

## 🛠️ 技術棧

### 前端技術
- **HTML5** - 語義化結構設計
- **CSS3** - 現代樣式與動畫
  - Flexbox & Grid 布局
  - CSS Variables 主題系統
  - Glassmorphism 視覺效果
- **Vanilla JavaScript** - 純原生 JS 實現
  - ES6+ 語法
  - 模組化設計
  - 本地存儲管理

### 部署 & 工具
- **Netlify** - 自動化部署與 CDN
- **Git** - 版本控制
- **自定義域名** - karia.store
- **SSL/TLS** - 安全加密傳輸

## 📁 項目結構

```
karia-portfolio/
├── index.html          # 主頁面文件
├── style.css           # 樣式文件
├── script.js           # 腳本文件
├── deploy-guide.md     # 部署指南
└── README.md          # 項目說明
```

## 🎯 核心功能

### 1. 雙語國際化
- 一鍵切換中英文介面
- 所有內容完整翻譯
- 語言偏好持久化存儲

### 2. 專業展示
- **關於我**: CTO 背景與技術專長
- **服務項目**: 完整的技術服務清單
- **作品集**: 精選項目展示
- **聯繫方式**: 多種聯繫管道

### 3. 商業功能
- **定價系統**: 透明的服務定價
- **幣別轉換**: USD ↔ TWD 即時轉換
- **比較指南**: 服務方案對比

### 4. 用戶體驗
- **快速載入**: 優化的資源載入
- **直觀導航**: 清晰的頁面結構
- **互動反饋**: 豐富的 hover 效果
- **無障礙設計**: 符合 WCAG 標準

## 🚀 快速開始

### 本地開發
```bash
# 克隆項目
git clone https://github.com/YOUR_USERNAME/karia-portfolio.git

# 進入目錄
cd karia-portfolio

# 啟動本地服務器 (可選)
python -m http.server 8000
# 或使用 Node.js
npx serve .

# 在瀏覽器中打開
open http://localhost:8000
```

### 部署到 Netlify
1. Fork 這個項目到您的 GitHub
2. 在 Netlify 中連接 GitHub repository
3. 設置構建命令（留空）
4. 設置發布目錄（根目錄）
5. 點擊部署

## 🔧 自定義配置

### 修改個人信息
編輯 `index.html` 中的 `data-en` 和 `data-zh` 屬性：

```html
<!-- 例如修改姓名 -->
<h1 data-en="Your Name" data-zh="您的姓名">Karia</h1>

<!-- 修改服務項目 -->
<div data-en="Your Service" data-zh="您的服務">...</div>
```

### 調整定價
在 `script.js` 中修改匯率和價格：

```javascript
const exchangeRate = 31.5; // USD to TWD 匯率
// 修改服務價格...
```

### 更換配色方案
在 `style.css` 中修改 CSS 變量：

```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
    /* 其他顏色變量 */
}
```

## 📈 SEO 優化

- ✅ Meta 標籤完整設置
- ✅ Open Graph 社交媒體優化
- ✅ 結構化數據標記
- ✅ 語義化 HTML 結構
- ✅ 圖片 Alt 屬性
- ✅ 快速載入時間

## 🌐 瀏覽器支持

- ✅ Chrome (推薦)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ 移動端瀏覽器

## 📝 更新日誌

### v1.0.0 (2025-01-25)
- 🎉 初始版本發布
- ✨ 雙語支持系統
- 💰 幣別轉換功能
- 📱 響應式設計
- 🎨 Glassmorphism 視覺效果

## 🤝 貢獻指南

歡迎提交 Issue 和 Pull Request！

1. Fork 項目
2. 創建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打開 Pull Request

## 📄 許可證

本項目採用 MIT 許可證 - 查看 [LICENSE](LICENSE) 文件了解詳情

## 📧 聯繫方式

- **網站**: [karia.store](https://karia.store)
- **Email**: contact@karia.store
- **GitHub**: [@Karia-code](https://github.com/Karia-code)

## 🙏 致謝

- 設計靈感來自現代 Web 設計趨勢
- 使用了開源字體和圖標庫
- 感謝 Netlify 提供免費託管服務

---

⭐ 如果這個項目對您有幫助，請給一個 Star！

**Made with ❤️ by Karia**
