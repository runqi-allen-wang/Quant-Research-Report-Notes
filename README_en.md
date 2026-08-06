# Quant Research Report Notes
[中文版 README](README_CN.md) \| English


> A project for reading, analyzing, and systematically accumulating knowledge from quantitative research reports, powered by [AlphaLens](https://github.com/runqi-allen-wang/AlphaLens).
![AlphaLens Poster](AlphaLens.png)

This repository organizes my study notes on financial engineering, quantitative investing, asset allocation, fund research, and AI-driven investment research reports. At present, it primarily focuses on public reports published by the [**HTSC Financial Engineering Research Team**](https://inst.htsc.com/research).

Each subfolder corresponds to one research report and usually contains:

- `notes.md`: structured study notes generated with AlphaLens and manually reviewed;
- `src/`: a reserved directory for subsequent strategy replication, factor testing, backtesting experiments, or data processing.

Rather than merely excerpting report content, this repository conducts secondary analysis around research questions, methodological mechanisms, validity boundaries, and sources of Alpha. Its purpose is to transform scattered research reports into a reusable, traceable, and extensible body of quantitative research knowledge.

---

## How AlphaLens Is Used in This Project

The report notes and README entries in this repository are generated according to the AlphaLens analytical framework.

AlphaLens is a lightweight, Skill-based framework for analyzing quantitative research reports. Its core objective is to formalize the reading methodology of an experienced quantitative researcher into a reusable workflow:

```text
Research report input
    ↓
Research type identification
    ↓
Analysis template selection
    ↓
Core contribution localization
    ↓
Alpha mechanism extraction
    ↓
Boundary and failure analysis
    ↓
Reusable knowledge accumulation
```

[AlphaLens](https://github.com/runqi-allen-wang/AlphaLens) does more than answer “What is this report about?” It also focuses on:

- What problem the research attempts to solve;
- Why the proposed method works;
- Where its value or Alpha comes from;
- Which assumptions the conclusions depend on;
- Under what conditions the method may fail;
- How the method can be replicated, extended, or transferred.

---

## Repository Structure

```text
├── report_01_ts_cta_methodology/
│   ├── notes.md
│   └── src/
│
├── report_02_chip_structure_end2end_ai_factor/
│   ├── notes.md
│   └── src/
│
├── ...
│
├── README.md
└── SKILL.md
```

Where:

- `report_xx_*`: an independent research directory for a single report;
- `notes.md`: structured study notes;
- `src/`: strategy replication, data processing, factor testing, and backtesting experiments;
- `SKILL.md`: the current report-analysis specification used by this repository.

---

## Current Notes

Recommendation uses three independent dimensions: 🚀 Industry Leadership; 🧩 Framework Completeness; 🔁 Strong Reproducibility.

| No. | Topic | Report | Main Idea | Time | Recommendation |
| --- | --- | --- | --- | --- | --- |
| [01](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_01_ts_cta_methodology/notes.md) | Time-Series CTA | HTSC Research, “[A Review of Time-Series CTA Methodologies: Market Regimes, Entry Signals, and Exit Mechanisms](https://inst.htsc.com/research/report?reportId=4507121011)” | Decomposes CTA return sources through market-regime identification, trend signals, and exit mechanisms to construct a systematic trend-following research framework | 2026-06-10 | 🧩 |
| [02](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_02_chip_structure_end2end_ai_factor/notes.md) | AI Factor | HTSC Research, “[An End-to-End AI Factor Based on Layered Chip-Distribution Structures](https://inst.htsc.com/research/report?reportId=4504481798)” | Uses chip-cost distributions to characterize investor behavior and applies CNN+GRU models to learn nonlinear stock-selection Alpha | 2026-06-02 | 🚀🧩 |
| [03](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_03_self_evolving_skill/notes.md) | AI Research Agent | HTSC Research, “[Self-Evolving Skills: Automated Iteration of Stock-Selection Strategies](https://inst.htsc.com/research/report?reportId=4501046409)” | Builds an automated quantitative research workflow through Agents, Skill management, and version iteration, improving strategy exploration and knowledge reuse | 2026-05-25 | 🚀🧩 |
| [04](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_04_multidimensional_timing_model/notes.md) | Market Timing | HTSC Research, “[Deconstructing and Rebuilding a Multidimensional Market-Timing Model](https://inst.htsc.com/research/report?reportId=4498558551)” | Decomposes market-timing signals into momentum chasing, bottom fishing, short chasing, and top escaping, then combines them by scenario to improve market-regime adaptability | 2026-05-18 | 🧩 |
| [05](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_05_china_assets_long_term_beta/notes.md) | China Asset Beta | HTSC Research, “[Capturing the Medium- to Long-Term Beta Opportunities in Chinese Assets: A 2026 Mid-Year Quantitative Outlook](https://inst.htsc.com/research/report?reportId=4500709151)” | Interprets the market through global stagnation rather than inflation, RMB appreciation potential, and crowded Alpha, then converts Chinese-asset Beta into manageable portfolio returns through multi-asset allocation and ETF-FOF construction | 2026-05-25 | 🧩 |
| [06](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_06_multi_objective_fundamental_factor_mining/notes.md) | Fundamental Factor Mining | HTSC Research, “[Trading Space for Time: A Multi-Objective Framework for Mining Fundamental Stock-Selection Factors](https://inst.htsc.com/research/report?reportId=4359005908)” | Uses parameterized financial-indicator expressions and NSGA-II to jointly optimize IIC, time-series win rate, and long-side ranking performance, thereby mining stable fundamental Alpha while preserving economic interpretability | 2025-08-11 | 🚀🧩🔁 |
| [07](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_07_intraday_explainable_factor_mining/notes.md) | Intraday Factor Mining | HTSC Research, “[Parameterized High-Frequency Features: A Minute-Level Explainable Factor-Mining Framework](https://inst.htsc.com/research/report?reportId=4470731640)” | Extracts interpretable microstructure signals through parameterized minute-level price-volume formulas and NSGA-III multi-objective search, providing independent incremental Alpha for daily-frequency AI stock-selection models | 2026-03-31 | 🚀🧩🔁 |
| [08](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_08_active_equity_market_review/notes.md) | Active Equity | HTSC Research, “[An In-Depth Review and Outlook of the Active Equity Market](https://inst.htsc.com/research/report?reportId=4466845800)” | Explains the revaluation of active-management capabilities through regulatory benchmarks, fund flows, product differentiation, and institutional platforms, extracting sustainable excess-return, risk-control, and organizational Alpha | 2026-03-27 | 🧩 |
| [09](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_09_quantitative_industry_rotation_rough_road/notes.md) | Industry Rotation | HTSC Research, “[The Rugged Road of Quantitative Industry Rotation](https://inst.htsc.com/research/report?reportId=4459844484)” | Rebuilds industry rankings using reversal-adjusted residual momentum, crowding alerts, and multi-objective genetic programming, while improving allocation weights and exit-risk management through style timing and CTA methods | 2026-03-13 | 🚀🧩 |
| [10](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_10_global_three_layer_liquidity_risk/notes.md) | Liquidity Risk | HTSC Research, “[A Three-Layer Global Liquidity Risk Early-Warning Model](https://inst.htsc.com/research/report?reportId=4460172299)” | Constructs a global liquidity warning system along the transmission chain of central-bank supply, leveraged financing, and market trading, then reduces multi-asset portfolio tail drawdowns through dynamic cash defense | 2026-03-15 | 🚀🧩 |
| [11](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_11_llm_concept_macro_stock_selection/notes.md) | Multi-Agent Selection | HTSC Research, “[LLM-Based Concept and Macro-Theme Stock Selection](https://inst.htsc.com/research/report?reportId=4454061267)” | Organizes parallel Agents through industrial-chain decomposition and multi-path macro scenario analysis, then converts unstructured thematic information into auditable stock portfolios through evidence arbitration | 2026-02-28 | 🚀🧩 |
| [12](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_12_korea_etf_market_overview_and_hot_products/notes.md) | Korea ETF Market | HTSC Research, “[Overview of the Korean ETF Market and Popular Products](https://inst.htsc.com/research/report?reportId=4455704456)” | Characterizes the Korean ETF ecosystem through underlying assets, active management, duopolistic competition, and shifts in popular products, revealing market expansion jointly driven by the semiconductor industry, cash-management demand, and product innovation | 2026-03-06 | 🧩 |
| [13](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_13_hong_kong_fundamental_quant_guide/notes.md) | HK Fundamental Quant | HTSC Research, “[A Guide to Fundamental Quantitative Investing in Hong Kong Equities](https://inst.htsc.com/research/report?reportId=4449343380)” | Standardizes heterogeneous Hong Kong financial statements across accounting standards, reporting times, and currencies; screens high-quality companies using a six-dimensional fundamental score; and enhances stock ranking with conventional price-volume and GRU factors | 2026-07-31 | 🧩🔁 |

---

## Focus of the Notes

Each report note is generally organized around the following dimensions.

### 1. Research Question and Core Framework

Restate the problem addressed by the report and clarify the logical relationships among data, models, signals, portfolios, and systems.

### 2. Methodological and Model Analysis

Evaluate whether the model assumptions, inputs and outputs, parameter settings, signal construction, regime identification, portfolio rules, and validation design are reasonable.

### 3. Data and Empirical Evidence

Key concerns include:

- Data sources and Point-in-Time consistency;
- Sample splitting;
- Look-ahead bias;
- Benchmark selection;
- Transaction costs;
- Style and industry exposures;
- Out-of-sample stability;
- Backtest periods and coverage of market regimes.

### 4. Alpha Mechanism Extraction

Alpha is not limited to conventional stock-selection returns. It also includes:

| Alpha Type | Focus |
| --- | --- |
| Prediction Alpha | Whether return or regime-prediction capability is improved |
| Risk Management Alpha | Whether volatility, drawdowns, or tail risk are reduced |
| Research Process Alpha | Whether research efficiency and experimental iteration speed are improved |
| Information Processing Alpha | Whether complex information can be processed and transformed more effectively |
| Data Quality Alpha | Whether incremental value is obtained from higher-quality data |
| Infrastructure Alpha | Whether the reproducibility and extensibility of the research system are improved |
| Decision Consistency Alpha | Whether subjective judgment and process instability are reduced |
| Organizational Alpha | Whether team knowledge accumulation and collaboration are improved |

### 5. Validity Boundaries and Failure Risks

The notes record not only model performance but also analyze:

- What conditions are required for the conclusions to hold;
- Whether the results depend on a specific market regime;
- Whether the method is sensitive to parameter choices;
- Whether the signal may decay;
- Whether turnover, capacity, and market-impact costs impose constraints;
- Which results may be difficult to transfer into live trading.

### 6. Replication and Transfer Directions

Assess whether the method can be:

- Replicated in other assets or markets;
- Transferred to different frequencies;
- Integrated into existing research workflows;
- Converted into subsequent factor tests, strategy backtests, or system-development tasks.

---

## Research Philosophy

When reading a research report, I primarily focus on the following questions:

1. What is the report's final deliverable: a factor, signal, position, risk state, fund evaluation, or Agent workflow?
2. What value does the method actually create: return prediction, risk control, research efficiency, information processing, or organizational capability?
3. Does the core variable provide independent incremental information, or does it merely re-express momentum, volatility, liquidity, or size exposure?
4. Do the empirical results depend on a specific sample, parameter setting, investment universe, market environment, or transaction-cost assumption?
5. Can the method be transferred to other assets, frequencies, or markets?
6. In live trading, would the primary risks come from signal decay, turnover, capacity, tail drawdowns, data quality, or execution costs?
7. What is most worth preserving over the long term: the report's specific conclusions, or its underlying research paradigm and methodology?

---

## Project Objectives

This repository aims to gradually build a searchable and reusable quantitative research knowledge base, so that each report becomes more than a one-time reading record and can instead be accumulated as:

- A reusable research framework;
- A testable factor hypothesis;
- An implementable strategy module;
- A traceable risk mechanism;
- An extensible Agent or research-infrastructure design;
- A starting point for subsequent code replication and empirical research.

---

## Disclaimer

This repository is intended solely for personal study, research documentation, and methodological replication. It does not constitute investment advice.

The views, data, and conclusions in the original reports belong to their respective authors. The contents of this repository reflect personal interpretation, structured organization, and secondary analysis. Any strategy, factor, or backtesting result may be affected by the sample period, parameter choices, transaction costs, data quality, market rules, and changes in market conditions, and therefore cannot represent or guarantee future returns.
