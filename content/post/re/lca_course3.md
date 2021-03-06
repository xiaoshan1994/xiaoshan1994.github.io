---
title: "Advanced Course on LCA —— Session 3: Economic Allocation"
date: 2021-08-16T16:13:31+02:00
description:
images:
- https://user-images.githubusercontent.com/65668613/129578026-ec0940d3-30b7-4b94-82b2-366cf33db933.png
thumbnailImagePosition: left
thumbnailImage: //user-images.githubusercontent.com/65668613/129578026-ec0940d3-30b7-4b94-82b2-366cf33db933.png
tags:
- CML
- Jeroen
Categories:
- Research
- Life Cycle Assessment (Training)
---

## Session 3
## Purpose

This software session focuses on reproducing the results of an LCA paper on economic allocation, defining functional flows and identifying multi functional processes, with the software program CMLCA. In today’s exercises, you will learn:

* to understand the main principles of economic allocation;
* how such analyses work in CMLCA software.

You may perform the exercise alone or together with (a) colleague(s) in a virtual room, and again, you don’t have to hand in the results.

## Data and Software

The software is CMLCA, which you already have installed on your computer.

## Exercise 3.1

Along with this exercise a copy of the paper “Guinée J.B., Heijungs R., Huppes G. (2004). Economic Allocation: Examples and Derived Decision Tree. Int. J. LCA 9 (1), 23-33” has been provided to you (see your “Reading materials”). Please read pages 23-27 (till the end of the page) of this paper.

## Exercise 3.2

Now we will reproduce the calculations made in this paper with CMLCA.
a) Open CMLCA and start new LCA project, and press OK. Press F11, select and select Scientist as user skill.

b) Implement the first allocation case described in section 3.2 (pp. 26-27) by adding/inserting the processes “primary aluminium production”, “extrusion to engine”, “use”, “collection & dismantling”, “secondary aluminium production” and “production of other semiproducts” with their data on economic (products) and environmental flows (extensions):

Note:

* When inserting the process and data for “use”, “used engine” is not a good in this example, but a “waste”.
* The reference flow is just a product out of the process “use” and is inserted into CMLCA as an economic flow with unit “yr” and value “5”.

c) The last window of this exercise of inserting process data should look like the window below:

![image](https://user-images.githubusercontent.com/65668613/129588694-04d197d5-4fc6-4c9b-867b-c206d34a8b88.png)

d) Insert the data for the reference flow (by adding "an Alternative").

e) Calculate the inventory table. Check the results with the results reported in the Guinée et al. article on p.27, just above Fig. 5. Are they the same? Press “close”. Select “Inventory analysis” from the main menu and next “Edit inventory settings”. Make sure that “Void processes” is on “Remove”! Calculate the inventory table once more. Now, you should get the following message: “Cannot invert technology matrix – rectangular matrix?” The cause of the different results is explained in the footnote1[^footnote1]. Next, analyse the causes of the reported “rectangular matrix” problem.

![image](https://user-images.githubusercontent.com/65668613/129590113-351bd341-1c02-4e81-8620-f1a85523fb7c.png)

f) Next, press the “Allocations button. Go to the tab sheet “Partitioning details” and press on the right column (“Principle”) the option “equal”. Enlarge the “Allocations” window to full screen view and stretch-up the column widths manually. Try to understand the allocation factors that then appear. Why are there different zeroes and ones for the various outputs; what is/are the functional flows (to be allocated to) and what is/are the nonfunctional flows (to be allocated)?

g) Insert the allocation factors calculated in Table 4 of the paper mentioned above, by selecting “Standard” in the right column (“Principle”) and typing the correct allocation factors for the non-functional flow (i.c. NH3) and check the “select” box. Click “Close”.

h) Go back to the main menu and select “Inventory results” and see if you can reproduce the results presented in the text on page 27 of the: “The total emissions follow from Fig. 5. For SO2 for system 1, the emission thus equals 1×10–3 kg [...]. The total emission of NH3 for system 1 thus equals 1×10–3 + 0.8×10–3 = 1.8×10–3 kg, [...].”

i) If you have time left, you could also try to perform the same economic allocation by inserting prices for the functional flows. For this go to the main screen, press “Scope definition”, and check “Prices of products” under “Financial information”. Select the currency “EUR”, press “Close”. Press “Manage items”, double-click on “Products”,
double-click on “used engine”, press “More” and insert “-100” under “Price”, and press “OK”. Now do the same for “aluminium scrap” by double-clicking on “aluminium scrap”, pressing “More” and insert “30” under “Price” and press “OK”. Close the “Manage items” window. We have now inserted the prices given in the article in Table 4 for the functional flows. Now go to “Allocations” again and select the tab sheet “Partitioning details” and select “Economic” under “Principles”, press “Close” and press “Inventory results”, and check if you get the same inventory results (tab sheet “Elementary flows”) as before.

Save the resulting file as “allocation exercise3.lca” since you will continue to work with this file later on this week.

https://leidenuniv1.sharepoint.com/sites/LCA-PR2020copy52/Class%20Materials/Exercises/LCA-PR_Software%20exercise3(online%20version).pdf

[^footnote1]: This option in CMLCA used to remove processes that were accidentally added but had no functional flow (FF). However, in ecoinvent V3 processes exist that have no functional flow but are at the same time indispensable for smooth operation of the V3 database for (difficult and also quite unclear) accounting reasons. Therefore, the option is now turned to “Keep” by default (Keep processes without FFs), but a consequence of this is that processes with no FF, such as [P6] “production of other semi-products” in the example above are kept within the system. [P6] misses a functional flow (Product) while the “collection & dismantling” process has two FFs (a product OUT and a waste IN). These are two mistakes but together they balance out, result in a square matrix that can be inverted, but produces wrong results. Keep this possibility in mind in your future case study work when you get unexpected results. However, when working with ecoinvent V3, NEVER turn the “Void processes” on remove. Again, more in general: NEVER change anything in the ecoinvent processes, also not in the allocation and cut-off details. Or in short, “don’t mess with ecoinvent”😀.
