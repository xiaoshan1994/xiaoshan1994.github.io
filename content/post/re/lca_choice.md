---
title: "Stochastic Technology Choice Model for Consequential Life Cycle Assessment"
date: 2021-12-23T11:36:41+01:00
categories:
- Research
- Life Cycle Assessment (Re)
tags:
- CML
- Sangwon Suh
keywords:
- tech
coverImage: https://pubs.acs.org/na101/home/literatum/publisher/achs/journals/content/esthag/2016/esthag.2016.50.issue-23/acs.est.6b04270/20161201/images/large/es-2016-042708_0006.jpeg
coverSize: partial
coverMeta: out
metaAlignment: left
thumbnailImage: https://publons.com/media/thumbs/journal/logos/588671b7-6994-4446-9df3-432dbd9cb13c.png.200x200_q95_detail_letterbox_upscale.png
thumbnailImagePosition: left
metaAlignment: left
Math: True
---
[***Environmental Science & Technology***](https://pubs.acs.org/doi/10.1021/acs.est.6b04270)
Arne Kätelhön, André Bardow, and Sangwon Suh*
Publication date: **November 2, 2016**
<!--more-->
Chair of Technical Thermodynamics, RWTH Aachen University, Schinkelstrasse 8, 52062 Aachen, Germany
*Bren School of Environmental Science and Management, University of California, Santa Barbara, California 93106-5131, United States
{{< toc >}}

# Abstract

Consequential Life Cycle Assessment (CLCA) largely relied on partial or general equilibrium models which can integrate market effects but have poor resolutions of the sectoral definition and the assumption of perfect oversight by all economic agents. A new Technology Choice Model (TCM) has been introduced to incorporate parameter uncertainties and suboptimal decisions due to market imperfections and information asymmetry in a stochastic setting. A case focused on rice production.

# Introduction

* CLCA could determine the environmental consequences of decisions such as {{< hl-text blue>}}the introduction of a new technology{{< /hl-text >}}, {{< hl-text blue>}}implementing a new policy{{< /hl-text >}}, or {{< hl-text blue>}}an increase in product demand{{< /hl-text >}}. Debate arises regarding its {{< hl-text blue>}}operational models{{< /hl-text >}} for technology choices and uncertainty implications.
* CLCA heavily relies on partial equilibrium (PE) and computational general equilibrium (CGE) models for modelling market effects.
* The advantages of both PE and CGE models lies in their ability to determine the quantity and price of products jointly based on econometrically derived underlying data. Also, covering multiple regions.
* The disadvantages are underlying theoretical assumptions will not be observed in real markets, e.g. economic agents may make suboptimal decisions due to imperfect information, which will not lead to a global optimum assumed by those models. Besides, Since all markets are equilibrium, prices and demands are determined by fixed elasticities based on outdated values or proxy data. Also, it is not suitable for modelling changes introduced at a detailed process-level, or determining substitution effects among alternative technologies serving the same market.
* CLCA is often exposed to large uncertainties. Main source arises from modelling changes from the composition of technology mixes. One test way is to set multiple scenarios showing the range of potential outcomes under different assumptions. But it leads to an extremely wide range and is often based on subjective choice of selective scenarios.
* Also Analytical Error Propagation and Monte Carlo simulation have been used in LCA uncertainty assessments but not typically applied to them since they make independent choices from the mathematical formulation.

# Basic Structure of the Technology Choice Model (TCM)

## Generalized calculus for LCA

* Matrix A shows the exchange of intermediate flows (functional flows), where the coefficient $a_{ij}$ indicates the production (>0) or consumption (<0) amount. For an invertible technology matrix A and a given functional unit vector f, a scaling vector s can be calculated from:
$$S = A^{-1}f(1)$$
* Based on ISO standards (14040 and 14044), elementary flows are defined as {{< hl-text orange>}}material or energy entering or leaving the studied system from or into the environment without previous or subsequent human transformation.{{< /hl-text >}}
* Matrix B shows the elementary flows of the unit processes, where the coefficient $b_{ej}$ shows the elementary flow e of unit process j entering (<0) or leaving (>0) the system.
* Multiplying the elementary flow matrix B with the scaling vector s yields the Life Cycle Inventory (LCI) vector g representing the total elementary flows associated with the functional unit f:
$$g = Bs = BA^{-1}f$$
* The characterization matrix Q contains characterization factors transforming the elementary flows into environmental impact flows. The characterization factor of elementary flow e for impact category z is represented by the coefficient qze of the characterization matrix Q. The total environmental impacts expressed in impact vector h are calculated such that:
$$h = Qg = QBA^{-1}f$$

## Case Study
* The functional unit is defined as "production of 1 kg processed rice"
*
## Supporting Information

https://pubs.acs.org/doi/suppl/10.1021/acs.est.6b04270/suppl_file/es6b04270_si_001.pdf
