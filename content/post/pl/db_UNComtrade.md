---
title: "UN Comtrade Database"
date: 2022-01-18T09:32:42+01:00
categories:
- Plastic
- Database
keywords:
- tech
thumbnailImage: https://www.insper.edu.br/wp-content/uploads/2021/01/UN_Comtrade.png
thumbnailImagePosition: left
metaAlignment: left
Math: True
---
<!--more-->
{{< toc >}}

[Get data](https://comtrade.un.org/data/)
HS (as reported) commodity codes:
3915 - Waste, parings and scrap. of plastics
391510 - Ethylene polymers; waste, parings and scrap
391520 - Styrene polymers; waste, parings and scrap
391530 - Vinyl chloride polymers; waste, parings and scrap
391590 - Plastics n.e.s in headings no.3915; waste, parings and scarp

https://unstats.un.org/wiki/display/comtrade/Taiwan%2C+Province+of+China+Trade+data
Taiwan, Province of China Trade data
Created by Vysaul Nyirongo, last modified by Ana Mendoza on May 11, 2021

Q: I did not find **Taiwan** trade flow in COMTRADE database. Would it be possible for me to obtain the Taiwan import and export to these partner Hong Kong and Mainland China data from COMTRADE ?

A: For political reasons, the UN is not allowed to show trade statistics referring to Taiwan, Province of China. Yes, in the partner breakdown, Taiwan, Province of China, is included under "Other Asia, not elsewhere specified" (code 490). Data for "Other Asia, nes" is available only to international organizations. {{< hl-text orange>}}In principle, trade data for territories belonging to Asia, but not specified by country, could end up in code 490.{{< /hl-text >}}{{< hl-text blue>}} In practice, only trade of Taiwan, Province of China is included under this code, except for several countries (such as Saudi Arabia, which report all of their exports to unknown countries).{{< /hl-text >}} Trade data for Taiwan, Province of China are not included within China's trade.

https://unstats.un.org/wiki/display/comtrade/World+Trade+Flows%3A+1962-2000
> Note in particular that the NBER-UN country code for Taiwan is ‘454900’.  This code corresponds to the UN country code of  ‘458960’ and the UN country description of  ‘Asia Othr. NS’, so we are imputing Taiwan trade from that classified as ‘Asia other not specified’ by the United Nations

https://www.unece.org/fileadmin/DAM/stats/documents/ece/ces/ge.20/2020/mtg1/4.1_Globalization_TT_UNECE_valuation2020.pdf
 * System of National Accounts 2008 (2008 SNA) recommends recording of imports and exports of goods at FOB value.
 * the FOB valuation seems to not be fully reconciled with the general conceptual principle of recording output at basic prices[^ba]:
  - FOB valuation principle : goods are valued excluding freight and insurance services between the exporting and importing countries (i.e., at a point of {{< hl-text blue>}}**uniform valuation**{{< /hl-text >}}).
  - basic price valuation principle : goods are valued at the **{{< hl-text blue>}}observed transaction price{{< /hl-text >}}** receivable by the producer (freight and insurance services are included or excluded depending on if these services are separately invoiced by the producer).
* Imports of goods are to be recorded in the supply and use tables at basic prices:
 - CIF to FOB adjustment is needed, if FOBtype data detailed by product group are not available for imports.

[^ba]: [The basic price](https://stats.oecd.org/glossary/detail.asp?ID=189) is the amount receivable by the producer from the purchaser for a unit of a good or service produced as output {{< hl-text orange>}}minus any tax payable, and plus any subsidy receivable{{< /hl-text >}}, on that unit as a consequence of its production or sale; {{< hl-text orange>}}it excludes any transport charges invoiced separately by the producer{{< /hl-text >}}.
