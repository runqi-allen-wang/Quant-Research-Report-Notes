# Quant Research Report Notes

> 基于 [AlphaLens](https://github.com/runqi-allen-wang/AlphaLens) 的量化研报阅读、分析与知识沉淀项目。
![AlphaLens Poster](AlphaLens.png)


本仓库用于整理我在量化研究学习过程中阅读的金融工程、量化投资、资产配置、基金研究与 AI 投研报告。目前主要关注 [**华泰金工组**](https://inst.htsc.com/research) 的公开研报。

每个子文件夹对应一篇研报，通常包含：

- `notes.md`：由 AlphaLens 生成并经人工检查的结构化学习笔记；
- `src/`：用于后续策略复现、因子检验、回测实验或数据处理的代码预留目录。

本仓库并不追求对研报进行简单摘录，而是希望围绕研究问题、方法机制、有效边界与 Alpha 来源进行二次分析，将分散的研报内容转化为可长期复用、可追踪、可扩展的量化研究知识。

---

## AlphaLens 如何参与本项目

本仓库中的研报笔记与 README 条目均按照 AlphaLens 的分析规范生成。

AlphaLens 是一个轻量 SKILL 化的量化研报分析框架，核心目标是将资深量化研究员的阅读方法固化为可复用流程：

```text
研报输入
    ↓
研究类型识别
    ↓
分析模板选择
    ↓
核心贡献定位
    ↓
Alpha 机制提炼
    ↓
边界与失效分析
    ↓
可复用知识沉淀
```

[AlphaLens](https://github.com/runqi-allen-wang/AlphaLens) 不只回答“这篇研报讲了什么”，还重点回答：

- 研究试图解决什么问题；
- 方法为什么有效；
- 价值或 Alpha 来源是什么；
- 结论依赖哪些假设；
- 研究在哪些条件下可能失效；
- 方法如何被复现、扩展或迁移。

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

其中：

- `report_xx_*`：单篇研报的独立研究目录；
- `notes.md`：结构化学习笔记；
- `src/`：策略复现、数据处理、因子检验与回测实验目录；
- `SKILL.md`：当前仓库使用的研报分析规范。

---

## Current Notes

Recommendation 使用三个独立维度：🚀：行业领先性；🧩：框架完整性；🔁：强可复现性。

| No. | Topic | Report | Main Idea | Time | Recommendation |
| --- | --- | --- | --- | --- | --- |
| [01](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_01_ts_cta_methodology/notes.md) | Time-Series CTA | 华泰研究《[时序 CTA 方法论综述：市场状态、开仓信号与退出机制](https://inst.htsc.com/research/report?reportId=4507121011)》 | 从市场状态识别、趋势信号和退出机制三个层面拆解 CTA 收益来源，构建系统化趋势跟踪研究框架 | 2026-06-10 | 🧩 |
| [02](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_02_chip_structure_end2end_ai_factor/notes.md) | AI Factor | 华泰研究《[基于筹码分层结构的端到端AI因子](https://inst.htsc.com/research/report?reportId=4504481798)》 | 利用筹码成本分布刻画投资者行为结构，并通过 CNN+GRU 学习非线性选股 Alpha | 2026-06-02 | 🚀🧩 |
| [03](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_03_self_evolving_skill/notes.md) | AI Research Agent | 华泰研究《[自进化 Skill：选股策略的自动迭代](https://inst.htsc.com/research/report?reportId=4501046409)》 | 利用 Agent、Skill 管理和版本迭代机制构建自动化量化研究流程，提升策略探索与知识复用效率 | 2026-05-25 | 🚀🧩 |
| [04](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_04_multidimensional_timing_model/notes.md) | Market Timing | 华泰研究《[多维择时模型的拆解与重构](https://inst.htsc.com/research/report?reportId=4498558551)》 | 将择时信号拆解为追高、抄底、追空和逃顶路径，并通过场景化组合提升市场状态适应能力 | 2026-05-18 | 🧩 |
| [05](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_05_china_assets_long_term_beta/notes.md) | China Asset Beta | 华泰研究《[把握中国资产的中长期 Beta 机会——2026 量化视角中期展望](https://inst.htsc.com/research/report?reportId=4500709151)》 | 以全球“滞而非胀”、人民币升值潜力与 Alpha 拥挤为状态判断，借助多资产配置和 ETF-FOF 将中国资产 Beta 转化为可管理的组合收益 | 2026-05-25 | 🧩 |
| [06](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_06_multi_objective_fundamental_factor_mining/notes.md) | Fundamental Factor Mining | 华泰研究《[以空间换时间——多目标基本面选股因子挖掘框架](https://inst.htsc.com/research/report?reportId=4359005908)》 | 以参数化财务指标表达式和 NSGA-II 同时优化 IIC、时序胜率与多头排序表现，在保持经济解释性的同时挖掘稳定基本面 Alpha | 2025-08-11 | 🚀🧩🔁 |
| [07](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_07_intraday_explainable_factor_mining/notes.md) | Intraday Factor Mining | 华泰研究《[高频特征参数化：分钟级可解释因子挖掘框架](https://inst.htsc.com/research/report?reportId=4470731640)》 | 以参数化分钟量价公式和 NSGA-III 多目标搜索提取可解释微观结构信号，并为日频 AI 选股模型提供独立增量 Alpha | 2026-03-31 | 🚀🧩🔁 |
| [08](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_08_active_equity_market_review/notes.md) | Active Equity | 华泰研究《[主动权益市场深度复盘与发展前瞻](https://inst.htsc.com/research/report?reportId=4466845800)》 | 从监管基准、份额流向、产品分化与机构平台四个层面解释主动管理价值重估，提炼可持续超额、风险控制与组织能力 Alpha | 2026-03-27 | 🧩 |
| [09](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_09_quantitative_industry_rotation_rough_road/notes.md) | Industry Rotation | 华泰研究《[量化行业轮动的“崎岖之路”](https://inst.htsc.com/research/report?reportId=4459844484)》 | 以反转修正残差动量、拥挤度预警与多目标遗传规划重建行业排序，并用风格择时和 CTA 改善权重配置与退出风险 | 2026-03-13 | 🚀🧩 |
| [10](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_10_global_three_layer_liquidity_risk/notes.md) | Liquidity Risk | 华泰研究《[全球三层次流动性风险预警模型](https://inst.htsc.com/research/report?reportId=4460172299)》 | 沿央行供给、杠杆融资与市场交易三层传导构建全球流动性预警，并以动态现金防御降低多资产组合尾部回撤 | 2026-03-15 | 🚀🧩 |
| [11](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_11_llm_concept_macro_stock_selection/notes.md) | Multi-Agent Selection | 华泰研究《[大模型概念与宏观热点选股](https://inst.htsc.com/research/report?reportId=4454061267)》 | 以产业链拆分和宏观多路径推演组织并行智能体，并通过证据仲裁将非结构化热点信息转化为可审计选股组合 | 2026-02-28 | 🚀🧩 |
| [12](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_12_korea_etf_market_overview_and_hot_products/notes.md) | Korea ETF Market | 华泰研究《[韩国 ETF 市场概况和热点产品](https://inst.htsc.com/research/report?reportId=4455704456)》 | 从底层资产、主动管理、双寡头竞争与热点产品迁移刻画韩国 ETF 生态，揭示半导体产业、现金管理需求和产品创新共同驱动的市场扩张 | 2026-03-06 | 🧩 |
| [13](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_13_hong_kong_fundamental_quant_guide/notes.md) | HK Fundamental Quant | 华泰研究《[港股基本面量化指南](https://inst.htsc.com/research/report?reportId=4449343380)》 | 统一港股异构财报的准则、时点与币种口径，以六维基本面评分筛选优质公司，并叠加传统量价与 GRU 因子增强股票排序 | 2026-07-31 | 🧩🔁 |

---

## 笔记关注内容

每篇研报的学习笔记通常从以下维度展开。

### 1. 研究问题与核心框架

重新表述研报试图解决的问题，并梳理数据、模型、信号、组合或系统之间的逻辑关系。

### 2. 方法与模型分析

分析模型假设、输入输出、参数设置、信号构造、状态识别、组合规则与验证设计是否合理。

### 3. 数据与实证证据

关注：

- 数据来源与 Point-in-Time；
- 样本划分；
- 前视偏差；
- 基准选择；
- 交易成本；
- 风格和行业暴露；
- 样本外稳定性；
- 回测区间与市场状态覆盖。

### 4. Alpha 机制提炼

Alpha 不局限于传统选股收益，也包括：

| Alpha 类型 | 关注内容 |
| --- | --- |
| Prediction Alpha | 是否提升收益或状态预测能力 |
| Risk Management Alpha | 是否降低波动、回撤或尾部风险 |
| Research Process Alpha | 是否提升研究效率和实验迭代速度 |
| Information Processing Alpha | 是否提高复杂信息的处理与转化能力 |
| Data Quality Alpha | 是否通过更高质量的数据获得增量 |
| Infrastructure Alpha | 是否提升研究系统的复现与扩展能力 |
| Decision Consistency Alpha | 是否减少主观判断和流程波动 |
| Organizational Alpha | 是否提升团队知识沉淀与协同能力 |

### 5. 有效边界与失效风险

不仅记录方法表现，也分析：

- 结论成立需要哪些条件；
- 是否依赖特定市场阶段；
- 是否存在参数敏感性；
- 信号是否可能衰减；
- 是否受到换手、容量与冲击成本限制；
- 哪些结果难以迁移到实盘。

### 6. 复现与迁移方向

评估方法是否能够：

- 在其他资产或市场复现；
- 迁移到不同频率；
- 与现有研究流程结合；
- 转化为后续因子检验、策略回测或系统开发任务。

---

## Research Philosophy

我在阅读研报时主要关注以下问题：

1. 研究最终交付的对象是什么：因子、信号、仓位、风险状态、基金评价，还是 Agent 工作流？
2. 方法到底创造了什么价值：收益预测、风险控制、研究效率、信息处理，还是组织能力？
3. 核心变量是否具有独立增量，还是对动量、波动率、流动性或规模风格的重复表达？
4. 实证结果是否依赖特定样本、参数、标的、市场环境或交易成本假设？
5. 方法能否迁移到其他资产、频率或市场？
6. 如果进入实盘，主要风险来自信号失效、换手、容量、尾部回撤、数据质量，还是执行成本？
7. 研报中最值得长期保留的，是具体结论，还是背后的研究范式与方法论？

---

## 项目目标

本仓库希望逐步形成一套可检索、可复用的量化研究知识库，使每篇研报不只是一次性阅读记录，而能够进一步沉淀为：

- 可复用的研究框架；
- 可检验的因子假设；
- 可实现的策略模块；
- 可追踪的风险机制；
- 可扩展的 Agent 或研究基础设施设计；
- 后续代码复现与实证研究的起点。

---

## Disclaimer

本仓库仅用于个人学习、研究记录与方法复现，不构成任何投资建议。

研报中的观点、数据与结论属于原作者，本仓库中的内容为个人理解、结构化整理与二次分析。任何策略、因子或回测结果均可能受到样本区间、参数选择、交易成本、数据质量、市场制度和市场环境变化的影响，不能代表未来收益。

