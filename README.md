# 碳化矽 (Silicon Carbide, SiC) 論文、專利與新聞自動化搜索系統 (Arena.ai Agent Mode)

本系統致力於自動搜尋、解析與彙整最近 3 個月內（即 **2026 年 5 月至 7 月**）全球碳化矽（SiC）相關的權威學術論文 ("paper"、"review"、"journal"、"research") 與專利、產業動態新聞。

---

## 系統特色與功能亮點

1. **多語系文獻覆蓋**：全面涵蓋 **英文 (English)**、**中文 (Chinese)**、**日文 (Japanese)** 三大語系之核心學術成果與專利動態。
2. **權威學術資料庫映射**：整合並提供至少 2 個主要資料庫的查詢 URL：
   - **Google Scholar (學術搜尋)**：`https://scholar.google.com/scholar?q="%22[關鍵字]%22&as_ylo=2026&scisbd=1"`
   - **ScienceDirect (Elsevier)**：`https://www.sciencedirect.com/search?qs=[關鍵字]`
3. **19 項核心關鍵字全域查詢**：
   - `Silicon Carbide COMSOL`
   - `Silicon Carbide Crystal`
   - `Silicon Carbide growth`
   - `Silicon Carbide simulation`
   - `Silicon Carbide 12inch`
   - `Silicon Carbide 8inch`
   - `Silicon Carbide 300mm`
   - `Silicon Carbide 200mm`
   - `Silicon Carbide DEFECT`
   - `Silicon Carbide n-type`
   - `Silicon Carbide p-type`
   - `Silicon Carbide machine learning`
   - `Silicon Carbide yolo`
   - `Silicon Carbide deep learning`
   - `Silicon Carbide 4H`
   - `Silicon Carbide Semi-insulating`
   - `Silicon Carbide STR`
   - `Silicon Carbide furnance` (及常見修正詞 `furnace`)
   - `Silicon Carbide patent`
   - `Silicon Carbide Semi-insulating` (依需求支援二次重點檢索)
4. **完整的參考網址與 PDF 指引**：每則論文與專利紀錄均提供完整 HTTP / HTTPS 原始參考連結，並附帶對應之 PDF 下載 / 全文檢索頁面連結及 `pdfs/` 本機摘要參考文檔。
5. **純 Markdown 格式輸出**：所有產出的報告、簡介索引與對照表均採用 Markdown (`.md`) 結構化格式，排版清晰易讀。
6. **全體繁體中文說明**：包括標題、文獻摘要、核心結論與圖表說明均採用繁體中文撰寫。
7. **日期專屬資料夾自動化建立**：每次調用腳本運行時，自動按該執行日期（`YYYY-MM-DD`）建立專屬成果資料夾（本此執行已生成 [`2026-07-29/`](./2026-07-29) 目錄）。

---

## 快速使用指引

### 1. 執行自動搜索與報告生成腳本
直接執行專案根目錄下之 Python 腳本：

```bash
python3 sic_paper_searcher.py
```

或指定任意自訂日期：
```bash
python3 sic_paper_searcher.py --date 2026-07-29
```

### 2. 產出成果架構說明（以 2026-07-29 為例）
執行完畢後，系統將自動於工作目錄建立如下結構：

```
2026-07-29/
├── SiC_Research_and_Patent_Report_2026-07-29.md  # 完整 48 篇論文/專利新聞詳細報告
├── README.md                                     # 當日搜尋任務總覽與索引
├── keyword_urls.md                               # 19 項關鍵字之 Google Scholar 與 ScienceDirect 自動搜尋連結表
└── pdfs/                                         # 重點文獻/專利 PDF 指引及參考摘要檔案 (含 48 個參考紀錄檔)
```

---

## 本次（2026-07-29）檢索總覽與重大發現摘要

於本次 `2026-07-29` 測試執行中，共收錄並分類 **48 則** 最近 3 個月內的 SiC 關鍵學術報告與專利突破，重點結論如下：
- **300mm (12 英寸) 碳化矽單晶晶圓正式進入商用化里程碑**：以 Wolfspeed 在 2026 年初發表 300mm 單晶 SiC 晶圓及 2,300 餘項專利佈局為首，確立了將碳化矽拓展至 AI 基礎設施與高壓直流充電領域的基礎。
- **深度學習與 YOLO 物體偵測模型普及於晶圓無損檢測**：多篇最新 2026 年期刊論文（如 *ScienceDirect / Diamond and Related Materials* 及 *MDPI Micromachines*）展示了 **YOLO11-OBB**、**YOLO26** 及視覺-語言對齊（**YOLO-LA**）在 4H-SiC 基底面位錯 (BPDs) 和微管檢測上的領先準確率。
- **熱場模擬 (COMSOL / STR) 為 8/12 英寸長晶裝備改進之依據**：新型雙瓣式電阻加熱長晶爐與退火工藝大幅降低了大尺寸碳化矽晶片生長時的固液介面熱應力。

歡迎點擊 [`2026-07-29/SiC_Research_and_Patent_Report_2026-07-29.md`](./2026-07-29/SiC_Research_and_Patent_Report_2026-07-29.md) 查看所有文獻完整內容。
