# 洲子街午餐籤

給內湖區洲子街105號辦公室用的午餐決定小工具。純前端、無需後端，可直接部署到 GitHub Pages。

- 收錄走路 10 分鐘內的 17 間店家（便當、美食街、小吃、咖啡輕食、異國料理）
- 可依「類型 / 步行時間 / 預算」篩選
- 按「抽籤決定午餐」隨機抽出一間，用籤詩卡片呈現
- 篩選條件會存在瀏覽器 localStorage，下次打開會記得你的設定

## 部署到 GitHub Pages（約 3 分鐘）

1. 在 GitHub 開一個新 repo，例如取名 `lunch-oracle`。
2. 把這個資料夾裡的 `index.html` 上傳到 repo 的根目錄（可以直接在 GitHub 網頁上「Add file → Upload files」拖曳上去，不需要用終端機）。
3. 進入 repo 的 **Settings → Pages**。
4. 在 "Build and deployment" 底下的 Source 選擇 **Deploy from a branch**，Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
5. 等 1–2 分鐘，頁面會出現在 `https://<你的帳號>.github.io/lunch-oracle/`。

之後想更新店家資料，直接編輯 `index.html` 裡 `SPOTS` 這個陣列（每間店一個物件），改完存檔、上傳覆蓋即可，不需要重新設定 Pages。

## 資料怎麼來的

店家清單、評分、營業時間是用 Google 地圖資料整理（2026年8月），價格區間則是依店家等級與評論內容做的**估計值**，實際售價請以現場公告為準。走路時間以每分鐘約 75 公尺概算，僅供參考。
