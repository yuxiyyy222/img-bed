---
typora-copy-images-to: upload
---

# DRACO 跨领域深度研究基准数据集

### * 在线使用数据集教程：[【OpenBayes 官方教程】公共资源介绍](https://www.bilibili.com/video/BV13G411R7ya/)

## 数据集简介

DRACO 跨领域深度研究基准数据集是由 Perplexity 团队发布的一个面向复杂研究任务评估场景的数据集，相关论文成果为 [DRACO: A Cross-Domain Benchmark for Deep Research Accuracy, Completeness, and Objectivity](https://hyper.ai/papers/2602.11685)，旨在系统评估深度研究系统在准确性、完整性和客观性方面的综合能力。

该数据集包含 100 个复杂研究任务，覆盖全球五大洲的 40 个国家与地区，涉及金融、购物/产品对比、学术、科技等 10 大应用领域。每个任务对应一个多步骤、多来源的信息检索与分析问题，并配有由 26 位领域专家设计和验证的评估标准。每个标准平均包含约 40 项评价指标，从事实准确性、分析广度与深度、展示质量以及引用质量四个维度对模型输出进行细粒度评估。

各领域任务占比如下图：

![](https://cdn.jsdelivr.net/gh/yuxiyyy222/img-bed/img/x2.png)

<center><p>任务领域分布</p></center>

**数据字段**:

- `id`: 任务的唯一标识符
- `domain`: 任务所属的领域
- `problem`: 需要解答的完整研究查询
- `answer`: JSON 编码的评估标准，包含各个评估维度的具体标准
