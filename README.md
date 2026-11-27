# 包裝物料倉儲管理系統

單一 HTML 檔案的簡易倉儲管理工具，支援物料管理、盤點、到倉、用量計算、CBM 計算與下單 Email 生成。

## 功能

- **Dashboard**：庫存警示、Critical / Low / OK 狀態
- **物料清單**：新增、編輯、刪除、Excel 導入/導出
- **盤點記錄**：批量輸入、匯出盤點清單、Excel 導入
- **到倉記錄**：記錄到貨、關聯下單、Excel 導入
- **用量計算**：依盤點與到倉自動計算 Monthly Usage
- **CBM 計算**：單物料與總庫存 CBM
- **下單**：依供應商範本生成 Email，儲存下單紀錄並與到倉結合
- **登入保護**：清空紀錄與修改物料需登入（預設密碼：`admin123`）

## 使用方式

### 直接開啟
下載 `index.html`，用瀏覽器開啟即可（資料存在瀏覽器 localStorage）。

### GitHub Pages 部署
1. 將此檔案放到 GitHub repository
2. Settings → Pages → Source 選擇 `main` 分支
3. 幾分鐘後即可透過 `https://你的帳號.github.io/倉庫名稱/` 使用

## 資料儲存
所有資料存在瀏覽器 `localStorage`，清除瀏覽器資料會遺失。建議定期匯出備份。

## 供應商 Email 範本
- **ChengDu**：Cheng.Luo@balluff.de 等
- **Arvato-Yannie**：yannie.tang@arvato.com 等
- **木林森**：sales3@mlsplywood.com
- 其他：通用格式

## 注意事項
- 本工具為前端原型，資料僅存在本地瀏覽器
- 登入狀態使用 sessionStorage，關閉分頁後需重新登入
- Excel 導入/導出使用 SheetJS（CDN）
