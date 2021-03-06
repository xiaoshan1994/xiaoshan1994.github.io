---
title: "Beggar Thy Neighbor? On the Competitiveness and Welfare Impacts of the EU’s Proposed Carbon Border Adjustment Mechanism"
date: 2021-09-07T11:36:29+02:00
description:
images:
- https://www.europarl.europa.eu/resources/library/images/20201012PHT89108/20201012PHT89108-ml.png
thumbnailImagePosition: left
thumbnailImage: //www.europarl.europa.eu/resources/library/images/20201012PHT89108/20201012PHT89108-ml.png
tags:
Categories:
- Research
- Environmentally Extended Input–Output Analysis
math: True
---

Pages Posted: 24 Jul 2021 Last revised: 30 Aug 2021
Jiarui Zhong
Martin-Luther-University Halle-Wittenberg
Jiansuo Pei
Renmin University of China - School of Applied Economics
https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3891356

## Abstract

Curbing climate change is gaining increasing consensus globally. While many countries seek to set carbon prices, significant **price dispersion** and **policy stringency** continue to raise concerns about competitiveness. To address this issue, the EU has proposed a **carbon border adjustment mechanism (CBAM)**, which aims to level the playing field by levying a carbon price on EU imports. Theoretically, this mechanism would reduce the competitiveness of developing countries' exports and, therefore, shift the environmental burden from developed regions to the emerging world. In this paper, we estimate the competitiveness and welfare impacts of the EU CBAM, based on the so-called multi-regional input-output approach. We quantify changes in the value of exports to the EU market upon CBAM implementation for both EU members and non-EU countries, plus the rest of the world. It is found that the EU CBAM will lead to a redistribution of competitiveness among countries and regions, while the effect is seen to be more pronounced in emissions-intensive and trade-intensive sectors. Moreover, a deeper sub-national-level analysis on China shows that, given its pervasive domestic production network, income losses in landlocked provinces exceed their export losses, contrasting with the pattern for trade-exposed provinces.

## Introduction

To counteract carbon leakage and the potential loss in competitiveness and to incentivize other countries to participate in combating climate change, the European Commission suggested the EU CBAM, which will levy carbon tariff on imports.

In theory, a CBAM is regarded as being effective in reducing carbon leakage and the negative impact on competitiveness induced by unilateral climate policies.

Such an outcome would violate the United Nations Framework Convention on Climate Change’s (UNFCCC) principle of **Common but Differentiated Responsibilities (CBDR)**.

## Data and model
### 2.1 Data
International Supply Use Tables (SUTs) from the World Input-Output Database (**WIOD**);
Chinese multi-regional input-output（CMRIO）tables;
China’s customs data;
Parameters from the GTAP database.
### Constructing the product-by-product CMRIO-WIOT of 2012
Using **a set of SUTs** to construct a product-by-product WIOT from WIOD.
Using **standard RAS method** to balance the blocks with the **non-negative entries**.
Using **cross-entropy (CE) matrix** balancing method constructed in Lemelin (2009) instead of the Generalized RAS (GRAS) algorithm, which Chen et al. (2019) applied (CE performs better when zero and negative entries exist due to the least information loss).

>References of RAS
[Macro-Integration - RAS (pdf file)](https://ec.europa.eu/eurostat/cros/system/files/Macro-Integration-03-M-RAS%20v1.0.pdf)
[Disaggregating Input-Output Tables by the Multidimensional RAS Method](https://arxiv.org/pdf/1704.07814.pdf)
The derived product-by-product WIOT contains 43 countries and a block for the rest of the world, each of which has 56 product sectors.

Embedding product-by-product CMRIO into the above-generated WIOT. The CMRIO contains **30 provinces** (excluding Tibet due to lack of data) of Mainland China and **30 product sectors**.

We map the **56 WIOT sectors** and **30 CMRIO sectors** into **23 product sectors**, using **N-to-1 matching** (see the matching from the original sector classification to the new sector classification given in Appendix 1).

To produce the initial values for the trade blocks **between the Chinese regions and other countries**, we use Chinese regional trade data for 2012 obtained from the **General Administration of Customs of China**.

The newly constructed CMRIO-WIOT contains **43 countries** (the rest of the world is treated as one region) and **30 Chinese provinces**. Each country/province has **23 product sectors**.

For the carbon emissions data, World Input-Output Database Environmental Accounts in Corsatea et al. (2019), converting from industry-by-industry WIOT using the same procedure as in Chen et al. (2019).

Finally, we borrow the **commodity-level substitution elasticities** between domestic and imported commodities and among imports from different sources from the **GTAP Database** (Aguiar et al., 2019).

The GTAP provides substitution elasticities for **59 GTAP commodities**, which we aggregate to obtain elasticities for the 23 sectors consistent with the sector classification in the CMRIO-WIOT.

The aggregation follows **Horridge (2018)**, which is argued to produce **a smaller aggregation bias** than the prevailing treatment of the **weighted average** of the substitution elasticities.

### 2.2 Accounting for carbon content

Without loss of generality, we assume that the **CBAM uses actual emissions data to determine the country-sector-specific benchmarks for non-EU products**. Specifically, we calculate the **emissions intensity for each commodity sector of each country**. (Alternatively, one may opt for a domestic (EU) benchmark, such as the EU average emissions intensity or best-available technology. But it will reduce enthusiasm for foreign producers)

Next, we assume that **the EU CBAM covers all goods sectors** as well as the **energy and transportation sectors**. Although the EU’s 2020 proposal indicates only starting with one or two relevant sectors in the initial phase, the CBAM will likely expand to other sectors in the following stages.

Also, to comply with WTO rules, the EU CBAM must not charge imports more than the domestic carbon price. Therefore, we assume throughout this paper that **the EU CBAM covers Scope 1 and 2 emissions only**.

Sectoral direct emissions coefficient: $\color{blue} f^{s,D}_i = F^S_i / X^S_i$, where 𝑠 ∈ 𝑆 is the country index, 𝑖 ∈ 𝑁 is the industry index, and 𝐷 stands for direct emissions. $F^S_i$ and $X^S_i$ are the total direct emissions and the total output of sector 𝑖 in country 𝑠.

Next, Scope 2 emissions account for emissions embedded in the amount of electricity, steam, and heating/cooling consumed for production. We calculate this as the direct emissions that are associated with the amounts of electricity, gas, steam, air conditioning supply, and water collection, treatment and supply consumed (Sector D35_E36).

Therefore, the indirect Scope 2 emissions of one unit of the final output for sector i in country s are:$f^{s ,D}_ = F^S_i/X^S_i$, where $f^{sl}=f^{s,D}*a_{i,4}^{s,d}$, where $f^{s,d34}$, \\(f^{s,d}_d\\),
represents the direct emissions from one unit of total output of the energy sector in the exporting country, $a_{a,D}$ is the direct consumption coefficient of sector 𝑖

$$
f^{s,l} = f^{s,D} * \sum_r a_i^s
$$

Inline math: \\(\varphi = \dfrac{1+\sqrt5}{2}= 1.6180339887…\\)

Block math:
$$
\varphi = 1+\frac{1} {1+\frac{1} {1+\frac{1} {1+\cdots} } }
$$
$a_{bc}$ or $a_{b_c}$ or ${a_b}_c$
