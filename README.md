# 时间序列分类基础模型：论文与代码汇总

本仓库汇总 TIC-FM、ChorusTIC 及时间序列分类基础模型综述与基准的公开研究材料，供算力申请单位查阅研究基础与代码实现。

**整理日期：2026 年 10 月 21 日。** 论文保留原始 PDF；代码保存为指定提交版本的源码快照，同时提供原始下载压缩包。公开榜单仅提供链接。

## 材料目录

| 研究工作 | 论文正文 | 代码 | 原始论文页面 |
| --- | --- | --- | --- |
| TIC-FM | [PDF（v2）](papers/TIC-FM-v2.pdf) | [浏览源码](code/TIC-FM/) · [下载 ZIP](code/TIC-FM.zip) | [arXiv:2602.00620](https://arxiv.org/abs/2602.00620) |
| ChorusTIC | [PDF（v2）](papers/ChorusTIC-v2.pdf) | [浏览源码](code/ChorusTIC/) · [下载 ZIP](code/ChorusTIC.zip) | [arXiv:2608.24033](https://arxiv.org/abs/2608.24033) |
| 综述与基准 | [PDF（v1）](papers/TSC-FM-Survey-and-Benchmark-v1.pdf) | 基准入口见下方公开榜单 | [Preprints.org](https://www.preprints.org/manuscript/202609.2097) |

**公开榜单：[TSC-FM Leaderboard](https://tsc-fm.dmirlab.com/leaderboard)**。排名及结果以在线榜单为准。

## 研究工作

### 1. TIC-FM

**Rethinking Zero-Shot Time Series Classification: From Task-specific Classifiers to In-Context Inference**

该工作研究通过上下文推断完成时间序列分类，将带标签样本作为上下文，在目标任务推断时无需更新模型参数。详细方法、实验设置与结果见论文。

- 原始代码仓库：[DMIRLAB-Group/TIC-FM](https://github.com/DMIRLAB-Group/TIC-FM)
- 归档提交：[`da015302d73c68ab0fc988166ae57e4d814b7681`](https://github.com/DMIRLAB-Group/TIC-FM/commit/da015302d73c68ab0fc988166ae57e4d814b7681)
- 环境及运行方法：[原项目 README](code/TIC-FM/README.md)
- DOI：[10.48550/arXiv.2602.00620](https://doi.org/10.48550/arXiv.2602.00620)

### 2. ChorusTIC

**ChorusTIC: Training-Free Multivariate Time Series Classification via Chorus In-Context Learning**

该工作研究面向单变量与多变量时间序列的上下文分类，通过时间及跨通道建模支持不同通道配置，在目标任务推断时无需拟合专用分类器。详细方法、实验设置与结果见论文。

- 原始代码仓库：[DMIRLAB-Group/ChorusTIC](https://github.com/DMIRLAB-Group/ChorusTIC)
- 归档提交：[`efef93698bd3afa9cfa0b6c7a1aea94190f2549a`](https://github.com/DMIRLAB-Group/ChorusTIC/commit/efef93698bd3afa9cfa0b6c7a1aea94190f2549a)
- 环境及运行方法：[原项目 README](code/ChorusTIC/README.md)
- DOI：[10.48550/arXiv.2608.24033](https://doi.org/10.48550/arXiv.2608.24033)

### 3. 综述与基准

**Surveying and Benchmarking Foundation Models for Time Series Classification**

该工作从表征迁移、微调与适配、上下文学习三个角度梳理时间序列分类基础模型，并提供覆盖 198 个时间序列分类数据集的统一评测基础设施。论文当前为预印本，具体评测协议与实验结果见正文。

- 论文页面：[Preprints.org / 202609.2097](https://www.preprints.org/manuscript/202609.2097)
- DOI：[10.20944/preprints202609.2097.v1](https://doi.org/10.20944/preprints202609.2097.v1)
- 在线评测榜单：[TSC-FM Leaderboard](https://tsc-fm.dmirlab.com/leaderboard)

## 文件与版本核验

- `papers/`：三篇原始论文 PDF。
- `code/`：两份源码快照和对应原始 ZIP，未修改上游源文件。
- [metadata/manifest.json](metadata/manifest.json)：下载地址、源码提交、文件大小、PDF 页数及 SHA-256 校验值。
- [metadata/SHA256SUMS.txt](metadata/SHA256SUMS.txt)：论文和代码压缩包的校验清单。

本仓库是材料汇总，不是新的模型实现。源码运行说明以各项目 README 为准；模型权重与实验数据不包含在源码快照中。材料整理时未执行模型训练或复现实验。本仓库不预设算力申请的 GPU 型号、卡数或使用时长。


