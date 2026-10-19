<div align="center">

# ⚖️ Indian Legal Knowledge Base (v3.0)
### Complete Structured JSON Corpus: 112 Files | 102 Primary Acts & Codes | 12,174 Sections

<p align="center">
  <b>The definitive, authoritative, machine-readable statutory corpus of India — featuring the complete 2026 Constitution of India, modern 2023 Criminal Codes (BNS, BNSS, BSA), historical repealed codes (IPC, CrPC, IEA), unified labor codes, direct taxation (Income-tax Act, 2025), securities regulations (SEBI & SCRA), telecommunications, and 92 specialized statutes across 13 legal domains.</b>
</p>

<!-- Shields / Badges -->
[![Corpus Size](https://img.shields.io/badge/Corpus%20Size-112%20Files%20%7C%20102%20Acts%20%7C%2012%2C174%20Sections-blue.svg?style=for-the-badge&logo=balance-scale)](https://huggingface.co/datasets/GSMS-B/indian-legal-knowledge-base-json)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-amber.svg?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/)
[![Official Source](https://img.shields.io/badge/Source-Gazette%20of%20India%20%7C%20India%20Code-emerald.svg?style=for-the-badge)](https://www.indiacode.nic.in/)
[![Format](https://img.shields.io/badge/Format-JSON%20%2F%20JSONL-orange.svg?style=for-the-badge&logo=json)](https://huggingface.co/datasets/GSMS-B/indian-legal-knowledge-base-json)
[![MCP Space](https://img.shields.io/badge/%F0%9F%A4%97%20Space-Indian%20Legal%20MCP-red.svg?style=for-the-badge)](https://huggingface.co/spaces/GSMS-B/indian-legal-mcp)

<br>

<img src="assets/poster.png" alt="Indian Legal Knowledge Base Poster" width="100%" />

</div>

---

> ### 🔗 Ecosystem Navigation
> - 📜 **Companion PDF Dataset:** For original Gazette of India and India Code source PDF publications, visit **[Indian Legal Knowledge Base (Official Source PDFs)](https://huggingface.co/datasets/GSMS-B/indian-legal-knowledge-base-pdf)**.
> - ⚡ **Live Model Context Protocol (MCP) Server:** Connect this corpus directly to Claude, ChatGPT, Cursor, or any agentic system using the **[Indian Legal MCP Server](https://huggingface.co/spaces/GSMS-B/indian-legal-mcp)**.

---

## 📚 What is Included?

The repository contains **112 structured data files** in `raw_acts/` plus the master consolidated file `sections.json`:

1. **Master Consolidated File**: `sections.json` (19.0 MB) containing all **12,174 sections across all 102 statutes** with uniform keys (`act_code`, `chapter_number`, `chapter_title`, `section_number`, `section_title`, `text`).
2. **102 Individual Statute Files**: Structured JSON for each statutory enactment with clean Roman chapters and sections.
3. **6 Criminal Concordance Mapping Tables**: Bi-directional section-to-section crosswalks:
   - `bns_to_ipc.json` & `ipc_to_bns.json` (Bharatiya Nyaya Sanhita $\leftrightarrow$ Indian Penal Code)
   - `bnss_to_crpc.json` & `crpc_to_bnss.json` (Bharatiya Nagarik Suraksha Sanhita $\leftrightarrow$ Code of Criminal Procedure)
   - `bsa_to_iea.json` & `iea_to_bsa.json` (Bharatiya Sakshya Adhiniyam $\leftrightarrow$ Indian Evidence Act)
4. **4 Constitutional Data Files**:
   - `CONSTITUTION_DATASET.json` & `constitution_of_india.json`
   - `constitution_of_india_articles.jsonl` (Articles 1–395 & Preamble)
   - `constitution_of_india_schedules.jsonl` (All 12 Schedules)
   - `constitution_of_india_appendices.jsonl` (All 3 Appendices)

---

## 🏛️ Domain Breakdown Summary (102 Acts, 12,174 Sections)

| Category / Domain | Statutes Count | Total Sections |
|---|:---:|:---:|
| Criminal Law & Penal Statutes | 14 | 2,784 |
| Constitutional Law & Public Administration | 9 | 992 |
| Commercial, Corporate & Financial Law | 14 | 1,731 |
| Banking, Finance & Revenue | 16 | 2,181 |
| Civil Procedure, Contracts & Property | 9 | 1,197 |
| Unified Labor Codes | 5 | 505 |
| Cyber, Technology, Telecom & Identity | 4 | 297 |
| Intellectual Property Rights (IPR) | 5 | 586 |
| Family & Personal Laws | 10 | 661 |
| Environmental & Green Law | 6 | 385 |
| Public Health, Healthcare & Food Safety | 3 | 315 |
| Social Protection, Education & Human Welfare | 6 | 352 |
| Energy, Infrastructure & Public Utilities | 1 | 188 |
| **Total** | **102** | **12,174** |

---

## 📊 Usage in Python

```python
import json

# Load master consolidated corpus (12,174 sections)
with open("sections.json", "r", encoding="utf-8") as f:
    corpus = json.load(f)

print(f"Total sections loaded: {len(corpus)}")

# Query provisions for a specific statute (e.g. SEBI Act, 1992)
sebi_sections = [s for s in corpus if s["act_code"] == "SEBI"]
print(f"SEBI Act sections: {len(sebi_sections)}")
```

---

## ⚖️ Legal Disclaimer

> **Important Notice:** This dataset is provided strictly for academic research, legal NLP, RAG benchmarks, and informational purposes. While verified against official government gazettes and India Code repositories, it does **not** constitute formal legal advice. For active litigation, commercial contracts, or compliance filings, always consult licensed advocates and cross-verify with the official Gazette of India (indiacode.nic.in).

## 👤 Curator & Citation

Curated with dedication by **GSMS-B**.

```bibtex
@dataset{indian_legal_knowledge_base_2026,
  author       = {GSMS-B},
  title        = {Indian Legal Knowledge Base: Complete Structured JSON Corpus of 102 Indian Acts and Codes (112 Structured Files, 12,174 Sections)},
  year         = {2026},
  publisher    = {Hugging Face},
  version      = {3.0.0},
  url          = {https://huggingface.co/datasets/GSMS-B/indian-legal-knowledge-base-json}
}
```

---

<div align="center">

## 👨‍💻 Created & Curated by **GSMS-B**

**Built with dedication for Indian Legal AI Researchers, NLP Practitioners, and Legal Scholars Worldwide.**

[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-GSMS--B-orange.svg?style=for-the-badge)](https://huggingface.co/GSMS-B)
[![GitHub](https://img.shields.io/badge/GitHub-GSMS--B-181717.svg?style=for-the-badge&logo=github)](https://github.com/GSMS-B)
[![Live MCP Server](https://img.shields.io/badge/Model%20Context%20Protocol-Indian%20Legal%20MCP-blue.svg?style=for-the-badge)](https://huggingface.co/spaces/GSMS-B/indian-legal-mcp)

*“Empowering democratic access to the laws of India through open, authoritative, and structured AI intelligence.”*

</div>