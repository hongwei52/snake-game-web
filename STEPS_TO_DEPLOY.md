# 部署到 GitHub Pages 的步驟

## 第一步：創建 GitHub 儲存庫

1. 訪問 [GitHub](https://github.com) 並登入您的帳戶
2. 點擊右上角的 "+" 符號，選擇 "New repository"
3. 在 "Repository name" 欄位中輸入 `snake_game_web`
4. 將儲存庫設為 "Public"
5. 不要勾選 "Initialize this repository with a README"
6. 點擊 "Create repository" 按鈕

## 第二步：將本地儲存庫推送到 GitHub

在終端機中執行以下命令（請替換 YOUR_USERNAME 為您的 GitHub 用戶名）：

```bash
git remote add origin https://github.com/YOUR_USERNAME/snake_game_web.git
git branch -M main
git push -u origin main
```

## 第三步：設置 GitHub Pages

1. 在 GitHub 上前往您的 snake_game_web 儲存庫
2. 點擊 "Settings" 標籤
3. 在左側導航欄中點擊 "Pages"
4. 在 "Source" 部分下，選擇 "Deploy from a branch"
5. 在 "Branch" 選擇器中選擇 "main"，並將文件夾設置為 "/ (root)"
6. 點擊 "Save" 按鈕

## 第四步：訪問您的網站

幾分鐘後，您的網站將可通過以下 URL 訪問：

```
https://YOUR_USERNAME.github.io/snake_game_web/
```

您現在可以將此鏈接分享給任何人，讓他們在線上遊玩您的貪食蛇遊戲了！ 