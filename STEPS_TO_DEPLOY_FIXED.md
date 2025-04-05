# 修正的部署步驟

## 第一步：創建 GitHub 儲存庫

1. 訪問 [GitHub](https://github.com) 並登入您的帳戶
2. 點擊右上角的 "+" 符號，選擇 "New repository"
3. 在 "Repository name" 欄位中輸入 `snake_game_web`
4. 將儲存庫設為 "Public"
5. 不要勾選 "Initialize this repository with a README"
6. 點擊 "Create repository" 按鈕

## 第二步：設定 Git 使用者資訊（如果尚未設定）

```bash
git config --global user.name "您的姓名"
git config --global user.email "您的email@example.com"
```

## 第三步：重新連接遠端儲存庫

如果遇到「Repository not found」錯誤，請確保您在 GitHub 上創建了儲存庫，並且使用正確的用戶名。如果您之前設定的遠端儲存庫 URL 不正確，請移除並重新添加：

```bash
# 移除現有的遠端儲存庫連接
git remote remove origin

# 添加新的遠端儲存庫連接（請替換為您的實際 GitHub 用戶名）
git remote add origin https://github.com/您的GitHub用戶名/snake_game_web.git
```

## 第四步：推送到 GitHub

```bash
git branch -M main
git push -u origin main
```

## 第五步：設置 GitHub Pages

1. 在 GitHub 上前往您的 snake_game_web 儲存庫
2. 點擊 "Settings" 標籤
3. 在左側導航欄中點擊 "Pages"
4. 在 "Source" 部分下，選擇 "Deploy from a branch"
5. 在 "Branch" 選擇器中選擇 "main"，並將文件夾設置為 "/ (root)"
6. 點擊 "Save" 按鈕

## 第六步：訪問您的網站

幾分鐘後，您的網站將可通過以下 URL 訪問：

```
https://您的GitHub用戶名.github.io/snake_game_web/
```

您現在可以將此鏈接分享給任何人，讓他們在線上遊玩您的貪食蛇遊戲了！

## 常見問題解決

### 錯誤：src refspec main does not match any

這通常表示您還沒有創建任何提交。確保您已經添加並提交了文件：

```bash
git add .
git commit -m "初始提交"
```

### 錯誤：remote: Repository not found

這表示 GitHub 上找不到您指定的儲存庫。請確保：
1. 您已經在 GitHub 上創建了儲存庫
2. 您使用了正確的 GitHub 用戶名
3. 儲存庫名稱拼寫正確
4. 您已正確設定遠端儲存庫 URL 