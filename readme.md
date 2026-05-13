
# 安裝task(啟動taskfile)
```bash
sh -c "$(curl -ssL https://taskfile.dev/install.sh)" -- -d -b /tmp && sudo mv /tmp/task /usr/local/bin/task && task --version
```
# 獲取 Gemini API Key
1. 開啟 [Google AI Studio](https://aistudio.google.com/)。
2. 使用 Google 帳號登入。
3. 點擊左側選單的 **「Get API key」**。
4. 點擊 **「Create API key」** (若無現有專案，選擇 "Create API key in new project")。
5. 複製 金鑰字串。

### 2. 環境配置
在專案根目錄建立 `.env.task` 檔案，並填入你的金鑰：

# 操作
- /add 增加某一檔案，增加token使用量，可重新讀取檔案內容，如果是aider改的不必再更新內容
- /drop 刪除某一檔案，減少token使用量
- /clear 重置context，減少token使用量
- /refresh 讓aider 重新讀取檔案內容
### 即使 aider 尊重.gitignore 但依然會將其中檔案加入 索引中，導致費用的提升，請加入.aiderignore排除。
