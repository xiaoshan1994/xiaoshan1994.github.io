---
title: "Modelling the global impact of China’s ban on plastic waste imports"
date: 2021-12-28T10:37:42+01:00
categories:
- Plastic
- Trade and Input-output Analysis
tags:
- China
keywords:
- tech
coverImage:
coverSize: full/partial
coverMeta: out
metaAlignment: left
thumbnailImage: https://ars.els-cdn.com/content/image/X09213449.jpg
thumbnailImagePosition: left
Math: True
---
[***Resources, Conservation and Recycling***](https://www.sciencedirect.com/science/article/pii/S0921344919305130)
Received 15 May 2019, Available online **10 December 2019**.
<!--more-->
Qiao Huang et al.
School of Statistics, Beijing Normal University, Beijing 100875, China
{{< toc >}}

# 1. Introduction
* China's plastic waste import ban was in January 2018.
* First study quantifying the impact of China's ban on waste imports by using multiregional input-output models(GMRIO).

# 2. Materials and methods

Four models: (1) Environmentally extended multiregional input-output model; (2) Structural path analysis; (3) Ecological network analysis and (4) Hypothetical extraction method.

![](https://ars.els-cdn.com/content/image/1-s2.0-S0921344919305130-gr1_lrg.jpg)

## 2.1. The extended multiregional input-output model
The standard Leontief demand-driven MRIO model is as follows:
$$x = Ly = (I - A)^{-1}y = (I - T\hat{x}^{-1})^{-1}y$$
After attaching the sectoral plastic waste imports vector, it can be transferred to an extended MRIO model:
$$ Q = qL\hat{y}$$
Where Q ($1 \times s$, million tons) represents the total amount of imported plastic waste consumed by sectors; q ($1 \times s$, tons/$)indicates direct plastic waste imports intensity.
This equation shows the direct and indirect imports of the plastic waste in China driven by global consumption.

## 2.2 Structural path analysis
* It can identify the essential paths in line with a specific sectoral final demand.
* End up with the fourth production layer accounting for 80% contribution.

## 2.3 Ecological network analysis

## 2.4 Hypothetical extraction method
Analysing the economic decrease assuming one or more sectors is removed from the economy.

## 2.5 Data sources
* Six groups of data:
(1) the global MRIO table (**Global MRIO in 2015** is derived from Eora database)
(2) plastic waste imports (UN Comtrde Database on the imports for category: "Waste, parings and scrap, of plastics (3915)" by mass(kg))
(3) population
(4) waste generation per capital (4-6 is sourced from two reports: *What a Waste: A Global Review of Solid Waste Management* (Hoornweg and Bhada-Tata, 2012) and *What a Waste 2.0: A Global Snapshot of Solid Waste Management to 2050* (Silpa et al., 2018))
(5) waste composition
(6) the waste collection rate of each economy.

## 2.6 Reconciliations of the multiregional input-output tables
About the aggregation of regions and sectors.

## 2.7. Adding waste trade data into the multiregional input-output tables
The author try to explain a flaw in this paper -- the truth is not all the plastic waste imports will be transferred into new products and meet sectoral demand.
{{< alert info >}} It is confusing that waste import acts as an environmental satellite account instead of export. Thinking of this: which one is resulted from the demand? {{< /alert >}}
