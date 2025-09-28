# 學習日誌情緒教練 Bot

這是一個 LINE Messaging API Bot 的專案，主題為 **學習日誌情緒教練**。  
使用者每天可以輸入學習心得與心情，系統將進行關鍵字萃取與情緒分析，並提供回饋。  
專案 | AI × NLP × LINE Messaging API


## 📌 專案簡介
- 使用者每天輸入 學習心得 + 心情
- Bot 自動進行 關鍵字提取 & 情緒分析
- 將資料儲存，並在每週產出 學習／情緒回顧
- 目標：讓學習更有自我覺察，培養正向的學習習慣


## 🗂️ 專案結構
- src/              # 主要程式碼
- tests/            # 測試程式
- notebooks/        # NLP 模型實驗
  - keywords_dev.ipynb   # 關鍵字提取測試
  - sentiment_dev.ipynb  # 情緒分析測試
- requirements.txt  # 套件需求
- .env.example      # 環境變數範例
- .gitignore        # 忽略檔案設定
- README.md         # 專案說明


## ⚙️ 環境需求
- Python 3.10+
- Flask（Web 框架，後續做 webhook）
- line-bot-sdk（LINE Messaging API SDK）
- python-dotenv（環境變數管理）
- SQLite（簡單資料儲存，未來擴充）


## 🚀 使用方式
### 1,安裝套件
pip install -r requirements.txt

### 2.建立 .env
LINE_CHANNEL_SECRET=your_channel_secret_here  
LINE_CHANNEL_ACCESS_TOKEN=your_channel_access_token_here

### 3.（未來）啟動伺服器並設定 LINE Webhook URL /callback


## 🧩 功能規劃
- v0：Echo Bot（確認 webhook 流程）
- v1：寫入 SQLite → 儲存學習心得 & 心情
- v2：關鍵字提取（TF-IDF / NLP 方法）
- v3：情緒分析（規則式 / 模型）
- v4：每週回顧報告（平均心情、Top Keywords）
- v5：視覺化（圖表化學習／情緒趨勢）


## 📊 系統流程圖（示意）
### flowchart TD
     A[使用者輸入心得+心情] --> B[LINE Webhook 接收]
     B --> C[關鍵字提取]
     B --> D[情緒分析]
     C --> E[SQLite 紀錄]
     D --> E[SQLite 紀錄]
     E --> F[即時回覆 + 週期回顧]

    
 ## 🗺️ Roadmap
 ###    
- v0 Echo Bot → 2025/10 上旬
- v1 SQLite 紀錄 → 2025/10 下旬
- v2 關鍵字提取 → 2025/11 上旬
- v3 情緒分析 → 2025/11 下旬
- v4 週期回顧 → 2025/12 上旬
- v5 視覺化 → 2025/12 下旬–2026/01


## 📖 授權
MIT License


