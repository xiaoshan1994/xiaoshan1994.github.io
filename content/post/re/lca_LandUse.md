---
title: Land use indicators in LCA
date: 2021-08-10T09:54:21+02:00
description:
images:
- https://1businessworld.com/wp-content/uploads/2020/06/17/Screen-Shot-2020-06-17-at-4.55.08-PM.png
thumbnailImagePosition: left
thumbnailImage: //1businessworld.com/wp-content/uploads/2020/06/17/Screen-Shot-2020-06-17-at-4.55.08-PM.png
tags:
Categories:
- Research
- Life Cycle Assessment (Re)
---

## Principles for life cycle inventories of land use on a global scale

Thomas Koellner, Laura de Baan, Tabea Beck, Miguel Brandão, Barbara Civit, Mark Goedkoop, Manuele Margni, Llorenç Milà i Canals, Ruedi Müller-Wenk, Bo Weidema & Bastian Wittstock
The International Journal of Life Cycle Assessment volume 18, pages1203–1215 (2013)
https://link.springer.com/article/10.1007/s11367-012-0392-0

### Land use elementary flows

In LCA, land occupation and land transformation can be distinguished as basic types of land use elementary flows (Milà i Canals et al. 2007). They result in either damage to or benefits for ecosystem quality. Whereas **land transformation causes a change in ecosystem quality, land occupation delays recovery**. For example, the conversion of tropical forest into cropland causes a drop in biodiversity and damages the original ecosystem. The continuous use of such cropland hinders the regrowth of tropical forest. In order to assess the impact of such land uses, it is necessary to at least register in the LCI the type of land use, the spatial extent, the temporal extent, and the geographical location (Milà i Canals et al. 2007). In LCIs, the elementary flows of land use are therefore specified as follows:

* For land occupation: square meter × years, land use type i, and region k

* For land transformation: square meter, initial land use type i → final land use type j, and region k

Human activities do not only alter the terrestrial but also the aquatic surface. Some processes imply the occupation or transformation of water surface (e.g., building a street on top of a river) or the bottom of water bodies (e.g., fish trawling). Mila i Canals et al. (2007) define **“physical changes in the seabed”** as **land use-related impacts** and distinguish between occupation and transformation impacts. ***The use of aquatic surface can cause environmental impacts and should be listed in LCIs as this is done in Ecoinvent (Frischknecht and Jungbluth 2007).*** In the following, we therefore also discuss the classification of surface use on top of or under water bodies. For simplicity, ***we use the term “land use” to express the use of terrestrial as well as aquatic surface***.

### Existing land use and cover classifications in LCA

The Life Cycle Inventory database ecoinvent 2.0 holds extensive data on land use of industrial processes (Frischknecht and Jungbluth 2007). It uses a land classification, which is based on the **CORINE (Plus) Classification**, but has **a much lower number of land use classes**. The disadvantage is that it omits classes, which are near to nature and beneficial from a biodiversity or ecosystem services point of view. For many LCA applications this is not a problem, but for assessing “green” land uses (e.g., occupation of primary forest) to compensate intense land uses (e.g., crop production) the current Ecoinvent classification is not sufficient. Also, the assessment of ecosystem services as input into the production system is not possible without taking near-to nature land uses into account. Ecoinvent database version 3 has based its land classification on the typology presented in this paper (Weidema et al. 2011).

The classification of land use within the LCIA method ReCiPe defines 18 categories. A comparison of land use types as defined in Ecoinvent and ReCiPe can be found in the final report (de Schryver and Goedkoop 2008). For agricultural land use types (crops/weeds, fertile and infertile grassland, tall grassland/herb) a distinction between monoculture, intensive, and extensive land is made. Forests are distinguished by tree types (coniferous, broad-leafed, mixed) and intensity of use (monoculture, plantation, extensive). The advantage of this method is the inclusion of main land use and boundaries (which are of special importance for biodiversity). However, this classification does not necessarily encompass all relevant global land cover types.

## Overview and methodology: Data quality guideline for the ecoinvent database version 3

https://www.ecoinvent.org/files/dataqualityguideline_ecoinvent_3_20130506.pd

Weidema B P, Bauer C, Hischier R, Mutel C, Nemecek T, Reinhard J, Vadenbo C O, Wernet G
ecoinvent report No. 1(v3)
St. Gallen, 2013-05-06

### 6.7 Land occupation and land transformation

Land occupation and land transformation receives increasing attention in life cycle inventory analyses and life cycle impact assessment methods.

Table 6.1. **Land use classes** used in the ecoinvent database. Table continues on next page.

![image](https://user-images.githubusercontent.com/65668613/128849182-1f6372a7-9280-47d8-800f-aa6c2b58b83a.png)

Land use is inventoried through the use of data on:
* Land occupation for the current land use (the occupied land is prevented from changing to a more natural state).
* Land transformation (from previous land use and to current land use, e.g., the conversion of a former natural area to industrial land; the conversion of a gravel quarry to a natural area by active re-cultivation).

land occupation is recorded in area*time (m2*year).

A land transformation consists of two entries:
1. Land transformation, from land use class X, and
2. Land transformation, to land use class Y.
Example: "Transformation, from forest", in m2 and "transformation, to mineral extraction site", also in m2. Land transformation thus records a state before and after a transformation.
