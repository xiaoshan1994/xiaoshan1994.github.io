---
title: "Global Sustainability Accounting—Developing EXIOBASE for Multi-Regional Footprint Analysis"
date: 2021-07-19T09:57:38+02:00
description: "A global multi-regional input−output database (EXIOBASE) with a focus on environmentally relevant activities, allowing insights into the production-related impacts and consumption footprints."
images:
- https://exiobase.eu/images/sliderafbeeldingen/slider_global_consumption.PNG
thumbnail: https://exiobase.eu/images/sliderafbeeldingen/slider_global_consumption.PNG
tags:
- MRIO
- EIOA
Categories:
- Research
---

A global multi-regional input−output database (EXIOBASE) with a focus on environmentally relevant activities, allowing insights into the production-related impacts and consumption footprints[^fo].

## Introduction
### 1.1. Developments in Multi-Regional Input-Output Analysis (MRIO) ***Harmonization***

* Compared to other databases, EXIOBASE has a clear environmental and resource focus with high levels of detail in primary production.

Harmonizing and detailing supply and use tables (SUT):
* Gathering SUT from the relevant statistical offices. In the specific case of EXIOBASE, data is
gathered from the EU27 via Eurostat, and other SUT and IO tables from 16 other countries.
Together, these cover 90% of the global gross domestic product (GDP). (See supporting
information for further details.)
* Harmonizing SUT to allow for consistency in pricing layers (treatment of margins and taxes),
and for the consistent treatment of purchases by residents whilst abroad.
* Detailing SUT to give a consistent classification or, at a minimum, a link between classified
imports and exports of different countries. This is either done through basic assumptions or, in
the case of EXIOBASE, by using auxiliary data from FAO and European AgroSAM for
agriculture, the International Energy Agency (IEA) database for energy carriers[^ca] and electricity,
various resource databases for resources, etc.

Harmonizing and estimating environmental and social extensions:
The objective of EXIOBASE is to integrate a larger amount of data from environmental accounts,
covering both resource inputs (energy, materials, water and land), as well as outputs of waste and
emissions to air and water.
* Collecting and allocating available labour, material, land and water extraction data (e.g., the
statistical databases of the Food and Agriculture Organization of the United Nations
(FAOSTAT, Aquastat) and of the International Labour Organization (LABORSTA)) to product
groups and industry sectors.
* Estimating energy and emissions data in EXIOBASE, this involved transforming the energy data of the IEA database for 63 energy carriers from **territory to residence principle** and allocating the energy supply and use to sectors and final use categories. Emissions are estimated consistently for all countries on the basis of energy and other activity data and TNO’s bottom-up TEAM model [25].

Creation of MRIO tables and footprint analysis：
In addition to the MRSUT, EXIOBASE also contains symmetric MRIO tables under various
assumptions (in order for footprints or consumption-based accounts to be calculated, assumptions must
be made on **converting multiple output industries into single output activities**, and further on **linear demand-supply relationships**[26]).

### 1.2. EXIOBASE Advances

The second version of EXIOBASE (EXIOBASE2—for the base year 2007) follows on from the first
development of EXIOBASE (v1—for the year 2000 within the EXIOPOL project) [15], see Table 1.
EXIOBASE2 sought to make advances compared to existing MRIO databases in a number of areas. Due
to **aggregation errors** inherent to IO modeling [27], **a focus was placed on increasing the product and industry detail of the model**. To harmonize with the material balances of waste accounts derived elsewhere in the CREEA project, additional detail was put into both the product and industry classifications, resulting in 200 products and 163 industries (see supporting information) for enabling the
tracing of waste and recycling flows. In addition to the sector detail, EXIOBASE2 estimated five additional “rest of world” regions for countries not explicitly covered in EXIOBASE v1. These changes
make EXIOBASE2 the most detailed MRIO currently available. Adopted alongside the increased detail
was rectangular instead of square SUT. This detail has been suggested to be essential for resource
accounting [20]. This adoption provides the ability to represent a single technology that produces
multiple co-products, such as an oil refinery.

![image](https://user-images.githubusercontent.com/65668613/126135268-e9224927-dbdd-4670-9e1c-51e1a638a166.png)


[^fo]: https://www.mdpi.com/2071-1050/7/1/138/htm
[^ca]: Energy carriers include electricity and heat as well as solid, liquid and gaseous fuels. They occupy intermediate steps in the energy-supply chain between primary sources and end-use applications. An energy carrier is thus a transmitter of energy.
