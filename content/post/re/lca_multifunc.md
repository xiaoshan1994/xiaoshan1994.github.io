---
title: "Proper or messy allocation?--Systematic approach to identifying and solving multi-functionality in LCA"
date: 2021-08-14T11:20:07+02:00
description:
images:
- https://www.setac.org/resource/resmgr/science-corner/lca-setac-book-graphic.jpg
thumbnailImagePosition: left
thumbnailImage: //www.setac.org/resource/resmgr/science-corner/lca-setac-book-graphic.jpg
tags:
- CML
- Jeroen
Categories:
- Research
- Life Cycle Assessment (Training)
---

* Avoided burden[^bur]
![image](https://user-images.githubusercontent.com/65668613/129441605-dae3539e-cc73-4c14-ac96-33f05980a763.png)

* Most existing LCA databases today do not include multi-functional processes.
  - including ecoinvent
* MF is 'solved' by database developers by delivering only mono-functional datasets.
* Mostly, practitioners cannot change this methodological decision anymore and often don't realize that they are handling ('accepting') more MF issues than they realize.
* Consequently, most software doesn't include ways to address MF.
* While it is known as one of the most determining factors of LCA results.
  - Certainly, in the increasing number of CE and symbiosis applications of LCA
* And most published literature remains vague on MF details too.
  - Non-transparent reporting of MF; claiming to have no or just 1 MF issue while also the (pre-allocated) ecoinvent database is used for example.

## 4 steps approach

Most LCA case studies so far apply one of the solutions without properly justifying where and what exactly the multi-functionality problem is and which criteria are used for determining that.

Therefore, we developed a 4 steps approach, explicitly distinguishing these steps, aiming for more transparency in the discussion on multi-functionality approaches and solutions.

### We first need to define the problem

* Multi-functionality (MF) = the problem
* Allocation = one of the solutions
   - partitioning the inputs and outputs of unit processes among products systems.

### What is MF

* These are processes which have more than one functions.
  - "multifunctional processes"

### Definitions

Economic Allocation: Examples and Derived Decision Tree
Jeroen B. Guinde*, Reinout Heijungs and Gjah Huppes
  https://link.springer.com/content/pdf/10.1007/BF02978533.pdf

* Economic flow: a flow of goods, materials, services, energy or waste from one unit process to another, with either a positive (e.g. steel, transportation) or zero/negative (e.g. waste) economic value.
* Functional flow: any of the flows of a unit process that constitute its **goal**.
  - goods (products outflows) of a production process
  - waste inflows of a waste treatment process
  - every process needs **at least one functional flow**; even use/consumption processes (often delivering the FU/reference flow as functional flow)
  - A flow is not intrinsically a functional flow, but only with respect to a certain unit process (more specific: an outflow that is a functional flow for one unit process is a non-functional inflow for one or more other unit processes. An inflow that is a functional flow for a specific unit process is a non-functional outflow for one or more other unit processes)

* Non-functional flow: any of the flows of a unit process that are not a functional flow.
  - product inflows and waste outflows, as well as elementary inflows and outflows (natural resources and pollutants)

### Systematic approach

### Step 1: What are the good and waste flows of every process?

* To distinguish products from wastes, any criterion can be used if it supports determining which flows constitute the goal of a process and can be applied consistently for all processes.
* Basically, all LCA practitioners use **economic value** for this:
  - Good/product (G) is a flow with an economic value >= 0;
  - Waste is a flow with an economic value < 0.

### Step 2: What are the functional flows of every process?

* The functional flow(s) of each process are either products that are produced by a process or wastes that are treated by a process (others see above).
![image](https://user-images.githubusercontent.com/65668613/129449532-969f5896-3b33-4889-980f-5885a3fa8119.png)

### Step 3: which processes are multi-functional processes?

![image](https://user-images.githubusercontent.com/65668613/129450035-fd395f20-dbe4-4b97-843d-511344cb3c30.png)

### Step 4: How to resolve the problems related to that?

[^bur]: An approach used in life-cycle assessment (LCA), especially in the context of allocating environmental burden in the presence of recycling or reuse. When determining the overall environmental impact of a product, the product is given "credit" for the potential recycled material included. For instance, PET bottles may be given environmental credit for the PET they contain, as this material will eventually be recycled back into further PET products.[1] This credit is termed "avoided burden" because it refers to the impact of virgin material production that is avoided by the use of recycled material.
