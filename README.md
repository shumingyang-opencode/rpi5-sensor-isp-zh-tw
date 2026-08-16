# Raspberry Pi 5 感測器影像調適繁中教學站

手把手把 RPi5 上的 OV5647 感測器**初始化 → streaming → 調校**的深度實作教學（16 單元，中英對照）。

- 目標讀者：影像 / 韌體 / 相機工程師、學生
- 授權：本站內容 CC-BY-4.0
- 網站：https://shumingyang-opencode.github.io/rpi5-sensor-isp-zh-tw/

## 單元一覽

| # | 單元 | 深度重點 |
|---|------|---------|
| 01 | 平台相機生態總覽 | CSI-2、libcamera 堆疊、感測器選擇 |
| 02 | 影像感測器基礎 | Bayer、快門、感測器方塊、OV5647 規格 |
| 03 | 感測器通訊介面 | I2C 實作、讀 ID、register 讀寫、page |
| 04 | 相機框架與驅動 | libcamera 架構、unicam、DT overlay |
| 05 | 第一個鏡頭跑起來 | rpicam-apps 完整流程、RAW 擷取 |
| 06 | Sensor Bring-up 與除錯 | 上電時序、PLL、media 管線、決策樹 |
| 07 | ISP 管線深入 | 每個區塊 + 對應調校參數 |
| 08 | RAW 擷取與資料格式 | Bayer format、bit depth、RAW 分析 |
| 09 | 各平台 ISP 架構差異 | sensor 端 vs 平台 ISP |
| 10 | 曝光與自動曝光（AE） | 曝光 register、AE 收斂、測光 |
| 11 | 白平衡與色彩（AWB/CCM） | gains、CCM、色彩調校實作 |
| 12 | 鏡頭陰影校正（LSC） | 成因、網格、實作校正 |
| 13 | 雜訊與降噪 | 來源、NR 調校、DPC |
| 14 | 清晰度/HDR/調校工作流 | tuning 檔解析、完整流程 |
| 15 | 四平台影像調校比較 | 能力/工具鏈對照 |
| 16 | 多感測器與實作案例 | 客製 OV 接入、完整案例 |

## 開發

純靜態 HTML，無建置步驟。

```sh
python3 -m http.server 8000 -d .
```

## 相關連結

- 學習路徑建議服務：[learning-path-advisor](https://shuming-yang.github.io/learning-path-advisor/) — 依角色推薦教學網站學習路徑
