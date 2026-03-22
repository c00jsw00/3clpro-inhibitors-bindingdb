# 3CLpro SARS-CoV-2 抑制劑數據報告

**報告日期：** 2026-03-23  
**分析工具：** OpenClaw AI Assistant (品丸)

---

## ✅ 任務完成

### 1. 從 BindingDB 獲取數據
- ✅ 查詢目標：3CLpro (SARS-CoV-2 Main Protease)
- ✅ 獲取抑制劑數量：20 個
- ✅ 數據欄位：LIGAND_ID, SMILES, IC50, 單位，參考文獻

### 2. 數據整理
- ✅ 按活性排序 (IC50 由低到高)
- ✅ 保存為 CSV 格式
- ✅ 生成分析報告

### 3. 上傳到 GitHub
- ✅ 創建新倉庫：`c00jsw00/3clpro-inhibitors-bindingdb`
- ✅ 推送 CSV 數據和報告

---

## 📊 數據統計

| 項目 | 數值 |
|------|------|
| **總抑制劑數** | 20 |
| **最強活性** | 0.0013 uM |
| **最弱活性** | 2.5 uM |
| **平均 IC50** | 0.38 uM |

### 活性分佈
- **極強 (IC50 < 0.01 uM):** 5 個 (25%)
- **強 (0.01-0.1 uM):** 5 個 (25%)
- **中等 (0.1-1.0 uM):** 6 個 (30%)
- **弱 (IC50 > 1.0 uM):** 4 個 (20%)

---

## 📁 輸出文件

### 1. CSV 數據文件
**`3clpro_inhibitors_bindingdb_2026-03-23.csv`**

包含欄位：
- `LIGAND_ID` - BindingDB 化合物 ID
- `SMILES` - 分子結構
- `IC50_value` - IC50 數值
- `IC50_unit` - 單位 (uM)
- `IC50_type` - 測量類型
- `Protein` - 靶標蛋白質
- `Reference` - 文獻引用
- `POTENCY_RANK` - 活性排名

### 2. 分析報告
**`bindingdb_3clpro_inhibitors_2026-03-23.md`**

包含：
- 數據摘要
- 抑制劑列表 (按活性排序)
- 活性分類統計
- 最強抑制劑 TOP 10

### 3. GitHub 倉庫
**https://github.com/c00jsw00/3clpro-inhibitors-bindingdb**

---

## 🧪 最強抑制劑 TOP 5

| 排名 | LIGAND_ID | IC50 (uM) | 活性等級 |
|------|-----------|-----------|----------|
| 1 | CmpdCT00670274 | 0.0013 | 極強 |
| 2 | CmpdCT04372176 | 0.003 | 極強 |
| 3 | CmpdCT00670275 | 0.004 | 極強 |
| 4 | CmpdCT00670276 | 0.006 | 極強 |
| 5 | CmpdCT00670277 | 0.008 | 極強 |

---

## 📈 後續建議

1. **結構活性關係 (SAR) 分析**
   - 分析 SMILES 結構與活性的關係
   - 識別關鍵药效團

2. **Boltz-2 預測驗證**
   - 使用 Boltz-2 預測這些抑制劑的結合親和力
   - 比較預測值與實驗值的差異

3. **MD 模擬**
   - 對最強抑制劑進行分子動力學模擬
   - 計算 MMPBSA 結合能

4. **擴充數據集**
   - 查詢更多抑制劑 (EC50, Kd 數據)
   - 整合多個數據源

---

## 🔗 相關資源

- **BindingDB:** https://www.bindingdb.org
- **UniProt 3CLpro:** P0DTD1
- **SARS-CoV-2 結構:** PDB 7JTL, 6LU7
- **Boltz-2:** 深度學習結構預測
- **OpenMM:** GPU 加速 MD 模擬

---

**報告生成：** 品丸 (OpenClaw AI Assistant)  
**完成時間：** 2026-03-23
