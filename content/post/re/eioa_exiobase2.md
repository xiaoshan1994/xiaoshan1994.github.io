---
title: "Global Sustainability Accounting—Developing EXIOBASE for Multi-Regional Footprint Analysis"
date: 2021-07-19T09:57:38+02:00
description: "A global multi-regional input−output database (EXIOBASE) with a focus on environmentally relevant activities, allowing insights into the production-related impacts and consumption footprints."
images:
- https://exiobase.eu/images/sliderafbeeldingen/slider_global_consumption.PNG
thumbnailImagePosition: left
thumbnailImage: //exiobase.eu/images/sliderafbeeldingen/slider_global_consumption.PNG
tags:
Categories:
- Research
- Environmentally Extended Input–Output Analysis
---

A global multi-regional input−output database (EXIOBASE) with a focus on environmentally relevant activities, allowing insights into the production-related impacts and consumption footprints[^fo].

## 1. Introduction
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

EXIOBASE2 seeks to integrate economy-wide material and energy flow accounting with MRIO modelling (see [38–40]). This integration allows for the calculation of the various material flow metrics by recording used and unused extraction in each domestic economy, physical imports and exports, and enabling the tracing of raw material equivalents of imports and exports through Leontief modelling.

Life cycle assessment approaches are integrated through the use of life cycle inventory data to link the **direct physical and monetary inputs** required for the production of one unit of output in each industry sector, and by including characterization of environmental flows. At the basic level, the coefficients of the individual country IO tables were first estimated in both physical and monetary terms, linked by price estimates of the product groups and industry sectors. Hence, in this work, by using a consistent mathematical structure, all types of analysis from product life-cycle assessments to environmental footprints and economy-wide flow accounting can be performed.

## 2. Data Sources

A number of disparate databases were integrated in EXIOBASE 2, thereby establishing consistency between the thematic areas covered by the databases whilst also facilitating inter-disciplinary modelling.

### 2.1. National Account (SUT) Data

The statistical **national accounts in the form of SUT** for the 43 countries and in the form of national account aggregates for the “rest of world” regions are used as the main building blocks. SUT form the basis of GDP calculations [41], ensuring consistency through the integrated database to national account aggregates. However, some adjustments are necessary. The first stage in using the SUT requires assembling the inventory and validation of original aggregate SUT data. Inventorying implies gathering:

* For EU27: **ESA95 tables** discerning 59 sectors and products
* For the 16 non-EU countries: SUT and/or IO table in different kinds of classifications

SUT data are not always consistent across countries and therefore need adjustment for the MRIO context. Tables occasionally report **negative supply or negative sales** when all values should be gross, and published tables are **not always balanced**. Hence, as a first stage of the data harmonization, concordances of classification are prepared and cursory data validation performed. **Through a programmed interface**, the data consistency is checked and errors in original tables are corrected. Harmonization across different accounting conventions is done in this step. Key aspects include **the treatment of financial intermediation services indirectly measured (FISIM)[^FISIM], the handling of purchases by residents abroad and of purchases on domestic territory by non-residents, the conversion or estimation of data to enable the estimation of basic price tables (price harmonization), the preliminary balancing of tables, and the re-basing of tables to a common base year**. This automated approach creates datasets for multiple years and facilitates future data updates.

### 2.2. Trade

The main trade data used in EXIOBASE 2 originates from the **UN Comtrade database** [42] and the
**UN services trade database** [43]. The UN Comtrade data, although of reasonably high quality, is not
symmetrical; bilateral exports are not consistent with the mirror country’s bilateral imports. The BACI
database [44] is based on UN Comtrade, but is reconciled such that for a single year, every trade
flow is recorded as a single bilateral trade flow in both physical units and in free-on-board (f.o.b.)
monetary valuation.

### 2.3. Agriculture Social Accounting Matrices for European Countries (AgroSAM)

