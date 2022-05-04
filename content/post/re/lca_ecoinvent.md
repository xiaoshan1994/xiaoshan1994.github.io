---
title: "About ecoinvent"
date: 2022-05-03T16:40:15+02:00
description: ""
categories:
- Research
- Life Cycle Assessment (Training)
tags:
- ecoinvent
thumbnailImage: https://simapro.com/wp-content/uploads/2021/11/ecoinvent-logo-280x280.png
thumbnailImagePosition: left
metaAlignment: left
Math: True
---
<!--more-->
{{< toc >}}
Geographies
# Geographies
For example, Switzerland has the abbreviation CH, Czechia is CZ and China is CN.
Almost every activity in the database is also represented at the global level, using geographical location global (GLO) or Rest-of-the-World (RoW), representing the average global production.

Geographies for the same activity cannot overlap. For example, an activity from Switzerland cannot coexist with the same activity at the European (RER) level since Switzerland is contained within RER. Therefore, geographies such as “Europe without Switzerland” are created. Full and partial overlaps are reported in the geography file.

## Example calculation of the Rest of the World
Let us assume an activity is available for four different regions: the United States (US), India (IN), China (CN), and Global (GLO).

During the linking, the RoW production is generated as a copy of the global dataset. The production volume (PV) of the RoW activity is calculated by subtracting the production volume of the regional activities from the global volume:

PV RoW = PV GLO – PV US – PV IN – PV CN

In supply chains, the newly generated RoW process connects to other processes with overlapping geographical boundaries.

# Activities & Products
The ecoinvent database is a library of activities representing industrial or agricultural processes, each generating a resulting product. Each of these activities can also be called a unit process (UPR). More than 18,000 processes covering around 3,300 distinct products across all economic sectors are included in the latest version of the ecoinvent database.

