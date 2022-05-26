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

# Inventory parameters for regionalised mixes of municipal waste disposal in ecoinvent v3.5
Technical report Zurich, **December 2018**
**Gabor Doka**
Doka Life Cycle Assessments, Zurich
ecoinvent Association, Zurich
https://www.doka.ch/WasteDisposalMixDoka2018.pdf

Employed disposal activities in the model encompass a selection of {{< hl-text blue>}}unmanaged activities (open burning, open dumping){{< /hl-text >}}, and {{< hl-text blue>}}activities managed to different degrees (unsanitary landfill, sanitary landfill, municipal incineration){{< /hl-text >}}.

we decided to create {{< hl-text blue>}}five different climate classes{{< /hl-text >}} based on {{< hl-text blue>}}annual water infiltration{{< /hl-text >}} to discern the different local conditions, instead of inventorying the activities of each country with their specific climate.

From the present project, ecoinvent inventories for market mixes for {{< hl-text blue>}}37 European countries{{< /hl-text >}} are created, plus {{< hl-text blue>}}five focus countries of the Sustainable Recycling Initiative SRI{{< /hl-text >}} (Brazil, Colombia, Peru, India, South Africa).

{{< hl-text orange>}}Swiss disposal technologies in 1992{{< /hl-text >}}:
* municipal incineration with elaborate flue gas cleaning
* well-engineered sanitary landfills with landfill gas capture[^LFG] and leachate treatment
* well buffered residual material landfills for polluted inorganic waste

## Municipal waste disposal technology mix
1. Open dump ({{< hl-text orange>}}unmanaged{{< /hl-text >}})
  {{< hl-text blue>}}Uncollected waste{{< /hl-text >}} or collected waste with unmanaged disposals.

2. Open burning ({{< hl-text orange>}}unmanaged{{< /hl-text >}})
  Uncollected waste or collected waste with unmanaged disposals.

3. Unsanitary landfill ({{< hl-text orange>}}minimal management{{< /hl-text >}})
  Waste is {{< hl-text blue>}}compacted{{< /hl-text >}} and a {{< hl-text blue>}}daily cover{{< /hl-text >}} is applied. This mitigates the direct unhygienic effects of dumps, but {{< hl-text blue>}}emissions to air or water{{< /hl-text >}} remain unmitigated. The waste compaction and a daily waste cover leads to {{< hl-text blue>}}lower methane oxidation compared to open dumps{{< /hl-text >}} and therefore **{{< hl-text blue>}}larger methane emissions{{< /hl-text >}}**, which is modelled in the unsanitary landfill model.

4. Sanitary landfill ({{< hl-text orange>}}managed plant{{< /hl-text >}})
  sanitary landfills {{< hl-text blue>}}capture some landfill gas and treat the leachate{{< /hl-text >}}. In LCA results the {{< hl-text blue>}}flaring or utilization of landfill gas{{< /hl-text >}} is the most relevant difference compared to unsanitary landfills. Where information is available on landfill gas utilisation, it can be incorporated into the technology mix.

5. Municipal incineration ({{< hl-text orange>}}managed plant{{< /hl-text >}})
  Municipal incineration plants are {{< hl-text blue>}}costly investments{{< /hl-text >}} and are currently only observed in countries with a {{< hl-text blue>}}Gross National Income (GNI) above 10'000 $/capita.yr{{< /hl-text >}}. In countries below that threshold incineration can very likely be excluded.

The criteria to assign waste disposal technology over countries:
* Collection, management of collected waste
* occurrence of fires in dumps/landfills
* Gross National Income (GNI) above or below 10'000 $/capita.yr

