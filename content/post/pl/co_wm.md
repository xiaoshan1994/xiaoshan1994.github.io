---
title: "(Collection) Waste management"
date: 2022-05-24T16:46:53+02:00
categories:
- plastic
- collection
thumbnailImage: https://safetyculture.com/wp-content/media/2021/06/Waste-Management-Life-Cycle.png
thumbnailImagePosition: left
metaAlignment: left
Math: True
---
<!--more-->

{{< toc >}}
# Open Dumping
[Illinois Environmental Protection Agency](https://www2.illinois.gov/epa/topics/waste-management/illegal-dumping/Pages/open-dumping.aspx)
 An open dump is an {{< hl-text blue>}}illegal waste disposal site{{< /hl-text >}} and should not be confused with a permitted municipal solid waste landfill or a recycling facility
![](https://www2.illinois.gov/epa/topics/waste-management/illegal-dumping/PublishingImages/open-dump.jpg)
Any of the following seven conditions at a dump site can result in the issuance of an Administrative Citation:
* Litter
* Scavenging
* Open burning
* Placement of waste in standing or flowing water
* Promoting an increase of disease-carrying organisms
* Standing or flowing liquid discharge from the dump site
* Deposition of construction or demolition debris

# The Open Dump Dilemma: How to Help the Environment and Respect Human Rights
**1 March 2020**
**Women in Informal Employment: Globalizing and Organizing (WIEGO)**
https://www.wiego.org/blog/open-dump-dilemma-how-help-environment-and-respect-human-rights

> Open dumps, unlike sanitary landfills, are not engineered to protect the environment and human health...these sites are important sources of economic survival for expert recyclers – the world’s waste pickers – who earn a daily living there and feed our waste into the global recycling chain.

* Open dumps are the most prevalent form of waste disposal in the Global South.

# Inventory parameters for regionalised mixes of municipal waste disposal in ecoinvent v3.5 (2018)
Technical report Zurich, **December 2018**
**Gabor Doka**
Doka Life Cycle Assessments, Zurich
ecoinvent Association, Zurich
https://www.doka.ch/WasteDisposalMixDoka2018.pdf

## Highlights
* New activities are open burning, open dumping and unsanitary landfill.
* Five different climate classes are created based on annual water infiltration
* The devised methodology allows to create additional market mixes for other countries in the future as well as inputs of updated statistical data.

Employed disposal activities in the model encompass a selection of {{< hl-text blue>}}unmanaged activities (open burning, open dumping){{< /hl-text >}}, and {{< hl-text blue>}}activities managed to different degrees (unsanitary landfill, sanitary landfill, municipal incineration){{< /hl-text >}}.

we decided to create {{< hl-text blue>}}five different climate classes{{< /hl-text >}} based on {{< hl-text blue>}}annual water infiltration{{< /hl-text >}} to discern the different local conditions, instead of inventorying the activities of each country with their specific climate.

From the present project, ecoinvent inventories for market mixes for {{< hl-text blue>}}37 European countries{{< /hl-text >}} are created, plus {{< hl-text blue>}}five focus countries of the Sustainable Recycling Initiative SRI{{< /hl-text >}} (Brazil, Colombia, Peru, India, South Africa).

{{< hl-text orange>}}Swiss disposal technologies in 1992{{< /hl-text >}}:
* municipal incineration with elaborate flue gas cleaning
* well-engineered sanitary landfills with landfill gas capture[^LFG] and leachate treatment
* well buffered residual material landfills for polluted inorganic waste

## 1. Municipal waste disposal technology mix
(d). Open dump ({{< hl-text orange>}}unmanaged{{< /hl-text >}})
  {{< hl-text blue>}}Uncollected waste{{< /hl-text >}} or collected waste with unmanaged disposals.

(b). Open burning ({{< hl-text orange>}}unmanaged{{< /hl-text >}})
  Uncollected waste or collected waste with unmanaged disposals.

(u).  Unsanitary landfill ({{< hl-text orange>}}minimal management{{< /hl-text >}})
  Waste is {{< hl-text blue>}}compacted{{< /hl-text >}} and a {{< hl-text blue>}}daily cover{{< /hl-text >}} is applied. This mitigates the direct unhygienic effects of dumps, but {{< hl-text blue>}}emissions to air or water{{< /hl-text >}} remain unmitigated. The waste compaction and a daily waste cover leads to {{< hl-text blue>}}lower methane oxidation compared to open dumps{{< /hl-text >}} and therefore **{{< hl-text blue>}}larger methane emissions{{< /hl-text >}}**, which is modelled in the unsanitary landfill model.

(s). Sanitary landfill ({{< hl-text orange>}}managed plant{{< /hl-text >}})
  sanitary landfills {{< hl-text blue>}}capture some landfill gas and treat the leachate{{< /hl-text >}}. In LCA results the {{< hl-text blue>}}flaring or utilization of landfill gas{{< /hl-text >}} is the most relevant difference compared to unsanitary landfills. Where information is available on landfill gas utilisation, it can be incorporated into the technology mix.

(m). Municipal incineration ({{< hl-text orange>}}managed plant{{< /hl-text >}})
  Municipal incineration plants are {{< hl-text blue>}}costly investments{{< /hl-text >}} and are currently only observed in countries with a {{< hl-text blue>}}Gross National Income (GNI) above 10'000 $/capita.yr{{< /hl-text >}}. In countries below that threshold incineration can very likely be excluded.

The criteria to assign waste disposal technology over countries:
* Collection, management of collected waste
* occurrence of fires in dumps/landfills
* Gross National Income (GNI) above or below 10'000 $/capita.yr

![image](https://user-images.githubusercontent.com/65668613/170224741-d7b28276-c7f3-4baa-8a62-3850ad2014ad.png)

### 1.1 Collected waste
Collected% - percentage of generated waste being collected, in mass percent of generated waste.

Source:
1. percentage of the population being served by waste collection ([UN
statistics](https://unstats.un.org/unsd/envstats/Questionnaires/2019/Tables/Total%20population%20served%20by%20municipal%20waste%20collection.xlsx), 74 countries, 1990-2017)
2. Based on Gross National Income per capita (GNI)
![image](https://user-images.githubusercontent.com/65668613/170231914-10d041c0-0868-4322-a984-795337330dab.png)

![image](https://user-images.githubusercontent.com/65668613/170232186-0552a6e7-81fe-4a23-b5c5-82a3d869ad81.png)

### 1.2 Uncontrolled vs. controlled disposal
Some part of the collected waste can be assumed to end up in uncontrolled, unmanaged disposals.
![image](https://user-images.githubusercontent.com/65668613/170232699-29ab751d-5c02-4199-a47f-111626121457.png)

For large collection rates, the fraction of collected waste going to managed, controlled disposals is large.

![image](https://user-images.githubusercontent.com/65668613/170232950-87aa8b79-b7fa-48e2-a505-972b08ac47a8.png)

the part of the generated waste going into unmanaged, uncontrolled
disposals:
![image](https://user-images.githubusercontent.com/65668613/170233155-35d6ba6d-2063-4a67-8398-7f10d1d6303f.png)

### 1.3 Open burning
![image](https://user-images.githubusercontent.com/65668613/170445136-ae451fa0-87ff-46be-979a-d6fac8ca0a6e.png)

![image](https://user-images.githubusercontent.com/65668613/170446375-e07d7da6-a02c-4b42-bd05-2b4b27d79067.png)

![image](https://user-images.githubusercontent.com/65668613/170446477-fe8ba37a-9834-400c-a3b5-a7eb8f79bb69.png)

### 1.4 Open dumping
![image](https://user-images.githubusercontent.com/65668613/170446931-d4d35d58-4344-4dd6-810c-d72e2ef63c6f.png)

### 1.5 Unsanitary landfills
![image](https://user-images.githubusercontent.com/65668613/170451874-c5cf2f38-3c1b-44c9-a5e4-83ac6ad80a62.png)

The mass landfilled in an unsanitary landfill will be further modified by subtracting an estimated amount of waste being burnt off in landfill fires.

### 1.6 Landfill Fires
![image](https://user-images.githubusercontent.com/65668613/170452331-a67766bd-89b5-4b43-aad7-272f0624ddb5.png)

### 1.7 Sanitary landfills
In the sanitary landfill inventory model, {{< hl-text blue>}}landfill gas can be captured and flared or utilized and the leachate is captured and treated{{< /hl-text >}}.

Country-wise information on the quantitative extent of landfill gas capture is difficult to obtain.

### 1.8 Municipal incineration
* masses into waste incineration plants is available from Eurostat and OECD data
* The statistical data shows that in most countries practically 100% of incinerators also perform energy recovery.

## 2. Data reduction: Infiltration classes
In the model, {{< hl-text blue>}}scarcity of available precipitation water can influence the amount of landfill gases{{< /hl-text >}}. The rate of water infiltrating the landfill body determines the speed of weathering of the landfill and influences inventoried emissions from the landfill body.

Each country or region can be assigned to a class of five infiltration rates. Infiltration in the landfill model is annual precipitation minus annual
actual evapotranspiration.![]()
![image](https://user-images.githubusercontent.com/65668613/170456840-81522d39-506e-4999-84f9-ea2ffaa83468.png)
![image](https://user-images.githubusercontent.com/65668613/170457440-e4cf0afc-126c-44e9-8897-f50865b6d463.png)
![image](https://user-images.githubusercontent.com/65668613/170457570-33517d62-3ac2-42ac-ad47-a090066ca1aa.png)
![image](https://user-images.githubusercontent.com/65668613/170457626-97cfe152-41df-4816-a6dd-9cda109c5e2f.png)

## 3. Municipal waste treatment markets
### 3.1 Treatment technology mix
![image](https://user-images.githubusercontent.com/65668613/170459864-4bdc8ef4-46a3-4cb4-bbe7-31283c6a4281.png)

### 3.2 Waste treatment production volumes
![image](https://user-images.githubusercontent.com/65668613/170460932-fc575f76-4cea-4b4a-8e27-be3ea00753c7.png)

### 3.2.1 Discerned waste materials
{{< hl-text orange>}}Tab. 5.2 List of generic waste materials in mixed munici![]()pal waste used to generate new disposal activities in ecoinvent v3.5.{{< /hl-text >}}
1. graphical paper; packaging paper; paperboard
2. plastic, mixture; polyethylene (PE); polyethylene terephtalate (PET); polypropylene (PP); polystyrene(PS); polyurethane(PU,聚亚安酯); polyvinylchloride (PVC,聚氯乙烯)
4. glass
5. wood, untreated

### 3.2.2 Country-specific mass of disposed mixed municipal waste
{{< hl-text orange>}}Generated mass{{< /hl-text >}}
per-capita waste generation mMSW and a country's population by simple multiplication

{{< hl-text orange>}}Recycling rate{{< /hl-text >}}
* OECD data
  - From data for 45 OECD countries the entries for '{{< hl-text blue>}}Recycling{{< /hl-text >}}', '{{< hl-text blue>}}Composting{{< /hl-text >}}' and '{{< hl-text blue>}}Other recovery{{< /hl-text >}}' were added and then divided by the '{{< hl-text blue>}}Municipal waste generated{{< /hl-text >}}' figure to obtain a recycling rate.
* Eurostat data
  - From data for 40 European countries (including non-EU) the entries for '{{< hl-text blue>}}Material recycling{{< /hl-text >}}' and '{{< hl-text blue>}}Composting and digestion{{< /hl-text >}}' were added and then divided by the 'Waste generated' figure to obtain a recycling rate.

With data on the generated waste and the recycling rate it is now possible to calculate the non-recycled disposed waste mass as mD = mMSW ⋅ (1 – r).
The generated waste mass mMSW and disposed, non-recycled waste mass
mD.

### 3.2.3 Country-specific composition of disposed mixed municipal waste
{{< hl-text blue>}}Waste fraction analysis {{< /hl-text >}}for around 100 countries is available from UN statistics (UNSD 2016b), which is based on UN questionnaires, EU or OECD statistics with the majority of data originating in the period 2000-2013. This UN data however only discerns the following waste fractions: "Paper, paperboard", "Organic material", "Plastics", "Glass", "Metals", "Textiles", "Other inorganic material".

![image](https://user-images.githubusercontent.com/65668613/170530315-4499b5ee-007a-407d-9dcc-74407c9b8a68.png)

{{< hl-text orange>}}Subdividing Plastics{{< /hl-text >}}
The {{< hl-text blue>}}UN fraction "Plastics"{{< /hl-text >}} corresponds to the target fraction {{< hl-text blue>}}"plastic, mixture"{{< /hl-text >}}. Therefore this can be applied directly.

This method of using production input data to estimate waste data is flawed with respect of assuming that all polymer types have the same short lifetime. In a market that has not reached a steady state or plateau this means that polymer shares in production are not the same as polymer shares in disposal.
![image](https://user-images.githubusercontent.com/65668613/170531992-a9285c38-54e6-420d-a3fc-6d70d671aff8.png)

## LCI calculation tools  for regionalised waste treatment  – General introduction (2020)
Technical report, version 2, Zurich, July 2020

* Patterns of household waste disposal methods in developing countries vary according to climate, housing conditions, availability and cost of waste collection services, local regulations, cultural and other factors. Also the characteristics of the waste itself (smell, attractiveness to flies and rodents) determines disposal habits.

### Brazil{{< hl-text orange>}}
* sanitary landfill in Brazil are very diverse.
* 25% (147) reported to have neither base seal, nor gas collection pipes, nor any form of leachate collection and treatment.
* Incineration is only a targeted treatment for {{< hl-text blue>}}health care waste{{< /hl-text >}}, septic waste and food waste from ports and airports. {{< hl-text blue>}}Incineration of household waste can therefore be considered negligible in the current Brazilian situation{{< /hl-text >}}.
* Waste incineration is usually not practiced in {{< hl-text blue>}}all of Latin America{{< /hl-text >}}. Only Brazil and some Caribbean islands have experience with urban solid waste incinerators (PAHO 2010:130).

### India
* Urban households and businesses usually collect waste {{< hl-text blue>}}in a single bin{{< /hl-text >}}. Waste separation at the source is not commonly performed.
* a rate of 88% all generated municipal waste will probably end up
in open dumps and other unhygienic treatments
* The Indian national average landfill gas capture rate estimated for 2007 was very close to zero, as only a few small pilot projects in large cities exist.
* 6 waste incinerator plants existed in 2015; 12 facilities for refuse derived fuels (RDF); 600 digester plants for biowaste existed; 95 local bodies of a total of 203'700 have set up sanitary landfills

### South Africa
* In 2014 {{< hl-text blue>}}66%{{< /hl-text >}} of all households having municipal waste collection services while others having their own informal refuse dumps or communal waste dumps (no collection service) or simply littered their waste.
![image](https://user-images.githubusercontent.com/65668613/170819966-72884e88-6bfc-4ac4-af84-d9ee6d78cf62.png)
* "disposal to land" signifies an engineered landfill, while "disposal to landfill" is coined for more specific disposal in a non-engineered landfill (informal and open dumps).




[^LFG]: [Landfill gas (LFG)](https://www.epa.gov/lmop/basic-information-about-landfill-gas#:~:text=LFG%20is%20extracted%20from%20landfills,in%20an%20LFG%20energy%20project.) is a natural byproduct of the decomposition of organic material in landfills. LFG is composed of roughly 50 percent methane (the primary component of natural gas), 50 percent carbon dioxide (CO2) and a small amount of non-methane organic compounds.