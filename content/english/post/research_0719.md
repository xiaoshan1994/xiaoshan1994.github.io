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
### 1.1. Developments in Multi-Regional Input-Output Analysis (MRIO) Harmonization

Compared to other databases, EXIOBASE has a clear environmental and resource focus with high levels of detail in primary production.

Harmonizing and detailing supply and use tables (SUT):

* **Gathering SUT from the relevant statistical offices**. In the specific case of EXIOBASE, data is gathered from the EU27 via Eurostat, and other SUT and IO tables from 16 other countries. Together, these cover 90% of the global gross domestic product (GDP). (See supporting
information for further details.)
* **Harmonizing SUT to allow for consistency in pricing layers** (treatment of margins and taxes), and for the consistent treatment of purchases by residents whilst abroad.
* **Detailing SUT to give a consistent classification** or, at a minimum, a link between classified imports and exports of different countries. This is either done through basic assumptions or, in the case of EXIOBASE, by using **auxiliary data** from **FAO and European AgroSAM for agriculture**, the **International Energy Agency (IEA) database for energy carriers[^ca] and electricity**, various resource databases for resources, etc.

Harmonizing and estimating environmental and social extensions:

The objective of EXIOBASE is to integrate a larger amount of data from **environmental accounts**, covering both **resource inputs** (energy, materials, water and land), as well as **outputs of waste and emissions** to air and water.

* Collecting and allocating available labour, material, land and water extraction data (e.g., the statistical databases of the Food and Agriculture Organization of the United Nations (**FAOSTAT**, **Aquastat**) and of the International Labour Organization (**LABORSTA**)) to product groups and industry sectors.

* Estimating energy and emissions data in EXIOBASE, this involved transforming the energy data of the IEA database for 63 energy carriers from **territory to residence principle** and allocating the energy supply and use to sectors and final use categories. ***Emissions are estimated consistently for all countries on the basis of energy and other activity data and TNO’s bottom-up TEAM model [25]***.

Creation of MRIO tables and footprint analysis：
In addition to the MRSUT, EXIOBASE also contains symmetric MRIO tables under various assumptions (in order for footprints or consumption-based accounts to be calculated, assumptions must be made on **converting multiple output industries into single output activities**, and further on **linear demand-supply relationships**[26]).

### 1.2. EXIOBASE Advances

The second version of EXIOBASE (EXIOBASE2—for the base year 2007) follows on from the first development of EXIOBASE (v1—for the year 2000 within the EXIOPOL project) [15], see Table 1. EXIOBASE2 sought to make advances compared to existing MRIO databases in a number of areas. Due to **aggregation errors** inherent to IO modeling [27], **a focus was placed on increasing the product and industry detail of the model**. To harmonize with the material balances of waste accounts derived elsewhere in the CREEA project, additional detail was put into both the product and industry classifications, resulting in 200 products and 163 industries (see supporting information) for enabling the **tracing of waste and recycling flows**. In addition to the sector detail, EXIOBASE2 estimated five additional **“rest of world” regions** for countries not explicitly covered in EXIOBASE v1. These changes make EXIOBASE2 the most detailed MRIO currently available. Adopted alongside the increased detail was rectangular instead of square SUT. This detail has been suggested to be essential for resource accounting [20]. This adoption provides the ability to represent a single technology that produces multiple co-products, such as an oil refinery.