![image](https://user-images.githubusercontent.com/65668613/170224741-d7b28276-c7f3-4baa-8a62-3850ad2014ad.png)

### waste collection rate
Collected% - percentage of generated waste being collected, in mass percent of generated waste.

Source:
1. percentage of the population being served by waste collection ([UN
statistics](https://unstats.un.org/unsd/envstats/Questionnaires/2019/Tables/Total%20population%20served%20by%20municipal%20waste%20collection.xlsx), 74 countries, 1990-2017)
2. Based on Gross National Income per capita (GNI)
![image](https://user-images.githubusercontent.com/65668613/170231914-10d041c0-0868-4322-a984-795337330dab.png)

![image](https://user-images.githubusercontent.com/65668613/170232186-0552a6e7-81fe-4a23-b5c5-82a3d869ad81.png)

### Uncontrolled vs. controlled disposal
Some part of the collected waste can be assumed to end up in uncontrolled, unmanaged disposals.
![image](https://user-images.githubusercontent.com/65668613/170232699-29ab751d-5c02-4199-a47f-111626121457.png)

For large collection rates, the fraction of collected waste going to managed, controlled disposals is large.

![image](https://user-images.githubusercontent.com/65668613/170232950-87aa8b79-b7fa-48e2-a505-972b08ac47a8.png)

the part of the generated waste going into unmanaged, uncontrolled
disposals:
![image](https://user-images.githubusercontent.com/65668613/170233155-35d6ba6d-2063-4a67-8398-7f10d1d6303f.png)

### Open burning
![image](https://user-images.githubusercontent.com/65668613/170445136-ae451fa0-87ff-46be-979a-d6fac8ca0a6e.png)

![image](https://user-images.githubusercontent.com/65668613/170446375-e07d7da6-a02c-4b42-bd05-2b4b27d79067.png)

![image](https://user-images.githubusercontent.com/65668613/170446477-fe8ba37a-9834-400c-a3b5-a7eb8f79bb69.png)

### Open dumping
![image](https://user-images.githubusercontent.com/65668613/170446931-d4d35d58-4344-4dd6-810c-d72e2ef63c6f.png)

### Unsanitary landfills
![image](https://user-images.githubusercontent.com/65668613/170451874-c5cf2f38-3c1b-44c9-a5e4-83ac6ad80a62.png)

The mass landfilled in an unsanitary landfill will be further modified by subtracting an estimated amount of waste being burnt off in landfill fires.

### Landfill Fires
![image](https://user-images.githubusercontent.com/65668613/170452331-a67766bd-89b5-4b43-aad7-272f0624ddb5.png)

### Sanitary landfills
In the sanitary landfill inventory model, {{< hl-text blue>}}landfill gas can be captured and flared or utilized and the leachate is captured and treated{{< /hl-text >}}.

Country-wise information on the quantitative extent of landfill gas capture is difficult to obtain.

## Data reduction: Infiltration classes

In the model, {{< hl-text blue>}}scarcity of available precipitation water can influence the amount of landfill gases{{< /hl-text >}}. The rate of water infiltrating the landfill body determines the speed of weathering of the landfill and influences inventoried emissions from the landfill body.

Each country or region can be assigned to a class of five infiltration rates. Infiltration in the landfill model is annual precipitation minus annual
actual evapotranspiration.![]()
![image](https://user-images.githubusercontent.com/65668613/170456840-81522d39-506e-4999-84f9-ea2ffaa83468.png)
![image](https://user-images.githubusercontent.com/65668613/170457440-e4cf0afc-126c-44e9-8897-f50865b6d463.png)
![image](https://user-images.githubusercontent.com/65668613/170457570-33517d62-3ac2-42ac-ad47-a090066ca1aa.png)
![image](https://user-images.githubusercontent.com/65668613/170457626-97cfe152-41df-4816-a6dd-9cda109c5e2f.png)

## Municipal waste treatment markets




[^LFG]: [Landfill gas (LFG)](https://www.epa.gov/lmop/basic-information-about-landfill-gas#:~:text=LFG%20is%20extracted%20from%20landfills,in%20an%20LFG%20energy%20project.) is a natural byproduct of the decomposition of organic material in landfills. LFG is composed of roughly 50 percent methane (the primary component of natural gas), 50 percent carbon dioxide (CO2) and a small amount of non-methane organic compounds.