A set of social accounting matrices (SAM) for the EU27 was developed as part of the AgroSAM project at the Institute for Prospective Technological Studies [45]. These tables follow the standard Eurostat format for SUT in purchaser prices, but are extended to include feedbacks of primary inputs into final demand, although this feature is not used in this project. In addition, the project provided disaggregated agricultural data for 30 primary agricultural sectors and 11 food processing sectors. Such detail allowed the direct mapping of the AgroSAM database to the EXIOBASE2 classification for all sectors with the exception of fish product processing, which was aggregated with “food products nec”. As the AgroSAM data are only from 2000, the relative values (structure) of inputs and sales were taken for the agricultural and food sectors, and applied as coefficients for the disaggregation of the 2007 tables.

### 2.4. FAOSTAT and Other Sector Outputs

The Food and Agriculture Organization of the United Nations (FAO) database, FAOSTAT [46], provided in 2007 dollars, was used to estimate agricultural sector production values. These output data were coupled with the AgroSAM-derived coefficients for EU countries and the coefficient data for non-EU countries. Some adjustments were made to FAOSTAT data where there was a discrepancy between physical and monetary reported values.

Data for manufacturing product output for European countries are obtained from the PRODCOM database [47], and industry turnover from the Structural Business Statistics [48].

### 2.5. International Energy Agency Energy Balances

The International Energy Agency (IEA) **Energy Balances database** was used as the source of disaggregation for the energy flows [49,50]. ***The IEA database is converted from the territory to the residence principle***[^trprin] based on the accounting rules provided by the United Nations Department of Economic and Social Affairs [51] and Eurostat [52] by applying auxiliary datasets [53]. The most important of these transformations occurs in the transport sector, where a transformation is needed from the place where fuels are sold (basis for the territory principle) to the use by residents of a country. A secondary step tailors energy supply and use and emission factors to the EXIOBASE2 industry and product classifications, i.e., translates IEA flow and product to existing EXIOBASE2 categories. Several auxiliary datasets were used to perform this transformation [53]. In addition, for use of the energy accounts in detailing monetary SUT, derived prices were applied.  Combustion-related air emission accounts are calculated directly on the basis of the energy accounts described above, providing implicit internal consistency between the energy and emission accounts [53]. To do so, the energy flows related to combustion are identified and combined with emission factors following the so-called energy-first approach described in Eurostat [54]. These emission factors for greenhouse gases and air pollutants are available from the guidance for estimating emissions of greenhouse gases and air pollutants at the national level. The Intergovernmental Panel on Climate Change (IPCC) Guidelines for National Greenhouse Gas Inventories [55] and the European Monitoring and Evaluation Programme/European Environment Agency (EMEP/EEA) Guidebook [56] for air pollutants provide the methodologies for emission estimation. This set of methodologies also forms the basis on which countries estimate their annual emissions under the United Nations Framework Convention on Climate Change (UNFCCC) and Convention on Long-Range Transboundary Air Pollution (CLRTAP) international conventions.
For each country and sector, a suitable methodology has been selected based on the importance of the source (a more important emission source requires a more detailed method) but also on data availability. The methods are applied to each sector and each country at the global level, resulting in a global emissions dataset. This dataset is compared to the official emissions to identify outliers and possible errors, which are corrected where needed. A one-to-one comparison is not possible because of the territory principle applied in the official country inventories.
For the non-combustion air emission accounts, emissions are calculated in a similar way by combining various activity statistics (e.g., industrial production, use of products) with the methodologies from the guidelines described above. The activity statistics have been collected from various data sources, including the material use database described earlier. Emission factors are taken from the guidance documents and applied to selected activity data for each sector. Similar to the combustion emissions, the non-combustion emissions are also compared to official UNFCCC and CLRTAP emissions to identify possible outliers and errors, but a detailed comparison was not possible due to the different basis (territory vs. residency principle).

### 2.6. Emission Accounts

