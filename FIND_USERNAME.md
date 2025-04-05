# 如何找到你的 GitHub 用戶名

請按照以下步驟找到你的確切 GitHub 用戶名：

## 方法一：查看個人資料

1. 登入 GitHub 網站 (https://github.com)
2. 點擊右上角的頭像
3. 從下拉選單中選擇 "Your profile"（您的個人資料）
4. 在打開的頁面中，查看瀏覽器地址欄
   - 地址將顯示為 `https://github.com/你的用戶名`
   - 這個 "你的用戶名" 就是您的確切 GitHub 用戶名

## 方法二：查看設定頁面

1. 登入 GitHub 網站
2. 點擊右上角的頭像
3. 從下拉選單中選擇 "Settings"（設定）
4. 在左側導航欄中，點擊 "Emails"
5. 在頁面頂部，您可能會看到您的用戶名顯示

## 方法三：檢查 GitHub Pages URL

如果您之前有使用過 GitHub Pages：

1. 登入 GitHub 網站
2. 前往您之前創建的任何項目的設定頁面
3. 在左側導航欄中點擊 "Pages"
4. 查看 "Your site is live at https://您的用戶名.github.io/..."

確認您的確切用戶名後，請使用這個用戶名更新您的 Git 遠端儲存庫 URL：

```bash
git remote remove origin
git remote add origin https://github.com/您的確切用戶名/snake_game_web.git
```

這樣您就可以成功將代碼推送到 GitHub，並正確部署 GitHub Pages。 