# Quant Research Report Notes

这个仓库用于整理我在量化研究学习过程中阅读的研报笔记。目前我在看[**华泰金工组**](https://inst.htsc.com/research)。每个子文件夹对应一篇研报，包含该研报的学习笔记，以及后续用于策略复现、因子检验或回测实验的代码预留位置。

我希望这个仓库不只是简单摘录研报内容，而是把研报中的核心建模思想、因子逻辑、策略结构和潜在 Alpha 进行二次消化，形成可以长期复用的研究笔记。如果你对其中的内容感兴趣或者对我感兴趣，欢迎联系。

## Repository Structure

```text
.
├── 01_time_series_cta/
│   ├── notes.md
│   └── src/
│
├── 02_chip_structure_ai_factor/
│   ├── notes.md
│   └── src/
│
| ......
|
├── README.md
|
└── SKILL.md
```


## Current Notes

Recommendation 使用三个独立维度：

🚀：行业领先性；🧩：框架完整性；🔁：强可复现性。

| No. | Topic | Report | Main Idea | Time | Recommendation |
| --- | --- | --- | --- | --- | --- |
 [01](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_01_ts_cta_methodology/notes.md)               | Time-Series CTA   | 华泰研究《[时序 CTA 方法论综述：市场状态、开仓信号与退出机制](https://inst.htsc.com/research/report?reportId=4507121011)》 | 从市场状态识别、趋势信号和退出机制三个层面拆解 CTA 收益来源，构建系统化趋势跟踪研究框架    | 2026-06-10 | 🧩             |
| [02](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_02_chip_structure_end2end_ai_factor/notes.md) | AI Factor         | 华泰研究《[基于筹码分层结构的端到端AI因子](https://inst.htsc.com/research/report?reportId=4504481798)》            | 利用筹码成本分布刻画投资者行为结构，并通过 CNN+GRU 学习非线性选股 Alpha       | 2026-06-02 | 🚀🧩           |
| [03](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_03_self_evolving_skill/notes.md)              | AI Research Agent | 华泰研究《[自进化 Skill：选股策略的自动迭代](https://inst.htsc.com/research/report?reportId=4501046409)》         | 利用 Agent、Skill 管理和版本迭代机制构建自动化量化研究流程，提升策略探索与知识复用效率 | 2026-05-25 | 🚀🧩           |
| [04](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_04_multidimensional_timing_model/notes.md)    | Market Timing     | 华泰研究《[多维择时模型的拆解与重构](https://inst.htsc.com/research/report?reportId=4498558551)》                | 将择时信号拆解为追高、抄底、追空和逃顶路径，并通过场景化组合提升市场状态适应能力          | 2026-05-18 | 🧩             |
| [05](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_05_china_assets_long_term_beta/notes.md) | China Asset Beta | 华泰研究《[把握中国资产的中长期 Beta 机会——2026 量化视角中期展望](https://inst.htsc.com/research/report?reportId=4500709151)》 | 以全球“滞而非胀”、人民币升值潜力与 Alpha 拥挤为状态判断，借助多资产配置和 ETF-FOF 将中国资产 Beta 转化为可管理的组合收益 | 2026-05-25 | 🧩 |
| [06](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_06_multi_objective_fundamental_factor_mining.md) | Fundamental Factor Mining | 华泰研究《[以空间换时间——多目标基本面选股因子挖掘框架](https://inst.htsc.com/research/report?reportId=4359005908)》 | 以参数化财务指标表达式和 NSGA-II 同时优化 IIC、时序胜率与多头排序表现，在保持经济解释性的同时挖掘稳定基本面 Alpha | 2025-08-11 | 🚀🧩🔁 |
| [07](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_07_intraday_explainable_factor_mining.md) | Intraday Factor Mining | 华泰研究《[高频特征参数化：分钟级可解释因子挖掘框架](https://inst.htsc.com/research/report?reportId=4470731640)》 | 以参数化分钟量价公式和 NSGA-III 多目标搜索提取可解释微观结构信号，并为日频 AI 选股模型提供独立增量 Alpha | 2026-03-31 | 🚀🧩🔁 |
| [08](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_08_active_equity_market_review.md) | Active Equity | 华泰研究《[主动权益市场深度复盘与发展前瞻](https://inst.htsc.com/research/report?reportId=4466845800)》 | 从监管基准、份额流向、产品分化与机构平台四个层面解释主动管理价值重估，提炼可持续超额、风险控制与组织能力 Alpha | 2026-03-27 | 🧩 |

| No. | Topic | Report | Main Idea | Time | Recommendation |
| --- | --- | --- | --- | --- | --- |
| [05](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_05_multitarget_fundamental_factor_mining/notes.md) | Factor Mining I | 华泰研究《[以空间换时间——多目标基本面选股因子挖掘框架](https://inst.htsc.com/research/report?reportId=4359005908)》 | 以参数化基本面公式、IC/IC 胜率/NDCG@k 三目标和 NSGA-II 构建可解释因子搜索系统，并用显存缓存提升滚动挖掘效率 | 2025-08-11 | High |
| [06](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_06_intraday_parametric_factor_mining/notes.md) | Factor Mining II | 华泰研究《[高频特征参数化：分钟级可解释因子挖掘框架](https://inst.htsc.com/research/report?reportId=4470731640)》 | 将姊妹篇框架扩展到分钟量价数据，通过日内切片、条件掩码、时序算子、NSGA-III 和动态短板惩罚挖掘微观结构 Alpha | 2026-03-31 | High |
| [07](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_07_active_equity_market_review/notes.md) | Active Euqity Market | 华泰研究《[金工: 主动权益市场深度复盘与发展前瞻](https://inst.htsc.com/research/report?reportId=4466845800)》 | 分析新形势下，何种主动权益产品、基金经理和机构仍然具有长期竞争力 | 2026-03-27 | Low |
| [08](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_08_industry_rotation_rugged_road/notes.md) | Quant Pipeline | 华泰研究《[金工: 量化行业轮动的“崎岖之路”](https://inst.htsc.com/research/report?reportId=4459844484)》 | 通过残差动量、行业拥挤度、多目标遗传规划与风格择时，构建兼顾截面选行业和时序风险控制的动态行业轮动框架。 | 2026-03-13 | High |
| [09](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_09_global_three_layer_liquidity_warning/notes.md) | Risk Control | 华泰研究《[全球三层次流动性风险预警模型](https://inst.htsc.com/research/report?reportId=4460172299)》 | 从央行、资金和市场三层流动性构建全球风险预警信号，并以防御择时降低多资产组合在流动性危机中的同步回撤 | 2026-03-15 | Medium |
| [10](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_10_llm_concept_macro_stock_selection/notes.md) | LLM Stock Selection | 华泰研究《[大模型概念与宏观热点选股](https://inst.htsc.com/research/report?reportId=4454061267)》 | 利用多智能体大模型框架将概念与宏观事件转化为产业链映射和投资逻辑，通过非结构化信息挖掘主题选股 Alpha | 2026-02-28 | High |


## What I Record
每篇研报的学习笔记通常包括以下内容：

- **核心思路复述**：用尽量简洁的语言重新解释研报的研究问题、模型框架和策略流程。
- **模型设置分析**：关注模型假设、参数估计、信号构造、状态识别和回测设定是否合理。
- **因子选择分析**：分析所用因子或技术指标背后的经济含义、统计性质和可能的冗余问题。
- **优缺点评价**：从量化研究和实盘应用角度评价研报方法的可行性、稳定性和局限。
- **Alpha 提炼**：尝试总结真正可能贡献收益的部分，而不仅仅记录表面策略规则。

## Research Philosophy

我在阅读研报时更关注以下几个问题：

1. 这个策略到底赚的是什么钱？是趋势延续、风险补偿、行为偏差、期限结构，还是特定市场制度下的交易摩擦？
2. 模型中的变量是否真的有增量信息，还是只是对价格动量、波动率或流动性的重复表达？
3. 回测结果是否依赖强参数、样本区间、标的选择或交易成本假设？
4. 这个方法能否迁移到其他资产、其他频率或其他市场？
5. 如果要实盘化，最大的风险来自哪里：信号失效、换手过高、容量不足、尾部回撤，还是执行成本？


## Disclaimer

本仓库仅用于个人学习、研究记录和方法复现，不构成任何投资建议。研报中的观点、数据和结论属于原作者，本仓库中的笔记为个人理解与再整理。任何策略回测结果都可能受到样本区间、参数选择、交易成本、数据质量和市场环境变化的影响，不能代表未来收益。
