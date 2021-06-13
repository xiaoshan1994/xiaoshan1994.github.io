---
title: Linking Global Crop and Livestock Consumption to Local Production Hotspots
date: 2021-06-06T09:42:03+02:00
description: Identifying production hotspots for global crop and livestock consumption by a Spatially Explicit Multi-Reginal Input-Output model
images:
- https://i.ytimg.com/vi/Bye-XjYGOzM/maxresdefault.jpg
thumbnail: https://i.ytimg.com/vi/Bye-XjYGOzM/maxresdefault.jpg
tags:
- MRIO
- agriculture and food
Categories:
- Research
---

Identifying production hotspots for global crop and livestock consumption by a Spatially Explicit Multi-Reginal Input-Output model ( *[Zhongxiao's work](https://www.sciencedirect.com/science/article/pii/S2211912419300276)* on *Global Food Security*).

Keywords: primary crops; animal husbandry; spatially explicit; Multi-Regional Input-Output(MRIO) analysis.

## Research background

1. Food security is challenged by increasing global food demand driven by population growth and animal-based diets.
2. More crop production requires increasing areas of land and fresh water, causing associated environmental impacts[^1].
3. Also livestock should be a focus as their feed contains harmful ingredients[^2] which will released to our environment finally.
4. To preserve nature, high-income nations transfer this **environmental burden** to agriculture producing countries through **international trade**.
5. Two classical examples of shifting environmental burdens through international trade are the export of Brazilian soy and Indonesian palm oil, acting as case studies in this paper.
6. As no comprehensive assessment of crops and livestock embodied in trade **at a high spatial resolution** since, this work has been done, expecting to guide sustainable practices and healthier diets [^3] as well as facilitate global cooperation between production- and consumption-oriented countries [^4].
7. This work also facilitates a more accurate assessment of agricultural environment impacts in EXIOBASE.

## Materials and Methods

Using MRIO model with EXIOBASE, which is linked to crop and livestock data derived from FAOSTAT.

The database includes **8 crop sectors** linking **163 types of crop** derived from **FAOSTAT** (domestic extraction of primary crops, cereals are based on the weight of dry grain, vegetable and fruits are based on the weight of fresh fruit of human consumption, treenuts are based on the weight of nut for sale) with input-output accounts (Table S 8.10). This forms the
foundation for analysing the distribution of crops driven by consumption.
8 crop sectors in EXIOBASE:
| Number | Name	| CodeNr	| CodeTxt |
| --- | --- | --- | --- |
| 1	| Paddy rice	| p01.a	| C_PARI|
| 2	| Wheat	| p01.b	| C_WHEA|
| 3	| Cereal grains nec	| p01.c	| C_OCER|
| 4	| Vegetables, fruit, nuts	| p01.d	| C_FVEG|
| 5	| Oil seeds	| p01.e	|C_OILS|
| 6	| Sugar cane, sugar beet	| p01.f	| C_SUGB|
| 7	| Plant-based fibers	| p01.g	| C_FIBR|
| 8	| Crops nec	| p01.h	| C_OTCR|

163 types of domestic extraction used for primary crops:
e.g.:
Domestic Extraction Used - Primary Crops - Abaca	kt
...

We select related data from FAOSTAT to create **6 livestock satellite accounts** to match with EXIOBASE, including cattle, pig, chicken, duck, goat, and sheep (Table S 8.11).

|EXIOBASE sector number| EXIOBASE name| FAOSTAT product names|
| --- | --- | --- |
|11 |Poultry |Eggs, hen, in shell|
|14 |Raw milk |Milk, whole fresh cow; Milk, whole fresh goat; Milk, whole fresh sheep|
|43 |Products of meat cattle |Hides, cattle, fresh; Meat indigenous, cattle|
|44 |Products of meat pigs| Meat indigenous, pig|
|45 |Products of meat poultry| Meat indigenous, chicken; Meat indigenous, duck|
|46 |Meat products nec |Meat indigenous, goat; Skins, goat, fresh; Meat indigenous, sheep; Skins, sheep, fresh|

**Aquaculture** is not considered in this research due to a lack of spatially explicit data.



[^1]: e.g. Eutrophication, soil acidification, ecotoxicity, greenhouse gas emissions, and biodiversity loss.
[^2]: Livestock feed potentially contains additives, antibiotics and antimicrobials, leading eutrophication, soil contamination and the spread of drug-resistant pathogens.
[^3]: By identifying **spatial heterogeneity of different consumption patterns** and setting **a safe target** for primary crops and livestock consumption.
[^4]: With consumption-based accounting of primary crops and livestock.
