# AlunaStudio 優化任務清單

> 每次執行 3 項，完成後在 `[x]` 標記，並更新進度條。
> 主要檔案：`~/Developer/pure-veglife/docs/艾妮莎工具台.html`（後端總控台）
> 前端網頁：`~/Developer/aluna-studio/index.html`
> 編輯後台：`~/Developer/pure-veglife/docs/AlunaStudio-admin.html`（待分析）

---

## 進度總覽（每次更新）

```
後端總控台: █████████████████████████  38/38 (100%)
前端網頁:   ░░░░░░░░░░  0/6  (0%)
編輯後台:   ░░░░░░░░░░  待分析
整體進度:   ███████████████  38/47+ (81%)
```

### 第 1 輪（2026-05-19）完成：G1、G4、M1
### 第 2 輪（2026-05-19）完成：G2、G3、M2
### 第 3 輪（2026-05-20）完成：G5、G6、SP1
### 第 4 輪（2026-05-20）完成：G7、S1、S2
### 第 5 輪（2026-05-20）完成：SP2、F2、O1
### 第 6 輪（2026-05-20）完成：O2、D3、AI1
### 第 7 輪（2026-05-20）完成：AI2、AI3、C1
### 第 8 輪（2026-05-20）完成：MK1、MK2、R1
### 第 9 輪（2026-05-20）完成：SP3、F3、D1、D2、D4、S3
### 第 10 輪（2026-05-20）完成：F4、PR3、MK3、AI4、R3、C2
### 第 11 輪（2026-05-20）完成：C3、C4

---

## P0｜全域品牌色 + 即時資料錯誤（Critical）

| # | 項目 | 位置 | 狀態 |
|---|------|------|------|
| G1 | CSS `--pink` → `#2A1E1D`（深玫棕），`--pink-lt` → `#F5EDE8` | 工具台 `<style>` | [x] |
| G2 | Header bar 亮桃紅漸層 → 深玫棕 `#2A1E1D` solid | 工具台 `.app-bar` | [x] |
| G3 | 側欄 emoji（📋🏠🎉📢⚡👥）→ 純文字 + 2px 左邊線 active state | 工具台 sidebar | [x] |
| G4 | 全檔案 `$` → `NT$`（金額顯示格式） | 工具台全文 | [x] |
| G5 | `.sec-title` font-weight 900 → 400 | 工具台 CSS | [x] |
| G6 | 所有 CTA 按鈕（亮桃紅漸層）→ 深玫棕 solid + white text | 工具台全文 | [x] |
| G7 | 所有表格邊框 → 僅底線 1px `#E8DDD5` | 工具台全文 | [x] |
| M1 | bkSlotGrid 時間段 — 移除 18:30、19:00、19:30、20:00（工作室 18:00 關門） | 工具台 booking modal | [x] |
| M2 | bk-plan 下拉選項 — 移除「時租（30分計）」，選項改為：時租 / 半日上午 / 半日下午 / 月租核銷 / 包場 | 工具台 booking modal | [x] |
| SP1 | KPI 卡片「詢問→確認轉換率」— 移除紅色背景，改用左邊線樣式 | 工具台 `sec-space` | [x] |
| SP3 | 「+ 新增記錄」按鈕 → 品牌色（同 G6） | 工具台 `sec-space` | [x] |

---

## P1｜品牌質感（This Round）

