# YYB Hatsune Miku NT - SPA Hair 2.0 (Ray-MMD Preset)

適用於 MMD（MikuMikuDance）中 **Ray-MMD 1.5.2** 渲染引擎的頭髮材質預設（Matcap / SPA），適配模型為 **YYB 式 初音未來 NT（YYB Hatsune Miku NT）**。

---

## 📌 專案說明 (Overview)

本專案提供了一套針對 YYB Hatsune Miku NT 模型頭髮部分的高品質 Ray-MMD 材質配置文件與專用 Matcap 擴展，透過 `SJ_Matcap` 乘算 Sph 效果增強頭髮的高光質感、陰影過渡與立體層次。

### 包含內容 (Included Assets)
- **Shader 檔案**：
  - `Hair01_SJ_Matcap.fx` / `Hair01_SO_SJ_Matcap.fx`
  - `Hair02_SJ_Matcap.fx` / `Hair02_SO_SJ_Matcap.fx`
  - `Hair03_SJ_Matcap.fx` / `Hair03_SO_SJ_Matcap.fx`
  - `material_common_2.0.fxsub`
  - `SJ_Matcap_1.0(152).fxsub` (Ray-MMD Matcap 擴展腳本)
- **貼圖檔案**：
  - `Hair01.png`, `Hair01-ao.png`, `Hair01_normal.png`
  - `Hair02.png`, `Hair02-ao.png`, `Hair02_normal.png`
  - `Hair03.png`, `Hair03-ao.png`, `Hair03_normal.png`
  - `Gemstone14.png` (Matcap 貼圖)

> **註**：`_SO_` 版本包含 AO（環境光遮蔽）配置映射，可依照渲染場景的光影需求選擇使用。

---

## 📖 借物表與版權聲明 (Credits & Disclaimers)

本倉庫發布之內容涉及多方創作者之著作與智慧財產權，在引用或渲染發布作品時請務必標明借物表：

| 項目 | 創作者 / 權利方 | 說明 |
| :--- | :--- | :--- |
| **Character IP** | **Crypton Future Media, INC.** | 初音ミク (Hatsune Miku) 角色形象依據 Piapro 角色使用規範。 |
| **Model / Textures** | **三目YYB** | YYB 式初音未來 NT 模型原始貼圖與 UV 對應。 |
| **Shader Core** | **Rui** | [Ray-MMD](https://github.com/ray-cast/ray-mmd) (Physically-Based Rendering for MMD)。 |
| **Matcap Extension** | **三金络合物** | Ray用乘算Sph材質 // SJ_Matcap ver 1.1(152)。 |
| **Matcap Texture** | **Gemstone14** | 寶石球高光反射貼圖。 |

---

## ⚖️ 使用規約 (Terms of Use)

本專案**非一般開源代碼**，所有使用者必須嚴格遵守以下條款：

1. **嚴禁商業利用 (Strictly Non-Commercial)**：任何個人或團體不得將本專案全部或部分內容用於盈利活動、販賣或商業廣告。
2. **禁止未授權二次配布 (No Redistribution)**：請勿將本材質包中的貼圖或著色器原樣轉載至收費平台或未經授權的第三方資源站。
3. **標註借物表 (Credits Required)**：在任何公開發布的靜畫、動畫或 MMD 渲染影片中，必須註明上述 **借物表（三目YYB、三金络合物、Ray-MMD 等）**。
4. **禁止違反公序良俗與政治/宗教用途**。

---

## 🚀 使用方法 (How to Use)

1. **準備環境**：
   - 確保已安裝 **MikuMikuDance (MMD)** 與 **MikuMikuEffect (MME)**。
   - 載入 **Ray-MMD 1.5.2** 主特效（`ray.x`）。
2. **載入模型**：
   - 在 MMD 中載入 YYB Hatsune Miku NT 模型。
3. **分配材質**：
   - 開啟 MME 效果視窗，切換至 **`MaterialMap`** 分頁。
   - 找到初音未來頭髮對應的材質部位（通常為 `Hair01`、`Hair02`、`Hair03`）。
   - 對應套用本資料夾內的 `Hair01_SJ_Matcap.fx`（或 `_SO_` 版本）。
4. **預覽與調整**：
   - 在 MMD 控制面板中調整光照角度與相機角度，即可呈現 Matcap 寶石高光與髮絲光影。
