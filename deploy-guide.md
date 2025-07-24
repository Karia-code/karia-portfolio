# Karia Portfolio 部署指南

## 🚀 推薦方案：Netlify + 您的 karia.store 域名

### 🎯 方法一：直接拖拽（最快）
1. 登入您的 Netlify 帳號
2. 在儀表板找到 "Drag and drop" 部署區域
3. 將整個 `karia-portfolio` 資料夾拖拽進去
4. 等待部署完成（約1-2分鐘）
5. 獲得臨時網址如：`https://random-name-123456.netlify.app`

### 🔄 方法二：通過 GitHub（推薦給開發者）
1. 在 GitHub 建立新的 repository 叫 `karia-portfolio`
2. 上傳所有檔案到 GitHub
3. 在 Netlify 點擊 "New site from Git"
4. 連接您的 GitHub repository
5. 自動部署 + 未來更新時自動重新部署

### 🏷️ 連接您的 karia.store 域名（立即設置）：

#### ✅ 在 Netlify 設定域名：
1. **在您的 Netlify 網站儀表板**，點擊您剛部署的網站
2. **點擊 "Domain settings"** 或 "Set up a custom domain"
3. **點擊 "Add custom domain"**
4. **輸入 `karia.store`** 並點擊 "Verify"
5. **Netlify 會顯示 DNS 設定資訊**，類似這樣：
   ```
   Type: A
   Name: @ (或 karia.store)
   Value: 75.2.60.5 (Netlify 的 IP)
   
   Type: CNAME  
   Name: www
   Value: your-site-name.netlify.app
   ```

#### 🔧 現在立即在 Wix 修改 DNS 設定：

**步驟 1：獲取 Netlify DNS 資訊**
1. 在 Netlify 點擊 karia.store 旁的 "Options" 
2. 查看需要設置的 DNS 記錄（通常是）：
   ```
   A Record: @ (或空白) → 75.2.60.5
   CNAME: www → prismatic-cendol-1da3c1.netlify.app
   ```

**步驟 2：登入 Wix 修改 DNS**
1. **登入您的 Wix 帳戶**
2. **前往 "我的帳戶" > "域名管理"**
3. **找到 karia.store，點擊 "管理 DNS"**
4. **編輯或添加以下記錄**：
   - **A 記錄**: Name=@ (或留空), Value=75.2.60.5
   - **CNAME 記錄**: Name=www, Value=您的.netlify.app域名

**步驟 3：等待生效**
- DNS 變更需要 **1-24 小時**生效
- 可以用 [whatsmydns.net](https://www.whatsmydns.net) 檢查進度
- 生效後 Netlify 會自動生成 SSL 憑證

#### ⏰ 等待生效：
- DNS 變更需要 **1-24 小時**才會完全生效
- 可以用 [whatsmydns.net](https://www.whatsmydns.net) 檢查進度
- Netlify 會自動為 karia.store 生成 SSL 憑證

### ⚠️ 重要提醒：
- **保留 Wix 域名註冊**：不要轉移域名本身
- **只修改 DNS 設定**：讓域名指向新的主機
- **備份 Wix 設定**：記錄原本的 DNS 設定以防需要恢復

## 🔧 部署前檢查清單

- [x] 所有檔案都在同一個資料夾
- [x] index.html 是主檔案
- [x] 所有連結都是相對路徑
- [x] 圖片和資源檔案都正確載入
- [x] 語言切換功能正常
- [x] 響應式設計在手機上正常

## 📝 需要的檔案：
- index.html ✓
- style.css ✓  
- script.js ✓

## 🌐 其他選擇：

### GitHub Pages：
1. 在 GitHub 建立新 repository
2. 上傳所有檔案
3. Settings > Pages > Deploy from branch > main
4. 網址：`https://yourusername.github.io/repository-name`

### Vercel：
1. 到 [vercel.com](https://vercel.com)
2. 點擊 "New Project"
3. 上傳檔案或連接 GitHub
4. 網址：`https://project-name.vercel.app`

## � 升級到 GitHub 管理（強烈推薦）

### 為什麼要使用 GitHub？
1. **版本控制**：追蹤所有代碼變更歷史
2. **自動部署**：推送代碼後自動更新網站
3. **協作開發**：可以邀請其他開發者
4. **備份安全**：代碼永遠不會丟失
5. **專業形象**：展示您的開發能力

### 🎯 立即升級步驟：

#### 步驟 1：創建 GitHub Repository
1. **前往 [GitHub](https://github.com)**，登入您的帳號
2. **點擊右上角 "+" → "New repository"**
3. **Repository 名稱**: `karia-portfolio`
4. **設為 Public**（展示您的作品）
5. **點擊 "Create repository"**

#### 步驟 2：上傳您的代碼
```bash
# 在您的 karia-portfolio 資料夾中執行：
git init
git add .
git commit -m "Initial commit: Karia Portfolio"
git branch -M main
git remote add origin https://github.com/您的用戶名/karia-portfolio.git
git push -u origin main
```

#### 步驟 3：連接 Netlify 到 GitHub
1. **在 Netlify 點擊 "New site from Git"**
2. **選擇 "GitHub"** 並授權
3. **選擇您的 `karia-portfolio` repository**
4. **Build settings**:
   - Build command: 留空
   - Publish directory: 留空（根目錄）
5. **點擊 "Deploy site"**

#### 步驟 4：自動部署設定
- **以後任何代碼變更**，只需：
  ```bash
  git add .
  git commit -m "更新描述"
  git push
  ```
- **Netlify 會自動重新部署！**

### 🎁 GitHub 管理的額外好處：

1. **Portfolio 展示**：
   - GitHub profile 展示您的項目
   - 可以添加 README.md 說明

2. **Issues 管理**：
   - 追蹤 bugs 和新功能
   - 客戶可以直接報告問題

3. **Branches 功能**：
   - 測試新功能不影響主網站
   - 可以創建 `dev` 分支測試

4. **GitHub Pages 備選**：
   - 如果需要可以啟用 GitHub Pages
   - 雙重保障

### 💼 專業工作流程：
```
開發 → Git Commit → Push to GitHub → Netlify 自動部署 → 網站更新
```

## �💡 專業建議：

1. **使用您的 karia.store 域名**：完美的品牌域名！
2. **保持域名在 Wix**：避免轉移複雜性
3. **SSL 憑證**：Netlify 會自動為 karia.store 提供免費 HTTPS
4. **效能優化**：CDN 加速讓全球訪問更快
5. **SEO**：部署後記得提交 karia.store 到 Google Search Console
6. **GitHub 管理**：專業的代碼管理和自動部署

## 📧 Email 設定：
- 如果您有使用 Wix 的 Email 服務，DNS 修改後可能需要重新設定
- 建議先確認是否有使用 @karia.store 的郵箱

## 🆘 如果遇到問題：

- 檢查瀏覽器開發者工具的錯誤訊息
- 確認所有檔案路徑正確
- 測試語言切換功能
- 在手機上測試響應式設計
