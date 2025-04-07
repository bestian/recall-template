# 罷免網站模板 (Recall Campaign Website Template)

這是一個專為台灣 2025 年罷免活動設計的網站模板，使用 Jekyll 搭配 GitHub Pages 快速建置。只需幾個簡單步驟，即可創建一個專屬於特定罷免案的宣傳網站。

## 🚀 快速開始（使用 GitHub）

1. **使用模板創建儲存庫**
   - 點擊 GitHub 頁面上方的 "Use this template" 綠色按鈕
   - 命名新儲存庫，建議格式：`recall-xxx`（xxx 為立委姓名或選區）
   - 選擇 "Public" 儲存庫，點擊 "Create repository from template"

2. **設定儲存庫**
   - 在新儲存庫的 Settings → Pages 中，將 Source 設為 `gh-pages` 分支
   - 約 1-3 分鐘後，GitHub 會提供一個網址，格式為 `https://你的用戶名.github.io/recall-xxx`

3. **編輯 `_config.yml`**
   - 在儲存庫中找到 `_config.yml` 檔案並編輯
   - 修改以下關鍵設定：

```yaml
# 罷免資訊
group_name: "第X選區罷免行動聯盟"  # 罷免團體名稱
legislator: "OOO"                 # 被罷免立委姓名
district: "台北市第X選區"          # 選區名稱
kmt_puppet: "傅xx"                # 傀儡人物名稱（若不適用可留空）

# 社群媒體連結（不需要的可刪除或留空）
social:
  facebook: "https://facebook.com/your-page"
  instagram: "https://instagram.com/your-account"
  threads: "https://threads.net/@your-account"
  line: "https://line.me/your-account"

# 地圖嵌入連結（從 Google Maps 獲取）
map_src: "https://www.google.com/maps/d/embed?mid=YOUR_MAP_ID"
```

完成設定後，網站會自動更新，無需額外操作！

## 📱 自訂網站

若要進一步自訂網站內容，可以編輯以下檔案：

### 1. `_data/events.yml` - 罷免事件時間軸

```yaml
- date: "2024年12月20日"
  title: "強行修改《公職人員選舉罷免法》"
  url: "https://www.readr.tw/post/3005"
  description: "立法院在缺乏充分討論的情況下，三讀通過法案，引發社會強烈反彈。"

- date: "2025年1月2日" 
  title: "另一個事件"
  url: "https://news-url.com"
  description: "事件描述..."
```

### 2. `_data/actions.yml` - 行動方案

```yaml
- title: "現場連署"
  description: "到各罷免連署站連署罷免"
  icon: "map-marker"  # Font Awesome 圖示

- title: "自行列印"
  description: "到 recall2025.ourtaiwan.tw 生成連署書，列印簽名後，到罷免連署站送件"
  icon: "print"
  button: true  # 是否顯示列印按鈕
```

### 3. 更換 QR Code

將你的罷免連署 QR Code 圖片命名為 `qrcode.png` 並上傳到儲存庫，取代原有檔案。

## 🖨 列印功能

網站內建的列印功能會自動優化版面配置：
- 隱藏非必要資訊（跑馬燈、地圖等）
- 顯示 QR Code
- 調整排版適合紙張印刷

測試列印：點擊網站上的「列印宣傳單」按鈕，或使用瀏覽器的列印功能。

## 🔄 跑馬燈嵌入功能

網站提供可嵌入其他網站的跑馬燈程式碼。在電腦版瀏覽器中點擊「複製本程式碼」按鈕，然後將程式碼貼到其他網站的 HTML 中即可。

## 🧩 進階自訂（選用）

若有更深入的自訂需求，可以：

1. 克隆儲存庫到本地
   ```
   git clone https://github.com/你的用戶名/recall-xxx.git
   cd recall-xxx
   ```

2. 安裝 Jekyll 環境（需要 Ruby）
   ```
   gem install bundler jekyll
   bundle install
   ```

3. 本地運行測試
   ```
   bundle exec jekyll serve
   ```

4. 編輯網站模板（`_layouts/default.html`）和樣式表（`index.css`、`print.css`）

5. 提交並推送變更
   ```
   git add .
   git commit -m "自訂網站"
   git push
   ```

## 📋 注意事項

- 網站自動顯示 15 天倒數計時，提醒罷免行動的緊迫性
- GitHub Pages 有流量限制，若預期訪問量極大，建議考慮其他託管服務
- 請確保所有內容符合選罷法規定，避免觸法

## 🤝 貢獻與問題回報

發現問題或有改進建議？歡迎在 GitHub 提交 [Issue](https://github.com/bestian/recall-template/issues) 或 Pull Request。

## 📜 授權

本專案採用 MIT 授權條款，歡迎自由使用與修改。

---

此罷免網站模板由公民開發者貢獻，希望協助台灣公民社會更有效地組織罷免行動。若有疑問，請透過 GitHub Issues 聯絡我們。