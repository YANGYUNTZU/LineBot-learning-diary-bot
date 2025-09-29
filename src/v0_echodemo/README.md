# 📌 專案簡介
這是一個基於 LINE Messaging API 與 Flask 的聊天機器人專案。
目前為 v0 Echo Bot 版本，功能僅包含 回聲機制（使用者傳什麼訊息，Bot 就原封不動回覆）。
此專案將會逐步演進，最終目標是打造一個能夠 紀錄學習日誌、分析關鍵字與情緒、並提供週報與視覺化回顧 的「學習日誌情緒教練 Bot」。

## ⚙️ 安裝方式
- 首先至 Line Developers登入後，建立新的Providers
- 設定好自動回覆，將「Channel access token」以及「Channel secret 」儲存至記事本
- 在colab中安裝「LINE Bot SDK v3」、「Flask」、「pyngrok」
- 接著執行ngrok程式碼，取得Webhook URL，複製
- #從Line bot sdk pypl網站找到程式碼貼上  
https://pypi.org/project/line-bot-sdk/
- 將「Channel access token」以及「Channel secret 」做更換，執行，程式呈現運轉中
- 最後將Webhook URL貼回Line Developer的專案中
- 到Line app即可回聲對話

### 🚀下載專案
git clone https://github.com/YANGYUNTZU/LineBot-learning-diary-bot.git  
cd LineBot-learning-diary-bot/src/v0_echodemo


## 📅 後續計畫
- v1：新增 SQLite 紀錄功能（user_id, ts, text）
- v2：關鍵字提取模組（TF-IDF / spaCy / yake 測試）
- v3：情緒分析模組（rule-based / TextBlob / Hugging Face）
- v4：每週回顧（統計 + 簡單分析回饋）
- v5：視覺化報表（趨勢圖、情緒分布圖）

