<div align="center">

# ⚖️ Indian Legal Knowledge Base (v3.0)
### Complete Structured JSON Corpus of 102 Indian Acts & Codes (12,174 Sections)

<p align="center">
  <b>The definitive, authoritative, machine-readable statutory corpus of India — featuring the complete 2026 Constitution of India, modern 2023 Criminal Codes (BNS, BNSS, BSA), historical repealed codes (IPC, CrPC, IEA), unified labor codes, direct taxation (Income-tax Act, 2025), securities regulations (SEBI & SCRA), telecommunications, and 92 specialized statutes across 13 legal domains.</b>
</p>

<!-- Shields / Badges -->
[![Corpus Size](https://img.shields.io/badge/Corpus%20Size-102%20Acts%20%7C%2012%2C174%20Sections-blue.svg?style=for-the-badge&logo=balance-scale)](https://huggingface.co/datasets/GSMS-B/indian-legal-knowledge-base-json)
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

## 📖 Overview

The **Indian Legal Knowledge Base (JSON Corpus)** is an open-access, research-grade legal dataset meticulously curated for Natural Language Processing (NLP), Large Language Model (LLM) fine-tuning, Retrieval-Augmented Generation (RAG), and agentic legal tools.

Unlike raw or unstructured web scrapes, every section in this dataset has been extracted and normalized from official Gazette notifications and India Code publications with:
- **Exact chapter grouping, numerical ordering, and official headnotes.**
- **Accurate legislative amendments (including the modern criminal law reform effective July 1, 2024 and direct tax modernization under the Income-tax Act, 2025).**
- **2,629 bidirectional concordance mappings cross-referencing old and new criminal provisions.**
- **Complete constitutional framework incorporating the 106th Constitutional Amendment Act.**

---

## 📁 Repository Structure

```text
├── sections.json                  # Master consolidated file (17.5 MB) containing all 12,174 sections across 102 Acts
├── raw_acts/                      # Directory of 102 individual standalone Act JSON files + Concordance tables
│   ├── bharatiya_nyaya_sanhita_2023.json
│   ├── constitution_of_india_1950.json
│   ├── the_companies_act_2013.json
│   ├── income_tax_act_2025.json
│   ├── ... (102 Act JSONs)
│   ├── bns_to_ipc.json            # BNS (2023) -> IPC (1860) concordance table
│   ├── ipc_to_bns.json            # IPC (1860) -> BNS (2023) concordance table
│   ├── bnss_to_crpc.json          # BNSS (2023) -> CrPC (1973) concordance table
│   ├── crpc_to_bnss.json          # CrPC (1973) -> BNSS (2023) concordance table
│   ├── bsa_to_iea.json            # BSA (2023) -> IEA (1872) concordance table
│   ├── iea_to_bsa.json            # IEA (1872) -> BSA (2023) concordance table
│   ├── schedules.jsonl            # 12 Constitution Schedules (First to Twelfth)
│   └── appendices.jsonl           # 3 Constitution Appendices (I, II, III)
└── assets/
    └── poster.png                 # Official repository visual graphic
```

---

## 📚 Complete Catalogue of Covered Acts (102 Statutes in 13 Domains)

| Domain | Act Code | Official Statute Name | Enacted | Total Sections |
|---|---|---|:---:|:---:|
| **Criminal Law & Penal Statutes** | `ARMS` | Arms Act, 1959 | 1959 | 48 |
|  | `BNS` | Bharatiya Nyaya Sanhita, 2023 | 2023 | 358 |
|  | `BNSS` | Bharatiya Nagarik Suraksha Sanhita, 2023 | 2023 | 531 |
|  | `BSA` | Bharatiya Sakshya Adhiniyam, 2023 | 2023 | 170 |
|  | `CONTEMPT_COURTS` | Contempt of Courts Act, 1971 | 1971 | 24 |
|  | `CRPC` | Code of Criminal Procedure, 1973 | 1973 | 525 |
|  | `DPA` | Dowry Prohibition Act, 1961 | 1961 | 12 |
|  | `IEA` | Indian Evidence Act, 1872 | 1872 | 184 |
|  | `IPC` | Indian Penal Code, 1860 | 1860 | 575 |
|  | `NDPS` | Narcotic Drugs and Psychotropic Substances Act, 1985 | 1985 | 127 |
|  | `PCA` | Prevention of Corruption Act, 1988 | 1988 | 35 |
|  | `PMLA` | Prevention of Money Laundering Act, 2002 | 2002 | 81 |
|  | `POCSO` | Protection of Children from Sexual Offences Act, 2012 | 2012 | 47 |
|  | `UAPA` | Unlawful Activities (Prevention) Act, 1967 | 1967 | 67 |
| **Constitutional Law & Public Administration** | `ADVOCATES` | Advocates Act, 1961 | 1961 | 85 |
|  | `ATA` | Administrative Tribunals Act, 1985 | 1985 | 41 |
|  | `COI` | Constitution of India (2026 Edition) | 1950 | 507 |
|  | `LSAA` | Legal Services Authorities Act, 1987 | 1987 | 38 |
|  | `PCRA` | Protection of Civil Rights Act, 1955 | 1955 | 23 |
|  | `PHRA` | Protection of Human Rights Act, 1993 | 1993 | 45 |
|  | `RPA` | Representation of the People Act, 1951 | 1951 | 196 |
|  | `RTI` | Right to Information Act, 2005 | 2005 | 31 |
|  | `SCST` | Scheduled Castes and Scheduled Tribes (Prevention of Atrocities) Act, 1989 | 1989 | 26 |
| **Commercial, Corporate & Financial Law** | `ACA` | Arbitration and Conciliation Act, 1996 | 1996 | 92 |
|  | `CA` | Companies Act, 2013 | 2013 | 517 |
|  | `CHIT` | Chit Funds Act, 1982 | 1982 | 90 |
|  | `COMMERCIAL_COURTS` | Commercial Courts Act, 2015 | 2015 | 26 |
|  | `COMPETITION` | Competition Act, 2002 | 2002 | 95 |
|  | `CPA` | Consumer Protection Act, 2019 | 2019 | 107 |
|  | `IBC` | Insolvency and Bankruptcy Code, 2016 | 2016 | 281 |
|  | `IPA` | Indian Partnership Act, 1932 | 1932 | 74 |
|  | `LLP` | Limited Liability Partnership Act, 2008 | 2008 | 88 |
|  | `MSMED` | Micro, Small and Medium Enterprises Development Act, 2006 | 2006 | 32 |
|  | `RERA` | Real Estate (Regulation and Development) Act, 2016 | 2016 | 92 |
|  | `SCRA` | Securities Contracts (Regulation) Act, 1956 | 1956 | 78 |
|  | `SEBI` | Securities and Exchange Board of India Act, 1992 | 1992 | 92 |
|  | `SGA` | Sale of Goods Act, 1930 | 1930 | 67 |
| **Banking, Finance & Revenue** | `BRA` | Banking Regulation Act, 1949 | 1949 | 131 |
|  | `CGST` | Central Goods and Services Tax Act, 2017 | 2017 | 190 |
|  | `CUSTOMS` | Customs Act, 1962 | 1962 | 278 |
|  | `FCRA` | Foreign Contribution (Regulation) Act, 2010 | 2010 | 56 |
|  | `FEMA` | Foreign Exchange Management Act, 1999 | 1999 | 52 |
|  | `IGST` | Integrated Goods and Services Tax Act, 2017 | 2017 | 28 |
|  | `INSURANCE` | Insurance Act, 1938 | 1938 | 263 |
|  | `IRDAI` | Insurance Regulatory and Development Authority Act, 1999 | 1999 | 39 |
|  | `ITA` | Income-tax Act, 2025 | 2025 | 536 |
|  | `NIA` | Negotiable Instruments Act, 1881 | 1881 | 156 |
|  | `PBPTA` | Prohibition of Benami Property Transactions Act, 1988 | 1988 | 75 |
|  | `PSSA` | Payment and Settlement Systems Act, 2007 | 2007 | 42 |
|  | `RBI` | Reserve Bank of India Act, 1934 | 1934 | 132 |
|  | `RDBA` | Recovery of Debts and Bankruptcy Act, 1993 | 1993 | 45 |
|  | `SARFAESI` | SARFAESI Act, 2002 | 2002 | 61 |
|  | `STAMP` | Indian Stamp Act, 1899 | 1899 | 97 |
| **Civil Procedure, Contracts & Property** | `CPC` | Code of Civil Procedure, 1908 | 1908 | 171 |
|  | `EASEMENTS` | Indian Easements Act, 1882 | 1882 | 64 |
|  | `ICA` | Indian Contract Act, 1872 | 1872 | 268 |
|  | `LA` | Limitation Act, 1963 | 1963 | 32 |
|  | `MVA` | Motor Vehicles Act, 1988 | 1988 | 256 |
|  | `REGISTRATION` | Registration Act, 1908 | 1908 | 96 |
|  | `RFCTLARR` | Right to Fair Compensation & Transparency in Land Acquisition (RFCTLARR) Act, 2013 | 2013 | 114 |
|  | `SRA` | Specific Relief Act, 1963 | 1963 | 48 |
|  | `TPA` | Transfer of Property Act, 1882 | 1882 | 148 |
| **Unified Labor Codes** | `CALPRA` | Child and Adolescent Labour (Prohibition and Regulation) Act, 1986 | 1986 | 29 |
|  | `COW` | Code on Wages, 2019 | 2019 | 69 |
|  | `CSS` | Code on Social Security, 2020 | 2020 | 164 |
|  | `IRC` | Industrial Relations Code, 2020 | 2020 | 100 |
|  | `OSH` | Occupational Safety, Health and Working Conditions Code, 2020 | 2020 | 143 |
| **Cyber, Technology, Telecom & Identity** | `AADHAAR` | Aadhaar (Targeted Delivery of Financial and Other Subsidies) Act, 2016 | 2016 | 69 |
|  | `DPDPA` | Digital Personal Data Protection Act, 2023 | 2023 | 41 |
|  | `IT_ACT` | Information Technology Act, 2000 | 2000 | 125 |
|  | `TELECOM` | Telecommunications Act, 2023 | 2023 | 62 |
| **Intellectual Property Rights (IPR)** | `COPYRIGHT` | Copyright Act, 1957 | 1957 | 105 |
|  | `DESIGNS` | Designs Act, 2000 | 2000 | 48 |
|  | `GI` | Geographical Indications of Goods (Registration and Protection) Act, 1999 | 1999 | 89 |
|  | `PATENTS` | Patents Act, 1970 | 1970 | 175 |
|  | `TRADEMARKS` | Trade Marks Act, 1999 | 1999 | 169 |
| **Family & Personal Laws** | `FCA` | Family Courts Act, 1984 | 1984 | 23 |
|  | `GWA` | Guardians and Wards Act, 1890 | 1890 | 55 |
|  | `HAMA` | Hindu Adoptions and Maintenance Act, 1956 | 1956 | 30 |
|  | `HMA` | Hindu Marriage Act, 1955 | 1955 | 37 |
|  | `HSA` | Hindu Succession Act, 1956 | 1956 | 31 |
|  | `ISA` | Indian Succession Act, 1925 | 1925 | 392 |
|  | `MWPRDA` | Muslim Women (Protection of Rights on Divorce) Act, 1986 | 1986 | 7 |
|  | `MWPRMA` | Muslim Women (Protection of Rights on Marriage) Act, 2019 | 2019 | 8 |
|  | `PCMA` | Prohibition of Child Marriage Act, 2006 | 2006 | 21 |
|  | `SMA` | Special Marriage Act, 1954 | 1954 | 57 |
| **Environmental & Green Law** | `AIR` | Air (Prevention and Control of Pollution) Act, 1981 | 1981 | 62 |
|  | `EPA` | Environment (Protection) Act, 1986 | 1986 | 37 |
|  | `NGT` | National Green Tribunal Act, 2010 | 2010 | 39 |
|  | `VSA` | Van (Sanrakshan Evam Samvardhan) Adhiniyam, 1980 | 1980 | 10 |
|  | `WATER` | Water (Prevention and Control of Pollution) Act, 1974 | 1974 | 75 |
|  | `WPA` | Wild Life (Protection) Act, 1972 | 1972 | 162 |
| **Public Health, Healthcare & Food Safety** | `DCA` | Drugs and Cosmetics Act, 1940 | 1940 | 88 |
|  | `FSSA` | Food Safety and Standards Act, 2006 | 2006 | 101 |
|  | `MHA` | Mental Healthcare Act, 2017 | 2017 | 126 |
| **Social Protection, Education & Human Welfare** | `DV` | Protection of Women from Domestic Violence Act, 2005 | 2005 | 37 |
|  | `JJ` | Juvenile Justice (Care and Protection of Children) Act, 2015 | 2015 | 112 |
|  | `MWPSC` | Maintenance and Welfare of Parents and Senior Citizens Act, 2007 | 2007 | 32 |
|  | `POSH` | Sexual Harassment of Women at Workplace (Prevention, Prohibition and Redressal) Act, 2013 | 2013 | 30 |
|  | `RPWDA` | Rights of Persons with Disabilities Act, 2016 | 2016 | 102 |
|  | `RTE` | Right of Children to Free and Compulsory Education Act, 2009 | 2009 | 39 |
| **Energy, Infrastructure & Public Utilities** | `EA` | Electricity Act, 2003 | 2003 | 188 |

---

## 🏛️ Domain Breakdown Summary

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

## ⚖️ Legal Disclaimer

> **Important Notice:** This dataset is provided strictly for academic research, legal NLP, RAG benchmarks, and informational purposes. While verified against official government gazettes and India Code repositories, it does **not** constitute formal legal advice. For active litigation, commercial contracts, or compliance filings, always consult licensed advocates and cross-verify with the official Gazette of India (indiacode.nic.in).

## 👤 Curator & Citation

Curated with precision by **GSMS-B**.

```bibtex
@dataset{indian_legal_knowledge_base_2026,
  author       = {GSMS-B},
  title        = {Indian Legal Knowledge Base: Complete Structured JSON Corpus of 102 Indian Acts and Codes},
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