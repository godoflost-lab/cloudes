# 即時文字雲互動投票

這是一個部署在 **GitHub Pages** 的互動投票工具，結合 Firebase Firestore 即時更新文字雲。  
倉庫名稱：`cloudes`  
正式網址（部署後）：  
👉 https://godoflost-lab.github.io/cloudes/

---

## 使用方式

### 👩‍🏫 老師（主控台）
1. 進入 [主控台](https://godoflost-lab.github.io/cloudes/#/host)。
2. 輸入題目，按下 **建立房間**。
3. 系統會產生：
   - 學生作答連結 & QR code  
   - 投影用文字雲連結 & QR code  
4. 可隨時控制：
   - **開始作答 / 暫停作答**  
   - **清空所有作答**  
   - **匯出 CSV**  

---

### 🧑‍🎓 學生
1. 掃描 QR code 或進入連結（例如 `https://godoflost-lab.github.io/cloudes/#/r/ABC123`）。  
2. 輸入房號（或自動帶入），即可作答。  
3. 可輸入多個詞語，用 **逗號或換行** 分隔。  

---

### 📺 投影展示
- 開啟 [大螢幕展示](https://godoflost-lab.github.io/cloudes/#/d/ABC123)。  
- 即時更新文字雲，支援全螢幕（按 `F`）。  

---

### 🛠️ 自我檢測
若功能無法使用，請：
1. 進入 [主控台](https://godoflost-lab.github.io/cloudes/#/host) → 按 **自我檢測**。  
2. 會輸出診斷訊息，方便排查是否：
   - Firestore 未建立 / 規則問題  
   - 網路阻擋（防火牆 / 代理）  
   - 程式碼錯誤  

---

## 系統需求
- Firebase Firestore 已建立，並允許存取（目前 Rules 為測試模式，至 2025/09/23 前可用）。  
- 支援現代瀏覽器（Chrome, Edge, Safari）。  

---

## 部署方式（僅需一次設定）
1. 在倉庫根目錄放置 `index.html`。  
2. GitHub → **Settings → Pages** → 選擇 Branch: `main`、資料夾: `/ (root)`。  
3. 完成後即可從以下網址存取：  
   👉 https://godoflost-lab.github.io/cloudes/