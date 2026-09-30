# MNQ ATM Core V2.2（TradingView）

這個儲存庫保存 2026-09-30 提供的 TradingView Pine Script v6 原始碼，主檔為 [`MNQ_ATM_Core_V2.2.pine`](MNQ_ATM_Core_V2.2.pine)。主檔保留收到時的內容，方便比對與檢閱。

## 內容

程式使用 `strategy()`，屬於 TradingView 回測策略。它以 1 分鐘 MNQ 圖表為設計對象，計算台北時間 06:00–07:00 的區間，依結構突破與反轉條件管理限價掛單，並繪製進場、停損與目標價標記。

在 TradingView 的 Pine 編輯器貼上主檔後，可將策略加到 1 分鐘 MNQ 圖表檢視。這份 repo 未附回測報表，也未宣稱任何交易績效。

## 版本註記

目前程式將 `useFixedRisk` 設為 `false`，會執行結構停損分支。檔案開頭仍有固定 20／50 點的舊註解；閱讀或展示時，請以實際程式分支為準。此儲存庫未修改收到的 Pine Script，也尚未在 TradingView 編譯器驗證。
