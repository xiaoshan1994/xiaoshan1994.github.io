---
title: Waste is not a service
date: 2021-08-08T11:03:30+02:00
description:
images:
- https://1businessworld.com/wp-content/uploads/2020/06/17/Screen-Shot-2020-06-17-at-4.55.08-PM.png
thumbnailImagePosition: left
thumbnailImage: //1businessworld.com/wp-content/uploads/2020/06/17/Screen-Shot-2020-06-17-at-4.55.08-PM.png
tags:
- CML
- Jeroen
Categories:
- Research
- Life Cycle Assessment (Training)
---

https://link.springer.com/content/pdf/10.1007/s11367-021-01955-5.pdf

Almost every overview of LCA gives a graphical indication of the idea of a life cycle. Such diagrams consist of a linear sequence or network of blocks, connected with arrows, representing the major life stages of a product life cycle. Examples from recent textbooks on LCA can be found in Klöpffer and Grahl (2014, p. 2), Jolliet et al. (2016, p. 36), and Hauschild et al. (2018, p. 120). **All such flow diagrams agree on the basic setup of a chronological order: resource becomes products, products are used, and it all ends with disposal of waste**.

Yet, some of the databases for LCA tell a different story. In this paper, we focus on the ecoinvent database, a popular source of LCI data. We do not rule out that our analysis is also applicable to some other databases, but we did not analyse these.

In the methodology report for ecoinvent v2 (Frischknecht et al. 2004), it is stated that **waste disposal processes “deliver the service of waste treatment.”** Practically, this means that there is not a flow of waste from a waste generating process to a disposal process (Fig. 1a), but a flow of the service of waste treatment from a disposal process to a waste generating process (Fig. 1b). In the current version of ecoinvent (v3), this setup has been maintained, with one modification: the reference product of a disposal activity delivers a negative amount of “material for treatment” (Weidema et al. 2013). Probably, a main reason for this change in ecoinvent version 3 was to solve the flawed mass balance of the waste producing activity (i.e., the use process in Fig. 1a). Indeed, if we check the data, we see that **these processes have the name of a disposal activity, but the reference product has the name of the waste**, not of the service. For instance, the unit process “direct disposal of wastewater from textile production” has a negative input flow of “wastewater from textile production”. This setup is sketched in Fig. 1c.

