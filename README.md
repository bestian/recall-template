
# recall-template 罷免網站模版使用說明

這是一個簡單易改的靜態網站模版，適用於各種罷免立委的宣傳行動。只需進行幾項簡單修改，就可以快速架設屬於你的罷免網站。

---

## 🚀 快速開始

1. **下載專案**

   ```
   git clone https://github.com/bestian/recall-template.git
   cd recall-template
   ```

2. **開啟 `index.html` 開始編輯**

   使用你熟悉的編輯器（例如 VS Code）開啟專案，進行以下幾處自訂內容調整。

---

## 🛠 要修改的地方

### 1. **網站標題與對象名稱**
   修改 `<title>` 與 `<h1>`：

   ```html
   <title>罷免OOO</title>
   ...
   <h1>罷免OOO就是罷免傅xx</h1>
   ```

   替換成你要罷免的對象。

---

### 2. **社群連結**

   修改 `.social-icons` 區塊，替換成你自己的 Threads / GitHub 或其他平台連結：

   ```html
   <a href="https://www.threads.net/@你的帳號">Threads</a>
   <a href="https://github.com/你的帳號/你的儲存庫">GitHub</a>
   ```

---

### 3. **事件時間軸內容**

   修改 `.event-container` 中的內容，可以新增或移除事件：

   ```html
   <div class="event">
     <h4>日期：<a href="新聞連結">事件標題</a></h4>
     <p>簡短描述</p>
   </div>
   ```

---

### 4. **連署資訊與QRCode**

   - 若要替換 QR Code，請將你的 QR 圖片檔命名為 `qrcode.png` 並放入專案資料夾中。
   - 可自訂連署網址（通常會指向 [https://recall2025.ourtaiwan.tw](https://recall2025.ourtaiwan.tw)）。

---

### 5. **罷免地圖**

   替換 iframe 中的 Google Map URL 為你們自己的罷免連署站地圖：

   ```html
   <iframe src="你自己的地圖連結"></iframe>
   ```

---

### 6. **跑馬燈（可選）**

   若你希望嵌入這段跑馬燈到其他網站，可以複製 `<script id="recall">...</script>` 這段程式碼，貼到別人的網站中。

---

## 🖨 列印宣傳單功能

點擊「列印宣傳單」按鈕會自動觸發列印。你也可以客製化 `print.css` 設計列印版面樣式。

---

## 📦 發佈網站

你可以用以下方式部署這個靜態網站：

- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages（推薦）

---

## ✅ 授權

此模版採用 MIT License，歡迎自由使用與修改。

---

## 🙌 由誰製作

本模版由 [小巴老師 (Bestian Tang)](https://github.com/bestian) 製作，歡迎自由改作或回報問題。

---

需要進一步協助？可以在 GitHub 提 [issue](https://github.com/bestian/recall-template/issues)。

---