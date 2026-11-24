# 湯圓製造所

## 預覽
解壓縮後開啟 index.html。未設定雲端時為本機預覽，資料不會跨裝置同步。建議以 VS Code Live Server 或 `python -m http.server 8000` 開啟。

## 雲端部署
1. 在 https://supabase.com 建立新專案。
2. SQL Editor 建立新查詢，貼上 schema.sql 並執行一次。
3. 將 Project URL 和 publishable key（或 anon key）填入 config.js。不要使用 service_role key。
4. 將整個資料夾上傳 GitHub，使用 Render Static Site 或 GitHub Pages 部署，發布目錄為專案根目錄。
5. Supabase Authentication URL Configuration 設定正式 HTTPS 網址為 Site URL。兩人分別註冊、驗證電子郵件並登入。
6. 第一人建立共同空間，第二人輸入配對碼加入。配對碼請勿公開。每個空間最多兩人。
7. iPhone Safari 開啟正式網址，分享 → 加入主畫面。

## 限制
雲端尚未連接實際專案，未進行雙手機端到端測試。照片以小型 data URL 儲存（每張 1 MB），本機預覽有瀏覽器容量限制；不會自動遷移預覽資料。想你按鈕是共同紀錄而非背景推播。班表為逐日新增，紀念日為指定日期倒數，沒有循環排班或年度自動提醒。每日問答目前固定題目，夫妻100件事為自訂清單。轉盤選項不會跨裝置儲存。離線僅快取網站，不提供雲端離線寫入。未提供密碼重設及解除配對介面。圖片來自使用者提供的參考圖，公開發行前應確認授權。

## V4.6
全站視覺重整，原有資料鍵、SQL、登入及 CRUD 保留。五張使用者圖片原檔保留於 assets；公開發行前確認授權。app.js 為舊版保留檔，實際執行 index.html 內嵌程式。

V4.12：移除共同養成小屋及入口，保留既有資料與夫妻集點卡。
