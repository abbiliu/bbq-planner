# 年度烤肉聚會準備網站

規格見 `bbq-planner-spec.md`。純前端 SPA + Firebase Firestore 即時同步，部署到 GitHub Pages。

## 專案資訊
- Firebase 專案：`bbq-planner-878af`（Firestore 位置：asia-east1 Taiwan）
- Firebase 設定值：`firebase-config.json`（已內嵌在 `index.html` 中）
- GitHub repo：https://github.com/abbiliu/bbq-planner

## 網址
https://abbiliu.github.io/bbq-planner/

## 目前進度
- [x] Firebase 專案 + Firestore(Standard, asia-east1) 建立
- [x] GitHub repo 建立
- [x] Firestore 規則開放為公開讀寫（無登入、信任制，網址不要亂分享）
- [x] 首頁／活動列表（4.1）+ 歷年資料種子匯入（已實測：22 屆歷史資料、統計、記憶點編輯都正常）
- [x] 活動工作區（進 2026 活動後的分頁：總覽/認領/我的清單/花費/結算）+ 身分改用家庭名單比對（localStorage 存名稱，跨年可延用）
- [x] 打開網站直接自動進今年活動（不用先點一次），首頁改成儀表板：活動資訊+地圖導航連結+認領進度/參與人員/我的清單快捷卡，歷史紀錄收在下方連結（點了自動展開）
- [x] 活動資訊（4.2，地點/日期，可編輯，地址可一鍵開 Google Maps 導航）
- [x] 家庭名單（4.3，獨立頁面「參與人員」，新增/編輯/刪除，已實測）
- [x] 清單認領（4.4，改成點一下直接認領/取消認領，不用每次跳數量視窗；緊湊列表一頁看更多項；加了分類篩選；可直接新增項目/新分類；數量調整收在小圖示裡，已實測）
- [ ] 我的準備清單（4.5）
- [ ] 花費（4.6）
- [ ] 結算頁（4.7）
- [ ] 設定（4.8）
- [x] GitHub Pages 部署上線
