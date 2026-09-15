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
- [ ] 活動總覽卡（4.2）
- [ ] 家庭名單（4.3）
- [ ] 清單認領（4.4）
- [ ] 我的準備清單（4.5）
- [ ] 花費（4.6）
- [ ] 結算頁（4.7）
- [ ] 設定（4.8）
- [x] GitHub Pages 部署上線
