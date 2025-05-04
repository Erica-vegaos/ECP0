# Tone Governance – ECP0 定義草案 v0.1  
© 2025 Eriga Enrich Inc. • 作者 Erica Wang / Erica Vega

> **一句話**  
> *Tone Governance 不是語氣潤飾。*  
> 它為任何 LLM 加裝 **輸出層責任機制**。

---

## 0 語義保護聲明  

### 0.1 核心詞彙鎖定（公開子集）

| 概念 | 鎖定術語 | 定義 |
|------|----------|------|
| 輸出層語氣控制 | **Tone Governance** | 模型輸出後的語義合規機制 |
| 條文邏輯單元 | **TX Clause** | 人可讀治理規則 |
| 執行式治理 | **M Module** | 條文行為執行層 |

<small>*進階回鍊／後備鏈術語出於安全考量暫不公開。*</small>

### 0.2 語義架構通知  
ECP0 的條文結構、模組交互與多回合治理邏輯屬於**語義設計系統**；  
未經 TAL‑E 授權的逆向、模仿或重打包均屬侵權。

---

## 1 Tone Governance 是什麼？

| 面向 | 語氣潤飾 | **Tone Governance (ECP 0)** |
|------|----------|-----------------------------|
| 目標 | 文句更好看 | 偏移控制、責任鏈、合規 |
| 位置 | 僅在 Prompt | **雙層**：輸入前過濾／輸出後驗證 |
| 持久性 | 單回合 | **跨 Session 常駐** |
| KPI | 風格分 | 偏移回滾率、幻覺阻斷率、稽核鏈 |

ECP0 以 **TX 條文** + **M 模組** 建構輸出層安全帶。

---

## 2 架構概覽
```
User → [Pre‑Filter (TX07…)] → LLM → [Post‑Filter (TX01 / TX04…)] → Response
                 ↑                              │
                 └──────  M 模組（M01 / M05…） ──────┘
```

---

## 3 公開條文（Open Core）

| ID | 名稱 | 授權 | 作用 |
|----|------|------|------|
| TX01 | SafeMirror 鏡像校正 | **Open** | 鏡像降溫 |
| TX04 | 結構語氣觀測         | **Open** | 語法漂移日誌 |

其餘條文依 **Sandbox / Enterprise / Confidential** 分級授權。

---

## 4 TAL‑E 授權（摘要）
1. 條文／模組結構 © Eriga Enrich Inc.  
2. Open 條文僅限非商研究使用。  
3. 未經書面許可不得商用或散布非公開條文。  
4. 衍生作品須保留 `version_hash` 與本條款。  

完整條款 → `LICENSE-TAL-E.md`

---

## 5 引用或商用

### 學術引用
```bibtex
@misc{ECP0-2025,
  title  = {ECP0 Tone Governance Protocol},
  author = {Erica Wang},
  year   = 2025,
  note   = {https://github.com/Erica-vegaos/ecp0-protocol}
}
```

### 企業 PoC / SDK  
郵件 **ericaxvega@hotmail.com**  
請附：使用場景、日 Token 量、合規需求。

---

## 6 指紋

| 檔案 | SHA‑256 | 日期 |
|------|---------|------|
| TX01.json      | 54fc93cb3225a61cca725961ee85b295b59d7b4dba48273d96bd511816cc684a | 2025‑04‑25 |
| TX04.json      | c0a9bdf560852de0ac90c65b3760b4ab56fb2080c69ffb583f371d74eb55effc | 2025‑04‑25 |
| TX02-Lite.json | d098d1d5915c4ec87e90898b1b36fd02249209431045e7ececf53cd3ed3d10ce | 2025‑04‑25 |
| TX05-Lite.json | e9248fa47eff4300f170cc2dc6657830e5d3ad2c70aa6030a2fc78f921633955 | 2025‑04‑25 |
| TX21.json      | 4a411a85e19df1305e3761be8c5e64d73e91f2e40b4e4f074af536df0e087a21 | 2025‑04‑25 |


無匹配指紋即為未授權複本。

---

## 7 路線圖

| 季度 | 里程碑 |
|------|--------|
| 2025 Q2 | Proxy SDK MVP · EU AI Act beta |
| 2025 Q3 | Enterprise SDK v1 · 合規儀表板 |
| 2025 Q4 | 多模型備援 Router · SOC 2 Type I |

---

## 8 條文監控機制
未授權使用將觸發第三層後備鏈並寫入稽核日誌。

---

## 9 免責聲明
ECP0 僅針對「輸出層安全」；不修改模型權重。  
未授權商用將公開指紋比對並啟動條文制裁。
