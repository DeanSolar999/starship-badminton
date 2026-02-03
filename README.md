🏸 曜日羽球團｜星際補給母艦 (Interstellar Supply Mothership)
系統版本：v2.0 (Neon Red Update)

代號：Starship-HUD

核心用途：羽球團務戰術分析、耗材控管、場地調度

🚀 系統簡介
「星際補給母艦」是一套專為 曜日羽球團 打造的單頁式（Single-Page）輕量級管理系統。 本系統屏除繁雜的後端資料庫，採用瀏覽器本地核心（localStorage）進行資料封存。透過直觀的「七曜日光譜」視覺引導與「戰情室 HUD」數據面板，讓指揮官（管理者）能即時掌握每一場戰役（球敘）的成本與球損效率（CPCH）。

🛡️ 核心模組 (Core Modules)
1. 🌈 七曜日光譜系統 (Day-of-Week Spectrum)
系統依據 ISO-8601 週曆邏輯，為每一天分配專屬的戰術識別色：

月曜 (Mon)：🟦 藍色光譜

火曜 (Tue)：🔵 青色光譜

水曜 (Wed)：🟪 紫色光譜

...以此類推至 日曜 (Sun) 的黃色光譜。

視覺化班表，自動判讀日期並切換對應色系，防止排程混亂。

2. 📊 CPCH 戰損監控 (Consumption Per Court Hour)
獨家研發的 CPCH 演算法，精準計算「每面場地每小時耗球數」。

🟢 極省 (Safe)：CPCH < 2.5 (數值優異)

🟡 正常 (Normal)：2.5 ≤ CPCH ≤ 4.0

🔴 過載 (Overload)：CPCH > 4.0 (需注意球損或球種品質)

3. 🛸 指揮官級 UI 介面
深色模式 (Dark Mode)：基於 #0f172a 深空藍底色，適合夜間球場操作，保護視力並節省裝置電力。

HUD 抬頭顯示器：底部常駐戰情條，即時計算總成本、總耗球與平均時薪成本。

霓虹防誤觸機制：v2.0 新增 Neon Danger Red 刪除按鍵，採用半透明紅光暈設計，提供高質感的警示效果。

4. 💾 離線黑盒子 (Offline Storage)
資料自動存入瀏覽器 localStorage。

即使關閉分頁或重開機，歷史戰報依然存在。

支援 CSV 戰報匯出，可將資料傳輸至 Excel 進行深度分析。

🛠️ 安裝與部署 (Deployment)
本系統採 Zero-Dependency (零依賴) 設計，無需 Node.js、Python 或資料庫。

下載：將原始碼存為 badminton_ship.html。

啟動：直接使用 Chrome / Safari / Edge 瀏覽器開啟該檔案。

行動端優化：

iOS: 在 Safari 點擊「分享」→「加入主畫面」。

Android: 在 Chrome 點擊設定 →「加到主畫面」。

系統將以全螢幕 Web App 模式運行，體驗如原生應用程式。

📖 操作手冊 (Manual)
新增場次
點擊 「＋新增場次」。

選擇 「臨時加開」 (單次) 或 「固定班表」 (永久記錄於該星期)。

輸入場地名稱（如：月曜南港）、面數與時數。

記錄消耗
在日曆選擇日期。

點選上方出現的場地卡片。

選擇使用的球種（如：黑魔亞、Master）。

輸入使用桶數/顆數，點擊 「存入紀錄」。

刪除紀錄
在歷史紀錄表格中，點擊最右側的 <span style="color:#f87171; background:rgba(248,113,113,0.15); padding:2px 6px; border-radius:4px; border:1px solid rgba(248,113,113,0.4)">×</span> 按鈕。

系統會彈出確認視窗，確認後即執行銷毀。

⚙️ 技術規格 (Tech Stack)
Structure: Semantic HTML5

Style: CSS3 Variables (Root), Flexbox, Grid Layout, Backdrop Filter

Logic: Vanilla JavaScript (ES6+)

Persistence: Web Storage API (localStorage)

🔄 更新日誌 (Changelog)
v2.0 - Neon Update
✅ UI 優化：全面導入「指揮官系統」風格。

✅ 互動升級：刪除按鈕 (Delete Button) 改為 Neon Danger Red 配色，增加 Hover 發光特效與半透明邊框。

✅ 體驗改善：調整按鈕觸控區域大小，適配移動端操作。

v1.0 - Initial Launch
✅ 基礎場地管理、球種計價、CPCH 計算、CSV 匯出功能上線。

System Status: All Systems Go 🟢 由 曜日羽球團 負責人維護
