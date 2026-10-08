# 傳奇卡牌工坊｜3D 鐳射全息卡牌展示系統

> **入口檔案**：`index.html`  
> **專屬立繪**：`card_art.jpg`  
> **部署相容**：GitHub Pages 零建置依賴直推即用

---

## 專案特色

1. **TCG 黃金比例與 RWD 佈局**：
   - 遵循標準卡牌比例（`aspect-ratio: 63 / 88`）。
   - 桌面端（≥ 1024px）雙欄並排（3D 卡牌舞台 ＋ 磨砂玻璃控制台）。
   - 行動端（< 768px）自動切換垂直堆疊，卡牌居頂、控制收底。

2. **3D 物理視差與動態雷射系統**：
   - CSS 3D Transform（`perspective: 1200px`、`preserve-3d`）搭配 60/120fps LERP 物理阻尼平滑跟隨。
   - 4 種鐳射箔膜切換（Cosmos Holo 宇宙彩虹、Rainbow Secret 極光全息、Gold Ultra 黑金浮雕、Silver Phantom 冷冽銀鏡）。
   - 支援滑鼠游標、手機觸控滑動、陀螺儀（`DeviceOrientationEvent`）動態傾斜。

3. **零依賴與全功能控制台**：
   - 卡面所有文字支援 `contenteditable="true"` 即時編輯。
   - 支援 FileReader API 本機圖片立繪上傳與一鍵還原。
   - 支援 3D 180 度翻轉檢視官方認證卡背。
   - 整合 `html2canvas` 實作一鍵匯出 3x 高解析度無損 PNG。

---

## 部署至 GitHub Pages

1. 將本專案中的 `index.html` 與 `card_art.jpg` 上傳至 GitHub 儲存庫。
2. 進入 Repository 的 **Settings** -> **Pages**。
3. Source 選擇 **Deploy from a branch**，分支選擇 `main` / `root`。
4. 儲存後數十秒即可完成部署！
