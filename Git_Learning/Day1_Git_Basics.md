#  Day 1：了解 Git 與版本控制的基本概念
> Week 1｜Git 基礎篇  
> Date：2025-10-29  
> DEV：macOS + VS Code
> Author : Johnson Chen
---


### 1️⃣ 為什麼需要版本控制（Version Control）？
- 在專案開發過程中，版本控制能幫助我們追蹤、回復、協作。
- 沒有版本控制時的混亂：
  ```
  report_v1.docx
  report_v2.docx
  report_final.docx
  report_final_final.docx
  ```
- 有了 Git，你可以：
  - 追蹤誰改了什麼
  - 隨時回復到過去版本
  - 與他人同步進度
  - 保留完整歷史紀錄

---

### 2️⃣ Git 是什麼？
- Git 是 **分散式版本控制系統（Distributed Version Control System）**
- 由 Linus Torvalds（Linux 之父）在 2005 年開發。
- 每個開發者都有完整歷史，不依賴中央伺服器。
- 優點：高速、離線可用、安全。

---

### 3️⃣ Git 的版本控制方式：快照（Snapshot）
- SVN 儲存「差異（Diff）」；Git 儲存「快照（Snapshot）」
- 每次 commit 是當前專案完整的狀態
- 若檔案沒變，Git 會指向上一版本相同的檔案

```
Commit A → Commit B → Commit C
  |           |           |
snapshot1   snapshot2   snapshot3
```

---

## 💻 二、VS Code 實作練習（macOS 環境）

### 🔧 Step 1：確認 Git 是否安裝
```bash
git --version
```
若尚未安裝：
```bash
brew install git
```

---

### 🏗 Step 2：建立練習資料夾
```bash
mkdir git-practice
cd git-practice
```

---

### 🧱 Step 3：初始化 Git 倉庫
```bash
git init
```
建立 `.git` 隱藏資料夾，Git 用來儲存版本紀錄。

---

### 📝 Step 4：建立第一個檔案
```bash
echo "# My First Git Repo" > README.md
```

---

### ✅ Step 5：加入追蹤並提交
```bash
git add README.md
git commit -m "Initial commit"
```

---

### 🔍 Step 6：檢查提交紀錄
```bash
git log --oneline
```
範例輸出：
```
e3a1d2f (HEAD -> main) Initial commit
```

---

## 💡 三、Git 的三個區域

| 區域 | 說明 | 指令 |
|------|------|------|
| Working Directory | 目前編輯的檔案 | `git status` |
| Staging Area | 準備提交的檔案 | `git add` |
| Repository | 已提交的版本歷史 | `git commit` |

流程圖：
```
工作目錄 → 暫存區 → 儲存庫
   (add)      (commit)
```

---

## 🧩 四、延伸挑戰
1. 嘗試修改 README.md 新增一行文字，再進行一次 commit。  
2. 使用 `git log --oneline` 觀察版本變化。  
3. 用一句話解釋「為什麼 Git 是分散式？」。

---

## ✍️ 五、學習反思
> 今天學會了建立 Git 倉庫與第一次提交。  
> 明天將深入 `.git` 內部結構，理解 Git 如何保存 commit 與檔案快照。

---

📦 **下一步**
👉 [Day 2：Git 的架構與資料儲存方式]()
