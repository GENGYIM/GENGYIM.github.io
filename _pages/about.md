---
permalink: /
title: "Hello"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
# About me
Welcome to my personal GitHub Pages site!

## Personal Profile
I am Geng Yiming, a first-year Ph.D. student in [Peking University School of Stomatology](https://ss.bjmu.edu.cn/), [Peking University](https://www.pku.edu.cn/). I am fortunate to be supervised by Prof. [Zhou Yongsheng](https://ss.bjmu.edu.cn/Html/Doctors/Main/Index_353.html). 

## Research Interests
The construction of various nanodrug delivery systems and their applications in oral diseases, as well as the studies on the related mechanisms of autophagy and ferroptosis.

## Contact me
- GitHub：[GENGYIM](https://gengyim.github.io/)
- E-mail：gengym813@163.com

## Publication
1. Yiming Geng*, Shengyun Huang*, Li Ma* et al. [Propranolol-induced autophagic dysfunction combined with a targeted metal-organic framework as a novel strategy for improving antitumor therapeutic efficacy](https://www.sciencedirect.com/science/article/pii/S2352940723001567), Applied Materials Today.  
2. Yiming Geng*, Huwei Zou*, Haiwei Wu et al. [Recent advances in nanomaterial-driven strategies for diagnosis and therapy of vascular anomalies](https://link.springer.com/article/10.1186/s12951-024-02370-2), Review , Journal of Nanobiotechnology. 
3. Yiming Geng, Miao Yu, Haiwei Wu et al. [3D-printed personalized digital guide plate for greater palatine block in trigeminal neuralgia](https://www.sciencedirect.com/science/article/pii/S0266435624000160), British Journal of Oral & Maxillofacial Surgery.
4. Yiming Geng*, Cancan Meng*, Hanzhi Zhang* et al. [A novel therapeutic approach to hemangiomas: Combining photothermal therapy and ferroptosis in a microneedle delivery system](https://www.sciencedirect.com/science/article/pii/S2590006425003072)，Materials Today Bio.

## Portfolio
### 数据读取
[单细胞数据 GSE232240](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE232240) 
[转录组数据TCGA-HNSCC](https://portal.gdc.cancer.gov/)

### 数据预处理
1.UMAP细胞聚类分析

![UMAP 细胞聚类结果图](/images/屏幕截图 2026-01-17 100352.png){: style="width: 80%; max-width: 300px;"}

通过 UMAP 降维可视化展示细胞聚类结果，清晰呈现不同细胞亚群的分布特征

2.免疫细胞亚群分选

![免疫细胞亚群分选结果图](/images/02.png){: style="width: 80%; max-width: 300px;"}

基于细胞表面标志物完成免疫细胞亚群的分选与富集

3.NR组和RE组免疫细胞差异

![非响应组（NR）组和响应组（RE）组免疫细胞差异](/images/03.png){: style="width: 80%; max-width: 300px;"}

各样本中各类免疫细胞的相对比例构成

4.不同免疫细胞在 RE/NR 状态下的分布差异

![免疫细胞亚群分选结果图](/images/04.png){: style="width: 80%; max-width: 300px;"}

NR和RE应组B细胞比例存在差异

### 统计分析
综上述数据分析处理，发现响应组和非响应组B细胞比例发生变化，进一步统计不同组的B细胞之间差异基因表达。

1.两组样本间的基因差异表达

![两组样本间的基因差异表达结果图](/images/05.png){: style="width: 80%; max-width: 300px;"}

NR（无应答）与 RE（应答） 两组样本间的基因差异表达情况

2.GO 功能富集分析

![GO 功能富集分析](/images/006.png){: style="width: 80%; max-width: 300px;"}

差异基因主要集中在以抗体生成和 B 细胞免疫为核心的适应性免疫通路，提示 “NR/RE” 状态的差异可能与 B 细胞介导的体液免疫功能密切相关

3.KEGG 通路富集分析

![KEGG 通路富集分析](/images/13.png){: style="width: 80%; max-width: 300px;"}

差异基因主要富集在以细胞因子 - 细胞因子受体互作为核心的免疫调控通路，同时涉及造血、抗原呈递、炎症信号传导等过程

### 预测模型建立
使用Lasso回归模型

1. LASSO 回归的偏似然偏差诊断图

![ LASSO 回归的偏似然偏差诊断图结果图](/images/07.png){: style="width: 80%; max-width: 300px;"}

2. LASSO 回归的系数轨迹图

![LASSO 回归的系数轨迹图结果图](/images/08.png){: style="width: 80%; max-width: 300px;"}

### 构建风险模型，预测模型评估

选择逐步回归cox模型

RiskScore=-0.34549*BLK+-0.07645*2F2+-1.08219*L26+0.08742*SPESP1

1. 时间依赖的受试者工作特征曲线

![ 时间依赖的受试者工作特征曲线结果图](/images/09.png){: style="width: 80%; max-width: 300px;"}

评估模型在不同时间点（1 年、2 年、4 年）对事件发生的预测能力

2. Kaplan-Meier 生存曲线

![LASSO 回归的系数轨迹图结果图](/images/10.png){: style="width: 80%; max-width: 300px;"}

Kaplan-Meier 生存曲线，用于比较 TCGA-HNSCC（头颈部鳞状细胞癌）队列中，高风险评分（High RiskScore）与低风险评分（Low RiskScore）两组患者的生存预后差异

### 多免疫队列验证
选择逐步回归cox模型

RiskScore=-0.34549*BLK+-0.07645*2F2+-1.08219*L26+0.08742*SPESP1

1. 时间依赖的受试者工作特征曲线

![ 时间依赖的受试者工作特征曲线结果图](/images/09.png){: style="width: 80%; max-width: 300px;"}

评估模型在不同时间点（1 年、2 年、4 年）对事件发生的预测能力

2. Kaplan-Meier 生存曲线

![LASSO 回归的系数轨迹图结果图](/images/10.png){: style="width: 80%; max-width: 300px;"}

Kaplan-Meier 生存曲线，用于比较 TCGA-HNSCC（头颈部鳞状细胞癌）队列中，高风险评分（High RiskScore）与低风险评分（Low RiskScore）两组患者的生存预后差异