![image](https://user-images.githubusercontent.com/65668613/126135268-e9224927-dbdd-4670-9e1c-51e1a638a166.png)

The final main advancement of EXIOBASE2 was the expansion of monetary SUT to link to an additional physical SUT layer. The result is to express in the physical layer all product flows in mass (dry weight) or energy units, hence allowing for physical allocation. This implies that from a product perspective, the mass balance as well as the economic balance principle of “supply equals use” will hold, while also maintaining balances from an industry perspective (i.e., the supply of products by industry and outputs to nature are equal to the use of products and inputs from nature). ***The full physical layer was exploratory***, and a comprehensive description of the approach to physical layering, and the outcomes of the layering, is beyond the scope of this paper (see [34]). Estimates of the physical layer and pricing estimates are available upon request, but results presented in this work are not based on them.

#### General Framework of Methods

Within industrial ecology and sustainability assessment in general, various methods stand out for **the accounting of the social metabolism** [35]. The three most prominent of these are (economy-wide) **material and energy flow accounting, life cycle assessment, and IO analysis**. All three methods attempt to model the complexity of production and consumption systems in order to trace source impacts to a functional demand. All methods share a similar methodological background [36], and significant scope is available for the integration of both data and methods [37].

EXIOBASE2 seeks to integrate economy-wide material and energy flow accounting with MRIO modeling (see [38–40]). This integration allows for the calculation of the various material flow metrics by recording used and unused extraction in each domestic economy, physical imports and exports, and enabling the tracing of raw material equivalents of imports and exports through Leontief modeling.

Life cycle assessment approaches are integrated through the use of life cycle inventory data to link the **direct physical and monetary inputs** required for the production of one unit of output in each industry sector, and by including characterization of environmental flows. At the basic level, the coefficients of the individual country IO tables were first estimated in both physical and monetary terms, linked by price estimates of the product groups and industry sectors. Hence, in this work, by using a consistent mathematical structure, all types of analysis from product life-cycle assessments to environmental footprints and economy-wide flow accounting can be performed.

## Data Sources

A number of disparate databases were integrated in EXIOBASE 2, thereby establishing consistency
between the thematic areas covered by the databases whilst also facilitating inter-disciplinary modeling.

### 2.1. National Account (SUT) Data

The statistical **national accounts in the form of SUT** for the 43 countries and in the form of national account aggregates for the “rest of world” regions are used as the main building blocks. SUT form the basis of GDP calculations [41], ensuring consistency through the integrated database to national account aggregates. However, some adjustments are necessary. The first stage in using the SUT requires assembling the inventory and validation of original aggregate SUT data. Inventorying implies gathering:

* For EU27: ESA95 tables discerning 59 sectors and products
* For the 16 non-EU countries: SUT and/or IO table in different kinds of classifications

SUT data are not always consistent across countries and therefore need adjustment for the MRIO
context. Tables occasionally report **negative supply or negative sales** when all values should be gross,
and published tables are **not always balanced**. Hence, as a first stage of the data harmonization,
concordances of classification are prepared and cursory data validation performed. **Through a programmed interface**, the data consistency is checked and errors in original tables are corrected.
Harmonization across different accounting conventions is done in this step. Key aspects include **the treatment of financial intermediation services indirectly measured (FISIM)[^FISIM], the handling of purchases by residents abroad and of purchases on domestic territory by non-residents, the conversion or estimation of data to enable the estimation of basic price tables (price harmonization), the preliminary balancing of tables, and the re-basing of tables to a common base year**. This automated approach creates datasets for
multiple years and facilitates future data updates.

### 2.2. Trade

The main trade data used in EXIOBASE2 originates from the UN Comtrade database [42] and the
UN services trade database [43]. The UN Comtrade data, although of reasonably high quality, is not
symmetrical; bilateral exports are not consistent with the mirror country’s bilateral imports. The BACI
database [44] is based on UN Comtrade, but is reconciled such that for a single year, every trade
flow is recorded as a single bilateral trade flow in both physical units and in free-on-board (f.o.b.)
monetary valuation.











[^fo]: https://www.mdpi.com/2071-1050/7/1/138/htm
[^ca]: Energy carriers include electricity and heat as well as solid, liquid and gaseous fuels. They occupy intermediate steps in the energy-supply chain between primary sources and end-use applications. An energy carrier is thus a transmitter of energy.
[^FISIM]: In the System of National Accounts it is an estimate of the value of the services provided by financial intermediaries, such as banks, for which no explicit charges are made; instead these services are paid for as part of the margin between rates applied to savers and borrowers. The supposition is that savers would receive a lower interest rate and borrowers pay a higher interest rate if all financial services had explicit charges.
