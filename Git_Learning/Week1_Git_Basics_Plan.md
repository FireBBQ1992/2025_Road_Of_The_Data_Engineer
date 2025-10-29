# 🗓 Week 1：Git 基礎篇學習計畫
> 學習來源：《完全學會 Git, GitHub, Git Server 的 24 堂課》  
> 目標：在 7 天內掌握 Git 的核心概念與本地版本控制操作  
> 開始日期：2025-10-29
> 開發環境：macOS + VS Code
---

## 📘 Day 1：了解 Git 與版本控制的基本概念
### 🎯 學習重點
- 什麼是版本控制（Version Control）
- 為什麼需要 Git
- Git 的運作原理（快照 vs 差異儲存）
- 常見版本控制模型（集中式 vs 分散式）

### 💻 VS Code 實作練習
```bash
git --version
mkdir git-practice && cd git-practice
git init
echo "# My First Git Repo" > README.md
git add README.md
git commit -m "Initial commit"
```

### ✍️ 學習反思
> 認識版本控制的重要性與 Git 的核心設計理念。

---

## 📘 Day 2：Git 的架構與資料儲存方式
### 🎯 學習重點
- Git 三大區域：Working Directory、Staging Area、Repository
- Git 的物件結構（blob、tree、commit）
- `.git` 資料夾內容介紹

### 💻 VS Code 實作練習
```bash
ls -a .git
git cat-file -p HEAD
```

### ✍️ 學習反思
> 探索 Git 內部結構，理解 commit 與檔案物件的關聯。

---

## 📘 Day 3：建立與操作本地版本庫
### 🎯 學習重點
- git init 與 git clone 的差異
- 基本提交流程（add → commit → log）
- 常見狀態命令（status、diff、log）

### 💻 VS Code 實作練習
```bash
git status
git diff
git log --oneline
```

### ✍️ 學習反思
> 熟悉日常開發中的基本 Git 操作流程。

---

## 📘 Day 4：理解 Git 的提交歷史
### 🎯 學習重點
- commit hash、HEAD、parent 的概念
- 查看提交歷史（log、show）
- 回朔與檢視舊版本（checkout）

### 💻 VS Code 實作練習
```bash
git log --graph --decorate --oneline
git show HEAD~1
git checkout HEAD~1
```

### ✍️ 學習反思
> 透過歷史檢視學習版本控制的威力。

---

## 📘 Day 5：Git 分支（Branch）概念
### 🎯 學習重點
- 為什麼要使用分支
- 建立、切換、刪除分支
- 分支的 HEAD 與 commit 指標關係

### 💻 VS Code 實作練習
```bash
git branch feature-login
git checkout feature-login
git branch -a
git switch main
```

### ✍️ 學習反思
> 理解分支的靈活性與並行開發的重要性。

---

## 📘 Day 6：合併分支與衝突解決
### 🎯 學習重點
- `git merge` 與 `git rebase` 差異
- 發生衝突的原因與解法
- 使用 VS Code 解決 merge conflict

### 💻 VS Code 實作練習
```bash
git merge feature-login
# 若出現衝突，開啟 VS Code 解決
code .
```

### ✍️ 學習反思
> 學會面對衝突並有效解決是團隊開發的關鍵。

---

## 📘 Day 7：Git Flow 與專案管理實務
### 🎯 學習重點
- 常見開發流程（Git Flow、Feature Branch Workflow）
- 命名規範（feature/、hotfix/、release/）
- 為第二週連線 GitHub 打下基礎

### 💻 VS Code 實作練習
```bash
git branch develop
git checkout develop
git merge main
```

### ✍️ 學習反思
> 建立團隊開發思維，為遠端同步做好準備。

---

## ✅ Week 1 學習成果
- 熟悉 Git 的三區架構  
- 能建立本地倉庫與進行提交  
- 理解分支操作與合併流程  
- 為 GitHub 遠端同步做好準備

---
📦 **下一步建議**
👉 進入 Week 2：GitHub 遠端倉庫、SSH Key 與多人協作實作