Combustion-related air emission accounts are calculated directly on the basis of the energy accounts described above, providing implicit internal consistency between the energy and emission accounts [53]. To do so, the energy flows related to combustion are identified and combined with emission factors following the so-called energy-first approach described in Eurostat [54]. These emission factors for greenhouse gases and air pollutants are available from the guidance for estimating emissions of greenhouse gases and air pollutants at the national level. The Intergovernmental Panel on Climate Change (IPCC) Guidelines for National Greenhouse Gas Inventories [55] and the European Monitoring and Evaluation Programme/European Environment Agency (EMEP/EEA) Guidebook [56] for air pollutants provide the methodologies for emission estimation. This set of methodologies also forms the basis on which countries estimate their annual emissions under the United Nations Framework Convention on Climate Change (UNFCCC) and Convention on Long-Range Transboundary Air Pollution (CLRTAP) international conventions.

For each country and sector, a suitable methodology has been selected based on the importance of the source (a more important emission source requires a more detailed method) but also on data availability. The methods are applied to each sector and each country at the global level, resulting in a global emissions dataset. This dataset is compared to the official emissions to identify outliers and possible errors, which are corrected where needed. A one-to-one comparison is not possible because of the territory principle applied in the official country inventories.

For the non-combustion air emission accounts, emissions are calculated in a similar way by combining various activity statistics (e.g., industrial production, use of products) with the methodologies from the guidelines described above. The activity statistics have been collected from various data sources, including the material use database described earlier. Emission factors are taken from the guidance documents and applied to selected activity data for each sector. Similar to the combustion emissions, the non-combustion emissions are also compared to official UNFCCC and CLRTAP emissions to identify possible outliers and errors, but a detailed comparison was not possible due to the different basis (territory vs. residency principle).'atom-text-editor.vim-mode':

### 2.7. Labor Accounts

Available labor statistics show the global distribution of work conditions from the point of view of
where it occurs, both regionally and in main economic activities. Primary sources for labor inputs were
national labor force surveys, gathered from the International Labour Organization’s (ILO) LABORSTA
database [57], and a combination of labor force and industrial surveys in national accounts, obtained
from the Organisation for Economic Co-operation and Development’s (OECD) STAN database [58].
Labor data from LABORSTA consist of 39 economic sectors, whereas STAN covers up to 60 industries
and thereby provides better resolution compared to the MRIO sectors. Labor data were collected for
labor according to skill level and gender, which allows for the calculation of further quality of labor
indicators such as forced labor, child labor, vulnerable employment and damage-related indicators of
labor through occupational health damage see Simas et al. [18,19].

### 2.8. Water Accounts

EXIOBASE is a comprehensive database with a high level of sector disaggregation. In contrast, the
available data on water use and consumption collected by national statistical agencies, for example,
are not of sufficient coverage or quality to fit the requirements of EXIOBASE—or simply altogether
non-existent. As a consequence, modeled data covering the following categories were used. In the
following, we describe the sectors for which data were used with regard to the type of water (blue/green)
and the type of water flow (use/consumption). “Blue water” refers to water abstracted from surface water
and groundwater bodies, whereas “green water” refers to water from precipitation, which infiltrates into
the soil and is taken up by plants. “Water use” is the amount of water abstracted from water sources,
whereas “water consumption” in the hydrological sense is the difference between the water abstracted
and the water returned to the same watershed/ecosystem. In hydrological accounting terms, water
consumption is defined as water evapotranspiration plus water incorporated into products [59].
 Agricultural water consumption (blue/green)
 Industrial water use and consumption (blue)
 Domestic water use and consumption (blue)
 Agricultural nitrogen and phosphorous emissions to water
 Thermal pollution of (heat emissions to) water from energy production
