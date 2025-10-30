# 💡 Git Day 2：建立與操作本地倉庫
> 日期：2025-10-30  
> 學習主題：初始化本地 Git 倉庫、版本追蹤、提交變更、檢視歷史

---

## 🧭 學習目標
- 建立新的 Git 本地倉庫  
- 新增與提交檔案版本  
- 查看提交歷史與版本差異  

---

## 🧱 1. 建立新的本地倉庫

在專案資料夾中初始化 Git：

```bash
# 建立資料夾
mkdir git-demo
cd git-demo

# 初始化 Git
git init

# 檢查狀態
git status
```

> ✅ 結果：顯示「Initialized empty Git repository」代表建立成功。

---

## 🗂️ 2. 新增與提交檔案

建立一個新檔案並進行版本控制：

```bash
# 建立新檔案
echo "# My Git Project" > README.md

# 加入追蹤
git add README.md

# 提交
git commit -m "Add README file"
```

查看提交歷史：

```bash
git log
```

> ✅ 結果：可看到提交者、時間與提交訊息。

---

## 🔍 3. 追蹤修改與版本差異

編輯檔案後查看變更：

```bash
# 編輯 README.md
echo "This is my first Git project." >> README.md

# 檢查差異
git diff

# 提交修改
git add README.md
git commit -m "Update README with project description"
```

---

## 🧠 延伸學習
- `git status`：查看目前工作目錄與暫存區狀態  
- `git log --oneline`：以簡短格式顯示歷史紀錄  
- `git diff HEAD~1`：比較上一個提交的差異  

---

## 💻 VS Code 實作練習
1. 在 VS Code 開啟 `git-demo` 專案資料夾  
2. 透過內建的 **Source Control** 面板進行 `Stage` 與 `Commit`  
3. 使用 Terminal 執行 `git log` 與 `git diff`  
4. 試著建立第二個檔案（如 `notes.txt`）並提交

---

## 🪄 挑戰任務
建立一個新的 Git 專案，包含至少兩次提交，並觀察每次版本的差異：

```bash
git log --oneline
git diff HEAD~1 HEAD
```

---

## ✨ 今日學習反思
- 今天我學會了如何初始化 Git 專案與進行版本提交。  
- 我了解了「工作目錄、暫存區、提交歷史」三者的關係。  
- 下一步我想更熟悉 `git reset` 與 `git checkout` 的用途。

---

🏁 **下一堂課預告：Day 3 - 理解 Git 工作流程與分支操作（Branch）**
