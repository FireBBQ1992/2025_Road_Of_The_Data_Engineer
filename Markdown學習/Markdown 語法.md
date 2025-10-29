---
title: Markdown 語法
tags: [onboarding]

---
# Markdown 語法

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


## 表格
在編輯器的工具列就有插入表格的工具(HackMD)

![image](https://hackmd.io/_uploads/SJss0x73R.png)

| 表格標題 | 表格標題 | 表格標題 |
| ------- | ------- | ------- |
| 表格文字 | 表格文字 | 表格文字 |


直接使用 Markdown 繪製表格可能會有點混亂，所以我們建立了表格工具提升你的工作效率。

點擊任一格，就會在編輯器工具列中出現表格工具選項，你可以快速套用表格格式。

![image](https://hackmd.io/_uploads/rJprxiHh0.png)

[ → 深入了解「如何建立表格」](https://hackmd.io/c/tutorials-tw/%2Fs%2Fhow-to-create-table-tw)




