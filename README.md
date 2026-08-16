# Raspberry Pi 5 感測器影像調適繁中教學站

把 RPi5 上的 sensor 影像調適（sensor bring-up / ISP 管線 / 影像品質調校）做成**中英對照**的 16 單元分層教學，以 OmniVision 感測器（OV5647 / OV5640 / OV9281）為主要實例。

- 目標讀者：影像 / 韌體 / 相機工程師、學生
- 單元數：16（含 5 個影像調校專章 + 跨平台比較）
- 授權：本站內容 CC-BY-4.0
- 網站：https://shumingyang-opencode.github.io/rpi5-sensor-isp-zh-tw/

## 單元一覽

| # | 單元 | 內容 |
|---|------|------|
| 01 | 平台相機生態總覽 | CSI-2、libcamera、支援的 OV 感測器 |
| 02 | 影像感測器基礎 | Bayer、快門型態、感測器方塊 |
| 03 | 感測器通訊介面 | I2C/SCCB、register、OV 慣例 |
| 04 | 相機框架與驅動 | libcamera、unicam、DT overlay |
| 05 | 第一個鏡頭跑起來 | rpicam-apps 拍照與串流 |
| 06 | Sensor Bring-up 與除錯 | 上電、PLL、MIPI、register dump |
| 07 | ISP 管線深入 | black level → gamma |
| 08 | RAW 擷取與資料格式 | Bayer format、bit depth、ROI |
| 09 | 各平台 ISP 架構差異 | sensor 端 vs 平台 ISP |
| 10 | 曝光與自動曝光（AE） | shutter / gain / 測光 |
| 11 | 白平衡與色彩（AWB/CCM） | 色溫、gains、色彩校正 |
| 12 | 鏡頭陰影校正（LSC） | shading 成因與校正 |
| 13 | 雜訊與降噪 | NR 參數與取捨 |
| 14 | 清晰度/HDR/調校工作流 | tuning 檔與完整流程 |
| 15 | 四平台影像調校比較 | RPi5/Orange Pi/Orin/Thor |
| 16 | 多感測器與實作案例 | 客製 OV 接入、完整案例 |

## 開發

純靜態 HTML，無建置步驟。

```sh
python3 -m http.server 8000 -d .
```

## 相關連結

- 學習路徑建議服務：[learning-path-advisor](https://shuming-yang.github.io/learning-path-advisor/) — 依角色推薦教學網站學習路徑