| # | 項目 | 位置 | 狀態 |
|---|------|------|------|
| S1 | AI 特辦 P1/P2 標籤 → 小 badge，深玫棕 | 工具台 `sec-schedule` | [x] |
| S2 | 複製/預覽按鈕 → 降低視覺權重（outline + 小字） | 工具台 `sec-schedule` | [x] |
| SP2 | AI 分析建議深紫色 header → 淺米色卡片 | 工具台 `sec-space` | [x] |
| F2 | 收入/支出/利潤卡片 — 移除彩色背景 | 工具台 `sec-fin` | [x] |
| F3 | 財務表格邊框 → 同 G7 | 工具台 `sec-fin` | [x] |
| O1 | SOP 區塊 emoji 標題 → 全部移除 | 工具台 `sec-rules` | [x] |
| O2 | 重置按鈕 → 灰色 outline | 工具台 `sec-rules` | [x] |
| D1 | 月趨勢圖：資料 < 2 個月時隱藏 | 工具台 `sec-dash` | [x] |
| D2 | 轉換漏斗：全部為零時隱藏 | 工具台 `sec-dash` | [x] |
| D3 | AI 營運洞察 — 硬編碼建議文字後加「（範例）」 | 工具台 `sec-dash` | [x] |
| D4 | 星期分佈圖：無資料時隱藏 | 工具台 `sec-dash` | [x] |
| MK1 | IG 預覽 frame → 改為純文字預覽卡片 | 工具台 `sec-marketing` | [x] |
| MK2 | 自動分配按鈕 → 品牌色（同 G6） | 工具台 `sec-marketing` | [x] |
| AI1 | Agent Queue 深藍色區塊 → 白色卡片 + 深玫棕 serif 標題 | 工具台 `sec-ai` | [x] |
| AI2 | "AUTONOMOUS MODE · PREVIEW" → lowercase 小 badge | 工具台 `sec-ai` | [x] |
| AI3 | "EXECUTION LOG" → 「近期執行紀錄」（中文） | 工具台 `sec-ai` | [x] |
| C1 | 顧客類型欄位 → select enum（音療師/瑜珈老師/塔羅占星/美業/空中/其他） | 工具台 `sec-customers` | [x] |
| R1 | 規則頁面 emoji → 全部移除（同 O1） | 工具台 `sec-rules` | [x] |

---

## P2｜功能深化（下一輪）

| # | 項目 | 位置 | 狀態 |
|---|------|------|------|
| S3 | 週排程日期列 → 今日高亮 | 工具台 `sec-schedule` | [x] |
| F4 | 淨利下方加：備用金（20%）和可提領金額計算 | 工具台 `sec-fin` | [x] |
| PR3 | 特色條列 textarea → 加 `data-field="features_list"` markup | 工具台 `sec-pricing` | [x] |
| MK3 | 文案歷史庫 → 加 `status` 和 `post_date` 欄位 | 工具台 `sec-marketing` | [x] |
| AI4 | Agent Queue 待辦任務 → 加說明文字 | 工具台 `sec-ai` | [x] |
| R3 | 規則頁底部 → 加 `padding-bottom: 60px` | 工具台 `sec-rules` | [x] |
| C2 | 顧客卡片 → 顯示 total_bookings、total_revenue、contract_type | 工具台 `sec-customers` | [x] |
| C3 | 「+ 新增顧客」→ 品牌色（同 G6） | 工具台 `sec-customers` | [x] |
| C4 | 顧客頭像 → 姓名第一字圓形 badge（品牌色） | 工具台 `sec-customers` | [x] |

---

## 前端網頁｜index.html

| # | 項目 | 狀態 |
|---|------|------|
| FE1 | LINE 連結換成真實 LINE ID（目前為 `@alunastudio` 佔位）× 2 處 | [x] |
| FE2 | `.ph-mirror` → 換成真實照片 `images/mirror.jpg` | [ ] |
| FE3 | `.ph-bowls` → 換成真實照片 `images/bowls.jpg` | [ ] |
| FE4 | `.ph-bath` → 換成真實照片 `images/bath.jpg` | [ ] |
| FE5 | 加入「空間選物」區段（編輯感，非電商）：空間物件 / 日常香氛 / 生活好食 | [x] |
| FE6 | 部署至 GitHub Pages | [ ] |

---

## 檔案整理（需與使用者確認後執行）

| # | 項目 | 動作 |
|---|------|------|
| CL1 | `AlunaStudio.html`（舊前端）— 確認是否已由 index.html 取代 → 確認後 `trash` | 已刪除 |
| CL2 | `AlunaStudio-admin.html` — 確認功能是否已整合進工具台 → 確認後決定 | 已刪除 |
| CL3 | `承租人審核.html` — 獨立審核流程，工具台未取代 → 保留 | 保留 |

---

## 編輯後台｜AlunaStudio-admin.html

> 尚未分析，下一次工作台會先讀取此檔案列出優化清單。

---

*最後更新：2026-05-20*
