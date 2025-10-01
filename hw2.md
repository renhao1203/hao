＃＃ （1）PERT/CPM圖
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
 ＃＃ （2）甘特圖
``` mermaid
gantt
    title 專案甘特圖
    dateFormat  D
    section 規劃
    研擬計畫        :done,  des1, 1, 1d
    任務分配        :done,  des2, 2, 4d
    section 設備與程式
    取得硬體        :done,  des3, 2, 17d
    程式開發        :active,des4, 6, 70d
    安裝硬體        :         des5, 19, 10d
    section 測試、手冊
    程式測試        :         des6, 76, 30d
    撰寫使用手冊    :         des7, 29, 25d
    轉換檔案        :         des8, 29, 20d
    section 訓練與驗收
    系統測試        :         des9, 106, 25d
    使用者訓練      :         des10, 54, 20d
    使用者測試      :         des11, 131, 25d

```
