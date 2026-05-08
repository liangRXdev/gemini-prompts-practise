# 🏥 Gemini 醫療教學 Prompt 範本庫 (教學練習用)

[![Live Demo](https://img.shields.io/badge/Live_Demo-Click_Here-blue?style=for-the-badge&logo=github)](https://liangrxdev.github.io/gemini-prompts-practise/)

這是一個專為**臨床教師、藥師與醫療專業人員**打造的輕量化提示詞（Prompt）開源範本庫。旨在降低醫療人員使用生成式 AI（如 Google Gemini）的門檻，將高耗時的教學準備工作（如設計教案、製作衛教單張、彙整文獻）轉化為高效的人機協作流程。
* PS. 主要為2026/04/30 院內 Gemini 基礎課程教學用

## ✨ 核心特色

* **🚀 一鍵複製 (1-Click Copy)**：點擊按鈕即可複製完整提示詞，無縫貼入 Gemini 對話框，免去現場打字與構思的摩擦力。
* **🩺 醫療情境導向**：內建多種臨床教學專屬 Prompt，涵蓋 PBL 劇本生成、PICO 表格轉化、OSCE 考站設計與圖表生成等。
* **⚡ 極簡架構 (Zero-Config)**：採用純靜態前端架構（單一 `index.html` 檔案），資料與畫面分離，無需任何後端或資料庫即可運作。
* **📱 響應式設計 (RWD)**：支援手機、平板與桌機，方便臨床教師在任何裝置上快速查閱。

## 🛠️ 內建 Prompt 應用場景

目前範本庫收錄的提示詞涵蓋以下四大領域：
1.  **教材與簡報開發**：大綱生成、標題發想、資訊圖表快速產出。
2.  **臨床教學設計**：PBL 劇本生成（含干擾資訊設計）、互動式小遊戲開發。
3.  **多模態應用 (Nano Banana 2)**：將文字轉化為具備一致性的醫療情境圖片、公仔生成、漫畫分鏡繪製。
4.  **實證醫學與文獻解析**：長文本摘要、指引分析、PICO 結構化輸出。

## 🚀 如何使用與部署

### 一般使用者
直接開啟 [Live Demo](https://lianggaga927-beep.github.io/gemini-prompts-practise/)，找到符合您需求的提示詞卡片，點擊「複製 Prompt」，並前往 Gemini 貼上執行即可。

### 開發者 / 課程講師 (想要建立自己的範本庫)
如果您想加入自己開發的專屬 Prompt 範本，只需簡單三步驟：

1.  **Fork 或 Clone 專案**：
    ```bash
    git clone [https://github.com/lianggaga927-beep/gemini-prompts-practise.git](https://github.com/lianggaga927-beep/gemini-prompts-practise.git)
    ```
2.  **編輯 `index.html`**：
    找到程式碼後段 `<script>` 標籤內的 `promptData` 陣列，按照 JSON 格式新增物件：
    ```javascript
    {
        title: "您的新功能名稱",
        content: "在此輸入您的 Prompt 指令全文..."
    }
    ```
3.  **推送到 GitHub**：
    將變更 Commit 並 Push 回您的 GitHub 儲存庫，GitHub Pages 將在 1 分鐘內自動更新網頁內容。

## ⚠️ V.I.T.A.L. 醫療 AI 使用安全規範

使用本範本庫產出之內容時，請務必遵循以下 **V.I.T.A.L.** 審查原則，以確保臨床安全：

* **V (Verify Data)**：驗證數據，特別是藥物劑量、單位與檢驗正常值，務必經人工二次查核。
* **I (Identity)**：保護隱私，**嚴禁**於 Prompt 中輸入病人姓名、病歷號或具識別性之個資。
* **T (Traceability)**：文獻溯源，AI 可能產生虛構文獻，請務必點擊連結或搜尋 PMID 確認真實性。
* **A (Applicability)**：在地適用，確認 AI 建議之處置符合台灣健保規範、院內處方集與法規。
* **L (Logic)**：邏輯檢查，檢視 AI 產出的病理推論與教學誘答選項是否符合臨床合理性。

---
*Powered by Google Gemini & Designed for Clinical Educators.*