This last item addressing thermal discharges to water is a new quality aspect thus far unaddressed by
the SEEA.
This data allows coverage of both water quality issues and emissions to water, thus permitting water
use to be linked to actual environmental impacts [59]. Collection, classification and disaggregation of
the water data were required before use. These steps were of special relevance in the case of industrial
water use/consumption, wherein data from the WaterGAP model were used [60]. In contrast to the data
on agricultural water appropriation, these data are not available in the full product detail, but for only
five manufacturing sectors, two energy-producing sectors of different types of cooling systems
(once-through vs. tower cooling), as well as for different types of livestock breeding. Hence, these data
had to be allocated to the different product (and industry) groups used in EXIOBASE2. While this was a
relatively straightforward task in the case of the livestock data, the data on water appropriation in the
manufacturing sector had to be allocated to the more detailed EXIOBASE2 product classes using
physical production quantity data for the different products. In the case of energy production, the data
were allocated to the energy types that use cooling water in their production systems. Next, the data
were allocated to the specific EXIOBASE2 sectors via the monetary data from the SUTs on sectorial
activities [59].

### 2.9. Material Accounts

Data for the material extensions were retrieved from the Sustainable Europe Research Institute
(SERI) Global Material Flow database [61]. The Global Material Flow Database is the only database
with global coverage that comprises comprehensive resource extraction data for all material categories
in annual time series. The database is organized according to the standards of economy-wide material
flow accounting (MFA) as provided by Eurostat and the OECD [62,63].
The data in the Global Material Flow Database are mainly based on four data sources: the British
Geological Survey (BGS) and the US Geological Survey (USGS) for metal and mineral data;
the International Energy Agency (IEA) for the data on fossil fuels; and the Food and Agriculture
Organization of the United Nations (FAO) for the data on biomass extraction.

### 2.10. Land Accounts

Cropland data are collected on the individual crop basis (primary crop classification in FAOSTAT),
and supplemented by categories not commonly reported in statistics such as fallow land, forestry
plantations on arable land and land for other agricultural purposes (see [64] for full details on land use
data). In addition to the FAO online database, data and information were taken from a multitude of
single, specific sources as documented in the detailed report found in the supporting information for this
study. Also, Eurostat data for the aggregate categories “forage plants” and “fallow land” were taken
from the agricultural database to fill data gaps or replace FAO data.
FAO data for primary crops inherit specific properties, including the double or multiple counts of
land use in the case of multiple cropping in the span of one year. Such cropping practices are only
counted once in the EXIOBASE2 extensions.

In addition to cropland, permanent meadows and pastures constitute the remainder of utilized
agricultural land, and FAO reports permanent meadows and pastures as a single number. Forest area is a
single number in FAO statistics comprising both natural forests as well as managed forests and
plantations. Only the total area is reported; the statistics do not distinguish between the forest categories.
Built-up and related land encompasses all developed land, including transport corridors and human
settlements. The base data for the category are the 2011 Annex 1 Party Greenhouse Gas (GHG)
Inventory Submissions under the UNFCCC. Since these data do not cover all EXIOBASE2 countries
and are not complete for some regions, we used additional single-country sources or international data
such as from the European Corine Land Cover project.


[^fo]: https://www.mdpi.com/2071-1050/7/1/138/htm
[^ca]: Energy carriers include electricity and heat as well as solid, liquid and gaseous fuels. They occupy intermediate steps in the energy-supply chain between primary sources and end-use applications. An energy carrier is thus a transmitter of energy.
[^FISIM]: In the System of National Accounts it is an estimate of the value of the services provided by financial intermediaries, such as banks, for which no explicit charges are made; instead these services are paid for as part of the margin between rates applied to savers and borrowers. The supposition is that savers would receive a lower interest rate and borrowers pay a higher interest rate if all financial services had explicit charges.
[^trprin]: Emission accounts follow the so-called residence principle – that is, address the activities undertaken by the residents of a country, independent from where these take place – while emission inventories (as those used in the context of the Kyoto Protocol) follow the territory principle – that is, address the activities taking place within the territory, independent from where the subject resides.
