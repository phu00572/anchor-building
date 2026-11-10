# 固定點架設｜SREDDA・分力與均力・夾角、腿長與偏離受力

HTML 互動式簡報（Reveal.js＋Firebase 即時互動），合併「台灣山難事故及高風險環境發生案例與救援方法」研討會簡報的做法（純中文版）：23 頁內容＋文字雲＋共享白板＋投票＋結尾，全場建議 23 分 50 秒。

- **線上網址**：https://phu00572.github.io/anchor-building/
- **章節**：引起動機（封面、文字雲、北絲鬮溪案例）→ 維持注意（SREDDA、受力方向會變、單一強壯固定點、分力均力、三個點的分配、共享白板、夾角受力）→ 喚起行動（甜蜜點、腿長原理與計算器、偏離點／COD 強度值、現場檢核）

## 鍵盤快捷鍵

| 按鍵 | 功能 |
|------|------|
| → / ← | 下一頁／上一頁 |
| F | 全螢幕 |
| N | 講稿面板＋計時器（第一次按下開始計時，目標 23:50） |
| T | 計時器歸零 |
| S | Reveal 講者視窗（另開視窗，顯示講稿與下一頁） |

## 聽眾互動（Firebase，SLUG `anchor2026`）

- **封面 QR code**：手機掃描直接進入文字雲頁；投票頁另有 QR code 直達投票。
- **文字雲**：「架設固定點時，你第一個檢查什麼？」
- **共享白板「換你架架看」**：A、B、C 三個固定點、往下受力，學員用手機畫出連法，筆畫即時同步；可「復原我的上一筆」，講者電腦上可「清空全部」。白板頁有 QR code 直達。
- **投票「先猜再看」**：兩點分力夾角多少最理想？講者按「揭曉答案」標出正解（C　45°～60°）。
- **匿名提問牆**：每一頁左側都可以拉開，可互相按讚。
- **課後清空資料**：網址加 `?reset=1`（https://phu00572.github.io/anchor-building/?reset=1），確認後清空文字雲、投票、提問牆與白板。

## 頁面互動

案例卡、SREDDA 卡、架設方式卡（含單一強壯固定點六種架法）可點擊展開；對照表可點選列標示；角度實驗室可拖拉夾角與偏離角；最後一頁是可勾選的現場檢核清單。三個點的分配頁可切換「兩點先串接（25/25/50）」與「三腳各自到主力點」（左圖同步換成三點 BFK）。腿長計算器可選範例（日文教材圖 3、圖 4、1·2·3 ft、等長）、負荷與腳數，拖拉腳長看各腳 kgf。偏離點（COD）頁點選任一列（偏離角 10°～180°），右邊示意圖會跟著改變。各頁左側圖片點一下可全螢幕放大。

## 照片與圖檔（`images/photos/`）

P10、P11 卡片上的「真實照片」按鈕：

把照片存到 `images/photos/`，檔名對應如下（JPG，最長邊約 1600px）；同一種架法可放 2～4 張，加 `-2`、`-3`、`-4`：

| 卡片 | 檔名 |
|------|------|
| Y-hang | `y-hang.jpg` |
| 雙耳 8 字結 | `fig8-ears.jpg` |
| 雀頭結 Girth Hitch | `girth-hitch.jpg` |
| BFK | `bfk.jpg` |
| Sliding X＋限制結 | `sliding-x.jpg` |
| The Quad | `quad.jpg` |

六張卡片都已放入照片（BFK 有 2 張）。沒有照片的卡片，按鈕會顯示「照片待補」（聽眾版 `?clean` 會隱藏）。要換照片或加張數，覆蓋檔案後推送即可，不必改程式。P10 單一強壯固定點的「真實照片」：`single-basket.jpg`（繩圈雙環）、`single-girth.jpg`（雀頭結）、`single-base.jpg`／`-2`／`-3`（基部固定）、`single-fig8.jpg`（8 字結＋自我確保）、`single-clove.jpg`（雙套結＋自我確保）、`single-mmo.jpg`（MMO）。其他頁面的圖：`angle-force.jpg`（P5 夾角受力卡）、`direction.jpg`（受力方向會變）、`three.jpg`／`three-2.jpg`（三個點的分配）、`legs.jpg`／`legs-2.jpg`（腿長原理）、`legs-jp.jpg`／`legs-jp-2.jpg`（計算器的圖 3、圖 4）、`cod.jpg`（Deviation Forces）。

## 講稿與講義

- [講稿.pdf](講稿.pdf)：每頁附簡報畫面、建議秒數與中文講稿（共 27 頁）
- [簡報講義_聽眾版.pdf](簡報講義_聽眾版.pdf)：隱藏操作介面、展開所有點擊內容
- 截圖模式：網址加 `?shot`（關閉動畫）；聽眾版：加 `?clean`
- 改完內容後，在上一層資料夾執行 `python make_handouts.py` 重新產生兩份 PDF（會從線上網址截圖，請先推送部署）

## 資料來源

- 夾角與偏離 5° 受力：Grant Prattley〈Two-Point Anchor Angles: The Case for Building in Error〉Over The Edge Rescue（2025）
- A.D.D.R.E.S.S：ZA Adventure（2013）；ERNEST：Rigging Lab Academy；SRENEA：2024 中華山岳傳攀課程表
- 腿長與受力：John Long & Bob Gaines《Climbing Anchors》（cordelette 1/2/3 ft 圖）；日文教材圖 3、圖 4（700 kgF 計算例）；Kevin Heinrich〈The Best Climbing Anchor: A Look at Anchor Research〉；Chasse（2016）〈Revisiting the Quad for Load Distribution and Stance Management〉Rock and Ice；Beverly et al.（2005）〈Multi-point Pre-Equalized Anchoring Systems〉。計算器以虎克定律「受力與腳長成反比」計算（同材質、各腳接近平行、不計結的鬆弛）
- 夾角受力卡（P5）：KASK／Singing Rock（數值＝100 ÷（2 × cos（夾角÷2）），已驗算）
- 偏離點（COD）受力：以偏離角 θ 表示（直線 0°、完全折返 180°），F = 2T·sin(θ/2)（兩側張力相同、不計摩擦）；圖：Deviation Forces
- 北絲鬮溪事故：臺東縣消防局新聞稿與同行隊友事故紀錄（2025-05）
