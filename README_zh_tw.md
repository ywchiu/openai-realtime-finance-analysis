[English](README.md) | 繁體中文

# 即時股票分析助手

這個專案是一個即時股票分析助手，使用 OpenAI 的 Realtime API 和 Polygon.io 的金融資料 API 來提供最新的股票資訊和分析。

## 功能特色

- 使用 OpenAI 的 Realtime API 進行即時語音互動
- 透過 Polygon.io API 取得股票資訊
- 互動式股價圖表
- 與查詢股票相關的最新新聞
- 按鍵對講和語音活動偵測（VAD）模式
- 事件紀錄和視覺化

## 使用前準備

- OpenAI API 金鑰
- Polygon.io API 金鑰
- 已安裝 Node.js 和 npm

## 設定

1. 複製（clone）此專案庫
2. 安裝相依套件：
   ```
   npm install
   ```

## 執行應用程式

1. 啟動開發伺服器：
   ```
   npm start
   ```
2. 開啟瀏覽器並前往 `http://localhost:3000`

## 使用方法

1. 點擊「連線」按鈕開始對話
2. 使用按鍵對講按鈕或啟用 VAD 模式與助手互動
3. 詢問股票資訊，例如：「AAPL 的目前價格是多少？」
4. 在右側面板查看即時股票資訊、圖表和新聞

## 元件

- `ConsolePage`：處理使用者介面和邏輯的主要元件
- `LineChart`：顯示歷史股價資料
- `WavRecorder`：處理音訊輸入
- `WavStreamPlayer`：管理音訊輸出
- `RealtimeClient`：與 OpenAI 的 Realtime API 介接

## API 整合

- OpenAI Realtime API：用於語音互動和自然語言處理
- Polygon.io API：取得股票資訊、歷史資料和新聞

## 注意事項

- 應用程式使用本地中繼伺服器來隱藏 API 金鑰並執行自訂邏輯
- 你可以在手動（按鍵對講）和 VAD 模式之間切換語音輸入
- 事件紀錄顯示來自客戶端和伺服器的即時事件

## 疑難排解

如果遇到 API 金鑰問題，你可以透過點擊使用者介面中顯示的金鑰來重設它們。

## 聯絡 

[david@largitdata.com](mailto:david@largitdata.com)
