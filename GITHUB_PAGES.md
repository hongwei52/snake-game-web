# 不使用 Git 命令行部署到 GitHub Pages

如果您在使用 Git 命令行工具時遇到困難，可以直接在 GitHub 網站上上傳文件，這是一個更簡單的替代方案。

## 步驟一：創建 GitHub 儲存庫

1. 登入 GitHub 網站 (https://github.com)
2. 點擊右上角的 "+" 按鈕，選擇 "New repository"（新儲存庫）
3. 在 "Repository name"（儲存庫名稱）欄位中輸入 `snake_game_web`
4. 確保選擇 "Public"（公開）選項
5. 勾選 "Add a README file"（添加 README 文件）選項，這將初始化儲存庫
6. 點擊 "Create repository"（創建儲存庫）按鈕

## 步驟二：上傳文件

### 上傳 index.html 文件

1. 在您的儲存庫頁面，點擊 "Add file"（添加文件），然後選擇 "Upload files"（上傳文件）
2. 從您的電腦中選擇 `index.html` 文件進行上傳
3. 在 "Commit changes"（提交更改）部分，添加一個描述，如 "上傳貪食蛇遊戲網頁版文件"
4. 點擊 "Commit changes"（提交更改）按鈕

### 上傳其他文件（如果有）

以同樣的方式上傳任何其他需要的文件，如 CSS、JavaScript 文件等。

## 步驟三：啟用 GitHub Pages

1. 在您的儲存庫頁面，點擊 "Settings"（設定）標籤
2. 在左側導航欄中，點擊 "Pages"
3. 在 "Source"（源）部分下，選擇 "Deploy from a branch"（從分支部署）
4. 在 "Branch"（分支）選擇器中選擇 "main"，並將文件夾設置為 "/ (root)"
5. 點擊 "Save"（保存）按鈕
6. GitHub 將開始構建您的網站，這可能需要幾分鐘時間

## 步驟四：訪問您的網站

幾分鐘後，您的網站將可以通過以下 URL 訪問：

```
https://您的GitHub用戶名.github.io/snake_game_web/
```

您可以通過以下位置檢查部署狀態：

1. 在您的儲存庫頁面，點擊 "Settings"（設定）標籤
2. 在左側導航欄中，點擊 "Pages"
3. 您將看到一個綠色橫幅，顯示 "Your site is published at ..."（您的網站已發布在...）

## 更新網站

如果您想要更新網站，只需：

1. 在您的儲存庫頁面，找到要更新的文件
2. 點擊該文件進入查看模式
3. 點擊鉛筆圖標（編輯文件）
4. 進行您的更改
5. 點擊 "Commit changes"（提交更改）按鈕

每次提交更改後，GitHub Pages 都會自動重新部署您的網站。 