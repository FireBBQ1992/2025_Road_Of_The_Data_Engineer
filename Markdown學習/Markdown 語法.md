---
title: Markdown 語法
tags: [onboarding]

---

# 加入學習 Markdown 的行列吧！
如果您是 Markdown 的新手，而且剛開始探索 Markdown 的功能，本指南就是為您而寫。您將在此學習基本知識，從簡單的文字格式到建立清單等等。到最後，您將掌握所需的技巧，輕鬆寫出乾淨且有條理的文件。

Markdown 語法將寫在 `程式碼區塊` 中，以下展示一些常用的語法範例，讓我們開始吧！

# 指南概覽
- [Markdown 語法](#Markdown-語法)
- [文字格式](#文字格式)
- [表格](#表格)
- [筆記目錄](#筆記目錄)
- [切換編輯頁／檢視頁](#切換編輯頁／檢視頁)
- [瞭解更多HackMD使用方法](#瞭解更多HackMD使用方法)

## Markdown 語法

### 無序清單
語法: `- 無序清單`
- 無序清單
### 有序清單
語法: `1. 有序清單`
1. 有序清單
### 任務清單
語法: `- [ ] 任務清單`
- [ ] 任務清單

:::success
>[!Tip] 在行內按一下  <kbd>Tab</kbd> 即可增加縮排
>依照你的需求製作清單

1. 有序清單
    - 無序清單
2. 有序清單
    - [ ] 任務清單
:::

### 引用
語法: `> 引用`
> 引用
### 加上時間
語法: 輸入 `>[]` ，移動滑鼠到右側，就會出現選單（第二個選項）讓您在文件中插入當下的時間。

>[time=Wed, Oct 30, 2024 8:28 PM]

### 引用提醒
語法: 輸入 `>[!]` 並移動方向鍵至 `!` 右側將會出現引用提示的選單

>[!Note]註記

>[!Tip]提示

>[!Important]重要

>[!Warning]警示

>[!Caution]警告

### 色塊提醒

使用色塊來強調重要訊息，您只需要替換冒號 ``:::`` 後面的文字 ``info/success/warning/danger`` ，系統就會提供一個自動完成選單。


```
:::warning
文字 文字 文字
:::
```

:::warning
:warning: 警告
:::

:::danger
:radioactive_sign: 危險
:::

:::info
:information_source: 資訊
:::

:::success
 :100: 恭喜
:::

### 超連結
語法: `[連結名稱](URL)`
[連結名稱](URL)


## 文字格式
### 標題

在行首輸入 `#` 和一個空白，就會形成筆記標題. 每增加一個 `#` 就會成為第N層級的標題，最多六層，像這樣：

```
# 標題文字

## 標題文字

### 標題文字

#### 標題文字

##### 標題文字

###### 標題文字
```
### 粗體
語法: `**粗體**`
**粗體**
### 斜體
語法: `_斜體_`
_斜體_
### 純文字
語法: 以 \` \` 前後包住文字.

### 刪除線
語法: `~~刪除線~~`
~~刪除線~~
### 螢光筆
語法: `==螢光筆==`
==螢光筆==
### 上標
語法: `21^th^ 世紀`
21^th^ 世紀

### 下標
語法: `H~2~O`
H~2~O

### 語法區塊

1. 請在程式碼的前一行與後一行輸入 ` ``` ` 。
2. 您可以在程式碼區塊中指定語言類型，例如 html、javascript、python、markdown。
3. 就像這樣 :point_down: 
    ```
    ```python
      print('Hello, world!')
      # See if you can set arbitrary line number or 
      # change syntax highlighting for different language
      # in this code block.    
    ```
4. 然後，您可以將滑鼠移到程式語言名稱的右側，並使用功能表選擇加入行號、自動摺行[^自動摺行]，或不加上效果。

This is what it looks like after rendering :point_down: 

```python=6
  print('Hello, world!')
  # See if you can set arbitrary line number or 
  # change syntax highlighting for different language
  # in this code block.
```

## 我們重視您的回饋！
您覺得這篇指南有幫助嗎？ 歡迎填寫 [調查問卷](https://tally.so/r/wzQ6gZ) 告訴我們您的想法。

## 表格
在編輯器的工具列就有插入表格的工具

![image](https://hackmd.io/_uploads/SJss0x73R.png)

| 表格標題 | 表格標題 | 表格標題 |
| ------- | ------- | ------- |
| 表格文字 | 表格文字 | 表格文字 |


直接使用 Markdown 繪製表格可能會有點混亂，所以我們建立了表格工具提升你的工作效率。

點擊任一格，就會在編輯器工具列中出現表格工具選項，你可以快速套用表格格式。

![image](https://hackmd.io/_uploads/rJprxiHh0.png)

[ → 深入了解「如何建立表格」](https://hackmd.io/c/tutorials-tw/%2Fs%2Fhow-to-create-table-tw)

### 直接貼上 Excel 表格
您可以直接貼上 Excel 的表格，只要在工具列中啟用「智慧貼上」即可。

![image](https://hackmd.io/_uploads/SJqAm2IUA.png)

## 筆記目錄

輸入 `[TOC]` 將會出現如下的目錄，這個語法只會讀取 H1 ,H2 ,H3：

[toc]

如果你不想要加入 ``[TOC]``，筆記本來就有內建目錄可以瀏覽，並能夠在筆記內快速移動 :point_down:

>[!note] :bulb: **雙欄模式的目錄**
>
>您可以透過點擊雙藍模式中間的 `☰` 按鈕來檢視筆記目錄。
>![imgage](https://hackmd.io/_uploads/B1nfZK9TC.png =400x)

## 切換編輯頁面／檢視頁面

#### 編輯頁面
HackMD 編輯器的「編輯頁面」是您使用 Markdown 撰寫和套用格式的地方。
![圖片](https://hackmd.io/_uploads/rkzJ-PCJJl.png)

#### 檢視頁面
HackMD 編輯器的「檢視頁面」會顯示您的筆記將如何呈現；顯示套用格式的文字，包括標題、連結和圖片。讓您得以確保內容在分享或發佈之前，完全按照您的想法顯示。
您可以點選頁面右上角的 `編輯` 按鈕，隨時跳回編輯頁面。
![圖片](https://hackmd.io/_uploads/r1dnewRJkx.png)

## 瞭解更多HackMD使用方法
想要學習更多使用 HackMD 的方法嗎？查看您工作空間中的新手指南和進階指南。

### 新手指南將涵蓋
- 工作空間及側邊欄
- 個人工作空間
- 建立筆記
- 從範本建立筆記
- 插入圖片或GIF
- 留言和建議修訂
- 分享與設定權限
- 公開發表
- 瞭解更多HackMD使用方法

### 進階指南將涵蓋
- 團隊空間
- 與 GitHub 同步
- 串連API
- 書本模式
- 範本和客製化範本
- 嵌入筆記
- 使用MathJax寫出方程式
- 繪製UML流程圖
- 官方教學手冊

在您使用之前，HackMD 有一本官方的使用者手冊，裡面有所有功能的說明！

在我們的教學手冊中，您可以找到 HackMD 所有主要功能的詳細指南，提升您的工作效率。

### :point_right: [HackMD 教學手冊](https://hackmd.io/c/tutorials-tw/%2Fs%2Ftutorials-tw) :point_left:
#### 不想錯過 HackMD 的最新消息、新功能預告嗎？快按讚FB粉絲專頁或加入DC群吧~

- 客服信箱 :mailbox: support@hackmd.io
- <i class="fa fa-file-text"></i> 在 [Twitter](https://twitter.com/hackmdio) 上面提及 `@hackmdio` 
- <i class="fa fa-file-text"></i> [Facebook fanpage](https://www.facebook.com/hackmdio)
- <i class="fa fa-file-text"></i> [Discord channel](https://discord.gg/rAkfPd5Z)

## 我們重視您的回饋！
您覺得這篇指南有幫助嗎？ 歡迎填寫 [調查問卷](https://tally.so/r/wzQ6gZ) 告訴我們您的想法。


[^自動摺行]: 系統會將「超出文件寬度的程式碼區塊文字」自動換行，讓程式碼區塊的內容可以完整顯示，不需要滾動捲軸檢視。