## Types of activities
Several types of activities can be distinguished and will be described in more detail below. All activities have exchanges on the input side and on the output side.
![image](https://user-images.githubusercontent.com/65668613/166642567-6d9f03d5-56f8-498a-aa20-efefefb5ed80.png)

Exchanges from and to the environment, also called elementary exchanges, are placed on the input side when a process consumes natural resources, such as iron ore from the ground, water from a river or CO2 taken up from the air into a tree. Elementary exchanges are placed on the output side when a process releases emissions into soil, water or air.

All other exchanges are intermediate exchanges, i.e., the products consumed or produced by a process and exchanged with other processes. On the output side, we distinguish between types of products: reference products and by-products or waste.

## Ordinary transforming activities
All activities that are not of the special types described below are “ordinary” transforming activities. Transforming activities are human activities that transform inputs so that the output of the activity is different from the inputs, e.g., a hard coal mine that extracts hard coal in the ground to deliver the marketable product hard coal.

## Treatment activities
Waste in the ecoinvent database has no economic value and is not sold on the market. Since waste are intermediate exchanges, they cannot be released into the environment; but require treatment processes. Treatment processes (treatment activities) convert
* a waste into a valuable product, e.g., used cooking oil needs to be purified to become a valuable input to biofuel production. This process can be seen as recycling.
* a waste into emissions to the environment, i.e., elementary exchanges. An example would be the treatment of polluted wastewater to obtain unpolluted water, which is released into a river. This process can be seen as final disposal.

Treatment activities have a negative reference product, e.g., treatment of inert waste in a landfill has a reference product of -1 kg of inert waste.

The negative sign indicates that the treatment activity supplies the service of treating or disposing of its reference product. For example, the treatment of unsorted waste paper by sorting has unsorted waste paper as a negative reference product. Physically, the reference product is an input to the treatment activity, e.g., the unsorted waste paper is an input to the sorting process. However, reference products in ecoinvent datasets are placed on the output side, and they have a negative sign to maintain the mass balance of the process. The by-products of the treatment activity have a positive sign; they represent valuable products obtained after treatment, e.g., the sorted paper leaving the sorting process.
![image](https://user-images.githubusercontent.com/65668613/166641680-9ec733ad-77f0-410e-b6b2-98669e7e4cf6.png

## Market activities
![image](https://user-images.githubusercontent.com/65668613/166642370-4c8848a2-3697-4813-a149-3dfe0b996858.png)

Market activities are also called market datasets or simply markets. Market datasets transfer the product output of one or more producing (transforming) activities to activities that consume it as an input, e.g., from hard coal at the supplier to hard coal at the consumer. The geographical boundaries of a market are chosen to reflect real-world trade conditions. For example, hard coal consumers in Australia are primarily supplied by hard coal producers in Australia, justifying an Australian market for hard coal.
Market activities account for transport and losses of the product. They further provide the average consumption mix of a product for a given region and the marginal consumption mix in the consequential system model.
Learn more about markets here.

## Construction activities
Infrastructure (i.e., capital goods) in the ecoinvent database is defined as products that have a lifetime that exceeds one year and that are not meant for consumption. This definition includes both stationary infrastructure, such as buildings, electricity or gas grids, roads, rails, mines and production facilities, and mobile infrastructure, such as machinery, tools and vehicles.

An activity producing an immobile infrastructure product often carries the term “construction” in its name. Therefore, these activities are also referred to as construction activities. The reference unit of infrastructure products in the database is most commonly “unit”, e.g., 1 unit of power plant. A construction activity usually covers the initial construction, the maintenance of the infrastructure during its lifetime, the land occupation and land transformation (if applicable) and the decommissioning for waste treatment at the end of the lifetime. The waste streams from decommissioned infrastructure leave the activity as by-product/waste outputs. The mass of the infrastructure thus leaves the construction activity with the waste streams; therefore, infrastructure products are an exception in that they do not come with properties of mass and carbon content.

Instead of mass properties, infrastructure products have properties of “lifetime” and “lifetime capacity”.

## Service activities
Service activities have inputs and outputs required to perform a service on another product, without the actual input and output of the product receiving the service. Services are therefore defined as immaterial exchanges, i.e., without a physical good changing ownership.
For example, the service of sawing with a power saw does not have an input of the tree standing in the forest. Instead, the forestry process has an input of the tree standing in the forest, an input of power sawing (in hours) and an output of the felled tree. The amount of the saw, the fuel to operate it, the lubricating oil to maintain it and the emissions released during operation enter the forestry process indirectly through the service activity.

# Operation activities
Processes with the term “operation” as part of their name represent the use of a specific infrastructure product, e.g., “mine operation” as opposed to “mine construction”. Operation datasets thus always have inputs of infrastructure. The term “operation” is used as a synonym for “use”. The term is applied to both industrial activities, e.g., “gold refinery operation”, and household activities, e.g., “operation, computer, desktop”. Operation activities may also fulfil the criteria to be a service activity.

The reference products of operation activities are not of any special type; they are normal products, such as refined gold resulting from gold refinery operation.

## Products
## Reference products
The reference product is the driver of a process. It is the product for which a change in demand will affect the production volume of the process (also known as the determining product). The reference product can be a good or a service.

## By-products/waste
By-products and waste are co-produced together with the reference product but would not justify performing a process for their own sake. For example, straw is produced together with wheat grain, which is the reference product.

In most situations, by-products can easily be distinguished from reference products. Often, by-products are similar to waste and are therefore not even fully utilised, such as straw.

Within the category of by-products/waste, waste does not have an economic value, whereas by-products do have a value on the market.

The distinction between reference products and by-products/waste is process-specific, i.e., the same product can appear as a reference product in one process and as a by-product/waste of another process.

Every intermediate exchange also carries two by-product classifications that are consistent across all the processes in which the exchange appears. These classifications determine the fate of a by-product within the rules of different system models. Every intermediate exchange is classified as either waste, recyclable or allocatable product, and every intermediate exchange is classified either as a material for treatment (mft) or not a material for treatment (non-mft).

# System Models

System models set the methodological rules to calculate the database. All system models start from the same pool of individual processes of human activities (Undefined Unit Processes (UPR)) and apply different assumptions to determine the supply (linking) and the distribution of impacts between producers and consumers of products and services (allocation and substitution).

# UPR, LCI & LCIA
## Unit Process (UPR)
The basic building blocks of the database are individual processes of human activities and their exchanges with the environment (elementary exchanges) and with the technosphere (intermediate exchanges).
![image](https://user-images.githubusercontent.com/65668613/166637440-2842315e-5e58-40dd-bb05-bd3f9cb8109f.png)

The processes in the ecoinvent database represent the average production conditions within a geographical location, rather than company-specific or site-specific conditions. For example, the ecoinvent database would contain a process for the average banana production in Ecuador, rather than for banana production at the farm of a specific fruit company. Furthermore, the contained products are primarily intermediate products rather than final consumer products. For example, the database would contain wheat flour but not pasta made from that flour.
