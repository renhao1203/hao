## （1）PERT/CPM圖
``` mermaid
graph TD
    T1[1 研擬計畫]
    T2[2 任務分配]
    T3[3 取得硬體]
    T4[4 程式開發]
    T5[5 安裝硬體]
    T6[6 程式測試]
    T7[7 撰寫使用手冊]
    T8[8 轉換檔案]
    T9[9 系統測試]
    T10[10 使用者訓練]
    T11[11 使用者測試]

    T1 --> T2
    T1 --> T3
    T2 --> T4
    T3 --> T5
    T4 --> T6
    T5 --> T7
    T5 --> T8
    T6 --> T9
    T7 --> T10
    T8 --> T10
    T9 --> T11
    T10 --> T11
```
---
## （2）甘特圖
``` mermaid
gantt
    title 專案甘特圖
    dateFormat YYYY-MM-DD
    section 計畫
    研擬計畫 : done, a1, 2025-01-01, 1d 
    任務分配 : done, a2, after a1, 4d


    section 硬體
    取得硬體 : a3, after a2, 17d 
    安裝硬體 : a5, after a3, 10d


    section 軟體
    程式開發 :a4, after a2, 70d
    程式測試 :a6, after a4, 30d
 
    section 文件與轉換
    撰寫使用手冊  : a7,after a4,25d
    轉換檔案     : a8,after a4,20d

    section 測試與訓練
    系統測試 : a9, after a5 аб, 25d
    使用者訓練 :a10,after a7 a8, 20d
    使用者測試 :a11, after a9 a10, 25d

```
## （3）關鍵路徑
    1（研擬計畫） → 2（任務分配） → 4（程式開發） → 6（程式測試） → 9（系統測試） → 11（使用者測試）
