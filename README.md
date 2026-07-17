# Quant Research Report Notes

这个仓库用于整理我在量化研究学习过程中阅读的研报笔记与复现代码。每个子文件夹对应一篇研报，包含该研报的学习笔记，以及后续用于策略复现、因子检验或回测实验的代码预留位置。

我希望这个仓库不只是简单摘录研报内容，而是把研报中的核心建模思想、因子逻辑、策略结构和潜在 Alpha 进行二次消化，形成可以长期复用的研究笔记与代码框架。

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
└── README.md
```


## Current Notes

| No. | Topic | Report | Main Idea | Recommendation |
| --- | --- | --- | --- | --- |
| [01](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_01_ts_cta_methodology/notes.md) | Time-Series CTA | 华泰研究《时序 CTA 方法论综述：市场状态、开仓信号与退出机制》 | 市场状态识别、趋势开仓信号、止损与退出机制、CTA Alpha 来源 | Medium |
| [02](https://github.com/runqi-allen-wang/Quant-Research-Report-Notes/blob/main/report_02_chip_structure_end2end_ai_factor/notes.md) | AI Factor | 华泰研究《基于筹码分层结构的端到端AI因子》 | 利用筹码成本结构与CNN+GRU挖掘非线性选股 Alpha | High |
|[自进化 Skill：选股策略的自动迭代](https://inst.htsc.com/research/report?reportId=4501046409)| Agent | 华泰研究《自进化Skill：选股策略的自动迭代》 | 利用Agent 自动迭代选股 | Low |

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

## Planned Code Components

后续每篇研报对应的代码部分可能包括：

```text
src/
├── data_loader.py        # 数据读取与预处理
├── factors.py            # 因子或指标计算
├── signals.py            # 开仓、平仓、调仓信号
├── backtest.py           # 简单回测框架
├── evaluation.py         # 绩效评估与稳健性检验
└── config.py             # 参数配置
```

代码部分会尽量保持简洁，优先服务于理解研报逻辑，而不是追求复杂工程化。

## Disclaimer

本仓库仅用于个人学习、研究记录和方法复现，不构成任何投资建议。研报中的观点、数据和结论属于原作者，本仓库中的笔记为个人理解与再整理。任何策略回测结果都可能受到样本区间、参数选择、交易成本、数据质量和市场环境变化的影响，不能代表未来收益。
