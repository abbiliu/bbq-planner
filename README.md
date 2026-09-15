# 年度烤肉聚會準備網站

規格見 `bbq-planner-spec.md`。純前端 SPA + Firebase Firestore 即時同步，部署到 GitHub Pages。

## 專案資訊
- Firebase 專案：`bbq-planner-878af`（Firestore 位置：asia-east1 Taiwan）
- Firebase 設定值：`firebase-config.json`（已內嵌在 `index.html` 中）
- GitHub repo：https://github.com/abbiliu/bbq-planner

## ⚠️ 待辦：開放 Firestore 安全性規則
Firestore 目前預設是「所有讀寫都拒絕」。這份 spec 要求「不登入、不記名、信任制、所有人都能編輯」，
所以要手動把規則改成公開讀寫（僅供家族內部網址分享，不做任何權限控管）：

1. 開 https://console.firebase.google.com/project/bbq-planner-878af/firestore/rules
2. 把內容整段換成：
   ```
   rules_version = '2';
   service cloud.firestore {
     match /databases/{database}/documents {
       match /{document=**} {
         allow read, write: if true;
       }
     }
   }
   ```
3. 按「發布」

這一步涉及安全性設定，系統會擋下我自動執行，需要你自己按幾下。

## 目前進度
- [x] Firebase 專案 + Firestore(Standard, asia-east1) 建立
- [x] GitHub repo 建立
- [ ] Firestore 規則開放（見上）
- [x] 首頁／活動列表（4.1）+ 歷年資料種子匯入
- [ ] 活動總覽卡（4.2）
- [ ] 家庭名單（4.3）
- [ ] 清單認領（4.4）
- [ ] 我的準備清單（4.5）
- [ ] 花費（4.6）
- [ ] 結算頁（4.7）
- [ ] 設定（4.8）
- [ ] GitHub Pages 部署上線
