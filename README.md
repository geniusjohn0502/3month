# 三個月理財陪跑（NT$8,000）銷售頁

- **對外網址**：https://3month.morechoice.net（舊網址 `geniusjohn0502.github.io/plan-2028/3month/` 會自動跳到這裡）
- **本機資料夾**：`~/Documents/網頁與程式/三個月陪跑網頁`
- **在漏斗的位置**：Threads 導流 → 免費諮詢（consult.morechoice.net）→ 諮詢中提案 → **這一頁**（聊過之後給對方看）

2026-10-14 從 `plan-2028/3month/` 搬出來獨立成一個專案，外觀改成跟免費諮詢頁、桌遊報名頁同一套（米白底、苔綠＋陶土色、明體標題）。**改配色請三頁一起改。**

## 檔案

```
index.html      整頁（樣式寫在裡面）
about.jpg       開場照片（跟 consult 的 john.jpg 同一張）
about-john.jpg  About 區照片（跟 consult 同一張）
見證/01–10.jpg  學員 LINE 對話截圖（學員皆已同意公開）
CNAME           自訂網域，不要刪
```

## 改版

```bash
cd ~/Documents/網頁與程式/三個月陪跑網頁
git add <改過的檔案> && git commit -m "說明" && git push
# GitHub Pages 約 1 分鐘後生效
```

⚠️ **文案基準在私有 repo**：`100_Todo/projects/2026-08-03_三個月陪跑銷售頁.md`。改文案時 HTML 和那份 md 要一起改。

⚠️ **這是公開 repo**：客戶個資、內部定價邏輯、諮詢紀錄一律不得放進來。

## 網域設定（已完成，留著備查）

- Cloudflare DNS：`CNAME` `3month` → `geniusjohn0502.github.io`，**Proxy 關閉（僅 DNS，灰色雲朵）**
- GitHub → Settings → Pages：Custom domain `3month.morechoice.net`，Enforce HTTPS 勾選
- 憑證卡住發不出來時：把自訂網域清空 → 等建置完成 → 再設回去（consult 踩過）
