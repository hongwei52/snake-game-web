# GitHub 身份驗證方式

從 2021 年 8 月 13 日起，GitHub 不再支持使用密碼進行身份驗證。您需要使用以下方式之一進行身份驗證：

## 1. 使用個人訪問令牌 (PAT)

### 創建個人訪問令牌步驟：

1. 登入 GitHub 帳戶
2. 點擊右上角您的頭像，選擇 "Settings"（設定）
3. 在左側導航欄中，點擊 "Developer settings"（開發者設定）
4. 在左側導航欄中，點擊 "Personal access tokens"（個人訪問令牌），然後選擇 "Tokens (classic)"
5. 點擊 "Generate new token"（生成新令牌），然後選擇 "Generate new token (classic)"
6. 在 "Note" 欄位中，給令牌一個描述性名稱，如 "Snake Game Web Deploy"
7. 設定令牌過期時間（建議選擇 30 天或 60 天）
8. 勾選 "repo" 權限（這允許您完全訪問儲存庫）
9. 點擊 "Generate token"（生成令牌）
10. **重要：** 複製顯示的令牌，這是您唯一能看到它的機會

### 使用個人訪問令牌：

當 Git 提示您輸入密碼時，請輸入您剛剛創建的個人訪問令牌而不是您的 GitHub 密碼。

```bash
git push -u origin main
```

系統會提示您輸入用戶名和密碼：
- 用戶名：您的 GitHub 用戶名
- 密碼：貼上您的個人訪問令牌

## 2. 使用 SSH 密鑰

另一種方法是使用 SSH 密鑰進行身份驗證：

1. 生成 SSH 密鑰對
2. 將公鑰添加到您的 GitHub 帳戶
3. 使用 SSH URL 連接到 GitHub 儲存庫

```bash
git remote remove origin
git remote add origin git@github.com:您的GitHub用戶名/snake_game_web.git
git push -u origin main
```

## 3. 使用 GitHub CLI

您也可以使用 GitHub CLI 進行身份驗證：

1. 安裝 GitHub CLI
2. 運行 `gh auth login` 命令進行身份驗證
3. 按照提示操作

完成身份驗證後，您就可以順利推送代碼到 GitHub 了。 