{{< figure src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs11367-021-01955-5/MediaObjects/11367_2021_1955_Fig1_HTML.png?as=webp" width="800" height="600" caption="(a)The traditional textbook view of the production-use-disposal sequence; (b) the way it is implemented in ecoinvent v2, with a disposal process delivering a waste treatment service (WTS); (c) the way it has been implemented in ecoinvent v3 delivering a WTS but expressed as physical waste flow" >}}

So, it appears that there are at least three ways to model waste flows and disposal processes in LCA and that the conventions used for naming and indicating the sign do matter. The setup of ecoinvent v2 (Fig. 1b) is deviating from the textbook structure of a chronological account and it suffers from mass balance deficits, but it is at least unambiguous. **We argue that the setup of ecoinvent v3 (Fig. 1c) is ambiguous and confusing**.

Weidema et al. (2013) remark that “it does not matter whether a waste supplying activity records its waste as a physical output or as a negative physical input from a waste treatment service.” That may be true for a computer, but it is conditional on the provision that the LCA practitioner has well understood the conventions. In our experience with teaching LCA, the setup of Fig. 1c is highly confusing. Imagine a student modelling a system which produces 1 kg of a waste flow. Upon searching ecoinvent v3, he or she finds a suitable disposal process. But then, the student should take care to change the 1 kg waste into − 1 kg waste, because the waste is in fact not waste but a waste treatment service, even though it bears the name of a waste.

We argue that the logic of Fig. 1a is in many respects preferable:

* It is consistent with the overall idea of a flow diagram as a chronological overview.

* It puts the emphasis on the primarily physical character of LCA, in which material flows are the backbone.

* It allows for a more straightforward connection to chemical process models and software, such as Aspen Plus.

* It allows for an easier check of mass balances.

* It emphasizes the fact that upon a change in markets or technologies, wastes can become by-products or even co-products, necessitating the treatment as multioutput processes (it would be illogical that they would then suddenly “flip direction”).

* It allows for procedures consistently identifying and solving multifunctional processes, including open-loop recycling.Footnote1

One can wonder why ecoinvent v2 and ecoinvent v3 have chosen to use the formats of Fig. 1b and c and not the much more logical textbook format of Fig. 1a. The reason is that according to Weidema et al. (2013), **every unit process must have at least one reference product as an output**. And even stronger, if the process “has only one product output, this is the reference product.” The principles of ecoinvent v3 have been further elaborated by Weidema (2018). The consistency problems that are discussed in that paper in fact arise from an attempt to distinguish production processes and disposal processes and then to tweak disposal processes in a production format.

Suppose we have a waste disposal process which transforms a used exhaust air valve as used in a housing wall into its material constituents iron and PVC through some disassembling process. Neglecting energy requirements and emissions, the main flows are depicted in Fig. 2a: The used valve enters the process, and iron and PVC waste leave the process. Clearly, the purpose of the process is disassembling an input used valve. But following Weidema et al. (2013), the purpose of a process must be an output. Therefore, ecoinvent turns reality upside down, and reports used valve waste as a negative output and iron and PVC as negative inputs (Fig. 2b).

{{< figure src="https://media.springernature.com/full/springer-static/image/art%3A10.1007%2Fs11367-021-01955-5/MediaObjects/11367_2021_1955_Fig2_HTML.png?as=webp" width="800" height="600" caption="(a) The traditional textbook view of a particular disposal process that transforms a waste into materials; (b) the way this process is implemented in ecoinvent v3" >}}

The confusing practice to turn a waste output into a negative waste input is thus caused by the commandment that every process has at least one reference product at the output side. While we agree with the idea that every process has at least one reference product (otherwise, we would stop running the process), we do not agree with the idea that this reference product is necessarily an output. Figure 2a presents a clear example of a process for which every chemist, every process engineer, as well as everyone who has studied the textbooks by Klöpffer and Grahl (2014), Jolliet et al. (2016) and Hauschild et al. (2018) will choose the physical chronology as the correct representation. Figure 2b will be rejected by such persons as unnatural and counterintuitive.

There is one important attribute required to implement a more physical, natural, way of considering disposal activities and waste. **That is the distinction between goods and wastes, which then automatically leads to the identification of functional and non-functional flows**.

In our 2004 article on allocation (Guinée et al. 2004), we developed a procedure based on prices to distinguish wastes from goods. Instead of the “reference product,” we proposed the concept of “functional flow” (FF). The FF represents the key function (or functions) of that process or activity. The key function of a process can be to produce a certain good or service, in which case the FF is a good flowing OUT. But the function can also be to treat a waste flow in which case the FF is a waste flowing IN. Next, we argued that a multifunctional process is defined as a process having more than one FF. In this way multifunctional processes can be identified consistently and in a reproducible and unambiguous way and then be solved by one of the solutions available in literature (either system expansion, substitution or partitioning depending on the goal of the study). We translated these concepts and definitions in a 4-step approach that was recently published as a chapter in the LCA Compendium – Life cycle inventory analysis for consistently identifying and solving multifunctional processes (Guinée et al. 2018); see also video uploaded as Supporting Information. Notice that our approach subdivides the intermediate flows into functional flows and non-functional flows, but that we do not differentiate processes into production, disposal, or recycling. A process is just an activity that converts a bundle of input flows (some of which may be functional flows) into a bundle of output flows (some of which may be functional flows).

We conclude by urging ecoinvent and other database developers who adopted the same principles as ecoinvent, to repair this specific database characteristic, to allow for a distinction between goods and wastes in their databases, to open up pre-allocated database versions, and thus to allow practitioners to change database choices and solve inconsistencies between background and foreground processes regarding multifunctionality solutions. For the increasing number of LCAs on circular economy, symbiosis, and carbon capture and utilization (CCU) systems to become more reliable and credible, it is paramount to adopt consistent and reproducible approaches to identify and solve multifunctionality. Moreover, it will allow for a better representation of the actual physical direction of waste flows while avoiding confusion through minus signs: waste flows are not a service.

**Notes：In ecoinvent, recycling processes are also modelled as service processes with no outflow of recycled matter that can be connected to a process using that recycled matter. As a consequence, recycling as modelled in ecoinvent may not save any primary matter**.

This paper points out that it is unreasonable for the disposal process, acting as a service, to produce a negative output in the flow diagram of a life cycle in the current version of ecoinvent. The author suggests a logical, natural way to depict the waste rather than the goods as the output of a disposal process.
