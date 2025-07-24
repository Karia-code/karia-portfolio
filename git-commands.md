# Karia Portfolio - GitHub 上傳指令

## 📋 上傳步驟

### 1. 首先確保您已經創建了 GitHub Repository
- 前往 https://github.com
- 點擊右上角 "+" → "New repository"
- Repository 名稱: `karia-portfolio`
- 設為 Public
- **不要** 勾選 "Add a README file"（因為我們已經有了）
- 點擊 "Create repository"

### 2. 在終端中執行以下命令

```bash
# 進入您的項目資料夾
cd "c:\Users\MyPC\Desktop\k0-website\karia-portfolio"

# 初始化 Git 倉庫
git init

# 添加所有文件
git add .

# 創建第一次提交
git commit -m "🎉 Initial commit: Karia Portfolio with bilingual support"

# 設置主分支名稱
git branch -M main

# 連接到您的 GitHub repository
git remote add origin https://github.com/Karia-code/karia-portfolio.git

# 推送到 GitHub
git push -u origin main
```

### 3. 完成後
- 在 GitHub 上查看您的 repository
- README.md 會自動顯示在頁面下方
- 您的項目就成功上線了！

## 🔄 以後更新代碼

當您修改了代碼，只需要執行：

```bash
git add .
git commit -m "描述您的更改"
git push
```

## 🚀 連接 Netlify 自動部署

1. 在 Netlify 儀表板點擊 "New site from Git"
2. 選擇 "GitHub" 並授權
3. 選擇您的 `karia-portfolio` repository
4. Build settings 保持默認（空）
5. 點擊 "Deploy site"
6. 部署完成後，在 Domain settings 中添加您的 karia.store 域名

這樣以後每次 push 到 GitHub，Netlify 都會自動更新您的網站！
