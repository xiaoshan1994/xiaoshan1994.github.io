---
title: "A manual of Cometrade Plus "
date: 2022-01-27T20:01:16+01:00
description: ""
categories:
- Plastic
- Database
tags:
- abbreviation
- manual
keywords:
- tech
metaAlignment: left
thumbnailImage: https://www.insper.edu.br/wp-content/uploads/2021/01/UN_Comtrade.png
thumbnailImagePosition: left
metaAlignment: left
Math: True
---

<!--more-->

{{< toc >}}

# Trade Flow/rgDesc

| flwCode | flwDescription                           | flwCategory |
|---------|------------------------------------------|-------------|
| -1      | Not available or not specified.          |             |
| M       | Import                                   | M           |
| X       | Export                                   | X           |
| RX      | Re-export                                | X           |
| RM      | Re-import                                | M           |
| MIP     | Import of goods for inward processing    | M           |
| XIP     | Export of goods after inward processing  | X           |
| MOP     | Import of goods after outward processing | M           |
| XOP     | Export of goods for outward processing   | X           |
| MIF     | Import on intra-firm trade               | M           |
| XIF     | Export on intra-firm trade               | X           |
| DX      | Domestic Export                          | X           |
| FM      | Foreign Import                           | M           |

## Outward processing
[From WCO](http://www.wcoomd.org/en/topics/facilitation/instrument-and-tools/conventions/pf_revised_kyoto_conv/kyoto_new/spanf.aspx)
{{< hl-text orange>}}Goods in free circulation in a Customs territory may be temporarily exported for manufacturing, processing or repair abroad and then re-imported with total or partial exemption (/ɪɡ'zempʃn/) (or total or partial relief) from import duties and taxes.{{< /hl-text >}}

[Outward processing from EU commission](https://ec.europa.eu/taxation_customs/business/customs-procedures-import-and-export/what-exportation/outward-processing_en)
Outward processing means that Union goods may be {{< hl-text blue>}}temporarily exported{{< /hl-text >}} from the customs territory of the Union in order to {{< hl-text blue>}}undergo processing operations{{< /hl-text >}}. The processed products resulting from these goods can be re-imported and released for free circulation with {{< hl-text blue>}}total or partial relief from import duty{{< /hl-text >}}. {{< hl-text orange>}}A total relief from import duties must be granted when the goods have been exported merely to be repaired free of charge because of a {{< hl-text blue>}}contractual obligation{{< /hl-text >}} or because of {{< hl-text blue>}}a manufacturing or material defect{{< /hl-text >}}.{{< /hl-text >}} {{< hl-text orange>}}In other cases of outward processing, the import duties on the re-imported products are calculated only on the basis of the value resulting from {{< hl-text blue>}}the processing operation{{< /hl-text >}} undertaken outside the customs territory of the Union.{{< /hl-text >}}

Outward processing procedure is designed to give businesses the possibility to take advantage of benefits such as {{< hl-text blue>}}lower labour costs{{< /hl-text >}} or {{< hl-text blue>}}specific technical expertise{{< /hl-text >}} in non-EU countries.

[Inward processing from EU commission](https://ec.europa.eu/taxation_customs/business/customs-procedures-import-and-export/what-importation/inward-processing_en)

## Inward processing
[From WCO](http://www.wcoomd.org/en/topics/facilitation/instrument-and-tools/conventions/pf_revised_kyoto_conv/kyoto_new/spanf.aspx)
{{< hl-text orange>}}Goods can be brought into a Customs territory conditionally relieved from payment of import duties and taxes, on the basis that such goods are intended for manufacturing, processing or repair and subsequent exportation.{{< /hl-text >}}

Inward processing means that {{< hl-text blue>}}non-Union goods{{< /hl-text >}} are imported in order to be used in the customs territory of the Union in {{< hl-text blue>}}one or more processing operations{{< /hl-text >}}, for instance, for the purposes of {{< hl-text blue>}}manufacturing or repair{{< /hl-text >}}. {{< hl-text orange>}}When imported, such goods are not subject to: Import duty, other taxes related to their import, such as VAT and/or excises, and commercial policy measures.{{< /hl-text >}}

{{< hl-text orange>}}Inward processing procedure is designed to give businesses the possibility to process goods imported from outside the customs territory of the Union even before they decide, according to logistical, commercial or other conditions, whether to sell the finished products within the Union or outside.{{< /hl-text >}} The inward processing procedure can also be used for goods which just have to undergo standard forms of handling intended to preserve them, improve their appearance or marketable quality or prepare them for distribution or resale.

After the processing operations, the processed products can be either re-exported or released for free circulation in the EU; {{< hl-text orange>}}the latter (free circulation) would imply the obligation to pay import duty and taxes, as well as the application of commercial policy measures.{{< /hl-text >}} In addition, it is also possible to store processed products under customs warehousing or in a free zone.

## Intra-firm trade
International flows of goods and services between parent companies and their affiliates or among these affiliates.

# Customs Proc. Code and Customs/cstCode and cstDescription

| cstCode | cstDescription                                     |
|---------|----------------------------------------------------|
| -1      | Not available or not specified or no customs code. |
| C00     | All customs procedure codes                        |
| C01     | Clearance for home use                             |
| C02     | Reimportation in the same state                    |
| C03     | Outright exportation                               |
| C04     | Customs warehouses                                 |
| C05     | Free zone                                          |
| C06     | Inward processing                                  |
| C07     | Outward processing                                 |
| C08     | Drawback                                           |
| C09     | Processing of goods for home use                   |
| C10     | Carriage of goods coastwise                        |
| C11     | Customs offences                                   |
| C12     | Travellers                                         |
| C13     | Postal traffic                                     |
| C14     | Stores                                             |
| C15     | Relief consignments                                |
| C20     | CPC N.E.S.                                         |

[Text of the Revised Kyoto Convention](http://www.wcoomd.org/en/Topics/Facilitation/Instrument%20and%20Tools/Conventions/pf_revised_kyoto_conv/Kyoto_New)

| Specific Annexes |         | Specific Annex guidelines* |             |
|:----------------:|:-------:|:--------------------------:|:-----------:|
| A | Arrival of goods in a Customs territory | A1 | Formalities prior to the lodgement of the Goods declaration* |
|                  |                          | A2 | Temporary storage of goods*                                  |
| B | Importation                             | B1 | Clearance for home use*                                      |
|                  |                          | B2 | Re-importation in the same state*                            |
|                  |                          | B3 | Relief from import duties and taxes*                         |
| C                | Exportation              | C1 | Outright exportation*                                        |
| D                | Customs warehouses and free zones | D1 | Customs warehouses*                                 |
|                  |                          | D2 | Free zones*                                                  |
| E                | Transit                  | E1 | Customs transit*                                             |
|                  |                          | E2 | Transhipment*                                                |
|                  |                          | E3 | Carriage of goods coastwise*                                 |
| F                | Processing               | F1 | Inward processing*                                           |
|                  |                          | F2 | Outward processing*                                          |
|                  |                          | F3 | Drawback*                                                    |
|                  |                          | F4 | Processing of goods for home use*                            |
| G                | Temporary admission      | G1 | Temporary admission*                                         |
| H                | Offences                 | H1 | Customs offences*                                            |
| J                | Special procedures       | J1 | Travellers*                                                  |
|                  |                          | J2 | Postal traffic*                                              |
|                  |                          | J3 | Means of transport for commercial use*                       |
|                  |                          | J4 | Stores*                                                      |
| K                | Origin                   | J5 | Relief consignments*                                         |

“clearance for home use” means the Customs procedure which provides that {{< hl-text blue>}}imported goods enter into free circulation{{< /hl-text >}} in the Customs territory upon the payment of any import duties and taxes chargeable and the accomplishment of all the necessary Customs formalities.

“goods in free circulation” means goods which may {{< hl-text blue>}}be disposed of without Customs restriction{{< /hl-text >}}.

“re-importation in the same state” means the Customs procedure under which exported goods may be taken into home use and free of import duties and taxes, provided {{< hl-text blue>}}they have not undergone any manufacturing, processing or repairs abroad{{< /hl-text >}}. The goods that are eligible for re-importation in the same state can be goods that were in free circulation or were compensating products.

“drawback” means the amount of import duties and taxes repaid under the drawback procedure;

“drawback procedure” means the Customs procedure which, when goods are exported, provides for a repayment (total or partial) to be made in respect of the import duties and taxes charged on the goods, or on materials contained in them or consumed in their production;

“temporary admission” means the Customs procedure under which certain goods can be brought into a Customs territory conditionally relieved totally or partially from payment of import duties and taxes; such goods must be imported for a specific purpose and must be intended for re-exportation within a specified period and without having undergone any change except normal depreciation due to the use made of them.

[Temporary admission in EU](https://ec.europa.eu/taxation_customs/business/customs-procedures-import-and-export/what-importation/specific-use_en#:~:text='Temporary%20admission'%20allows%20goods%20to,part%20in%20a%20music%20show.)
Such as exhibiting at a trade fair or taking part in a music show. In some cases the completion of customs formalities is not required (e.g. temporary admission of means of transport).
An ATA or CPD carnet can be used for temporary admission. It covers professional equipment, goods for presentation or use at trade fairs, shows, exhibitions and the like commercial samples.

“{{< hl-text blue>}}stores{{< /hl-text >}}” means : stores for consumption(consumption goods and fuel for passengers and the crew) and stores to be taken away(consumption for being landed).

“Customs warehousing procedure” means the Customs procedure under which imported goods are stored under Customs control in a designated place (a Customs warehouse) without payment of import duties and taxes.



"free zone" means an area at a port where certain customs restrictions are not implemented (*from collinsdictionary.com*)
# About free zones
[*Practical Guidance on Free Zones* by World Customs Organization December 2020](http://www.wcoomd.org/-/media/wco/public/global/pdf/topics/facilitation/activities-and-programmes/free-zone/wco-fz-guidance_en.pdf?la=en)
![image](https://user-images.githubusercontent.com/65668613/151524265-91059387-43e7-4ccf-a597-64b75a7a14c2.png)
> FZs attract not only legitimate business, but also illicit activities that take advantage of regulatory exemptions in FZs and the lack of oversight therein. Such illicit activities include money laundering, tax evasion and trade in counterfeit goods or other illicit goods, such as drugs, weapons, cultural heritage, fake medicines and even environmental waste.

> Customs should establish basic construction standards and other standards to be implemented in FZs for Customs control. This covers Customs checkpoints, enclosed fencing surrounding the FZ, Customs inspection areas, video surveillance systems, installation of non-intrusive inspection (NII) equipment, the information network to be interfaced with Customs, etc.

![image](https://user-images.githubusercontent.com/65668613/151522849-dc64f5db-3868-4df7-ac32-0127c49f6789.png)

[‘Extraterritoriality’ of Free Zones: The Necessity for Enhanced Customs Involvement, WCO Research Paper No. 47, September 2019](http://www.wcoomd.org/-/media/wco/public/global/pdf/topics/research/research-paper-series/47_free_zones_customs_involvement_omi_en.pdf?la=en.)
The following factors contributing to risks associated with Free Zones:
* Relaxed controls inside FZ
* Insufficient Customs' involvement in the operation of FZ
* Ease in setting up companies inside FZ
* Insufficient integration of Information Technology(IT) systems by governmental agencies inside FZ.

![image](https://user-images.githubusercontent.com/65668613/151533777-e514fc22-ac73-4c37-85b4-6c8c773bd96c.png)

![image](https://user-images.githubusercontent.com/65668613/151537612-c62e83ea-5777-4775-933e-486ccfa0f841.png)

Anecdotal examples of illicit trade

![image](https://user-images.githubusercontent.com/65668613/151538994-99211c24-2ef5-4c29-ad39-45b0b583bcd5.png)

![image](https://user-images.githubusercontent.com/65668613/151539048-5792fbe2-ecfd-4f83-a29a-109cc275098a.png)

# Rules of Origin
[WTO](https://www.wto.org/english/tratop_e/roi_e/roi_info_e.htm#:~:text=Rules%20of%20origin%20are%20the,to%20the%20rules%20of%20origin.)
Rules of origin are the criteria needed to determine {{< hl-text blue>}}the national source of a product{{< /hl-text >}}. Their importance is derived from the fact that duties and restrictions in several cases depend upon the source of imports.

While the requirement of substantial transformation is universally recognized, some governments apply the criterion of change of tariff classification, others the ad valorem percentage criterion and yet others the criterion of manufacturing or processing operation.

Rules of origin are used:
— to implement measures and instruments of commercial policy such as {{< hl-text blue>}}anti-dumping duties and safeguard measures{{< /hl-text >}};
— to determine whether imported products shall receive {{< hl-text blue>}}most-favoured-nation (MFN) treatment{{< /hl-text >}} or {{< hl-text blue>}}preferential treatment{{< /hl-text >}};
— for the purpose of trade statistics;
— for the application of labelling and marking requirements; and
— for government procurement.
