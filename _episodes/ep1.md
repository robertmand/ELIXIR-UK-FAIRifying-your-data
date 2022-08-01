---
title: What is FAIR?
teaching: 40
exercise: 20
questions:
- What is FAIR? What is the origin of the FAIR movement?
- Why is FAIR important?
- What is the difference between FAIRness and FAIRification of data?
objectives:
- Understand FAIR background and main concepts
keypoints:
- FAIR stands for Findable, Accessible, Interoperable and Reusable
- What is meant by FAIRness and FAIRification of data?
- FAIR principles were gradually formed by different sources
- Most data can be FAIRified 
- Metadata is key component in the process of FAIRification
---


The FAIR principles were created to help researchers share, reuse, and manage their data.  A common layperson's interpretation of FAIR data is a dataset that can be:
- discovered and downloaded by others; and
- interpreted correctly through the provision of detailed descriptions about the data.

Descriptions of data (metadata) enables appropriate reuse, and similar to other aspects of published research, such as drawing plots in papers, where titles and notes are given as well as descriptions of axes where data are plotted.  It's important to note that the provision of metadata is key to FAIR.
![metadata](../fig/fairifying1.png)

Note that FAIR is not limited to the Life Sciences and spans across all research disciplines. The FAIR principles are also not limited to data, but can be applied to the sharing and reuse of software and data workflow. 

## So, what is FAIR?

FAIR is an acronym summarising the 4 principles of data being: **F**indable, **A**ccessible, **I**nteroperable and **R**esuable.

![FAIR principles https://www.scibite.com/solutions/enterprise-fair-data-mdm/](../fig/fairifying2.png)

To apply FAIR to your data (and metadata), each principle includes a subset of specific requirements that can be used as a checklist.  Note, we put these into context later in this course when we take real datasets through FAIRification.  This checklist is given in **BOX 2** of  Nature 2016 publication [FAIR Guiding Principles for scientific data management and stewardship](https://doi.org/10.1038/sdata.2016.18)


![metadata](../fig/FAIRchecklist01.png)

> ## Further watching, RDMbites on FAIR:
> The powerpoint will be converted to video, please add your comments directly in the powerpoint. Your name will be added as a reviewer
> - [F in FAIR](https://docs.google.com/presentation/d/1RwEVZC390wtxPQM-zQsBDT7IbNVq0wpZ/edit#slide=id.p2)
> - [A in FAIR](https://docs.google.com/presentation/d/1RwEVZC390wtxPQM-zQsBDT7IbNVq0wpZ/edit#slide=id.p2)
> - [I in FAIR](https://docs.google.com/presentation/d/1Ac0qF1IKIVH2kjGmXFbyH0WAqI2vXqUB/edit#slide=id.p1)
> - [R in FAIR](https://docs.google.com/presentation/d/1uMyUGVH6mm48iDm6jNoBnAuqF3sGiTeO/edit?usp=sharing&ouid=115915105600833888129&rtpof=true&sd=true)
> 
{: .callout}

## What is meant by FAIRness and FAIRification of data?

FAIRfication is the process of making your data FAIR.  Since giving a unique identifier to your data is part of the first **Findability** principle, by doing so you are performing part of the FAIRification process.

FAIRness refers to the extent to which your data follows FAIR principles.  A FAIR checklist can be used to achieve this by simply counting the number principles you can attribute to your data.  Data communities often have their own guidelines and interpretations of FAIRification of data.  This is discussed later and includes an example of the [GO-FAIR](https://www.go-fair.org/fair-principles/fairification-process/) initiative that provides a fairification workflow.

> ## Further reading
> - FAIR guiding principles, [FAIRification workflow and examples](https://www.go-fair.org/fair-principles)
> - [FAIRification recipes in FAIRcookbook](https://faircookbook.elixir-europe.org/content/home.html)
{: .callout}

## The benefits of FAIR

FAIRification of your data enables reuse by yourself and others.  When grant writing, funders now commonly require a justification of why new data are being generated as part of a study, compared to reusing publically available data at no cost.

Additionally, FAIRification allows **machine readability** of you data, enabling time efficient analysis. Machine readability often refers to how data can be discovered and downloaded within a script.  A script **one-liner** can be used to download a public dataset ready for analysis, compared to a lengthier process of downloading a dataset via a webpage and then moving this into the relevant analysis folder.  Machine readability also ensures that web search engines can find your data, thereby increasing its discoverability. 

A European Commission report in 2018 (https://op.europa.eu/en/publication-detail/-/publication/d375368c-1a0a-11e9-8d04-01aa75ed71a1/language-en), considers the detrimental effects of not complying with FAIR principles and details the negative impact on research activities, collaboration, and innovation (NEED LINK).  Additionally, an EMBL-EBI report in 2020 (https://op.europa.eu/en/publication-detail/-/publication/d375368c-1a0a-11e9-8d04-01aa75ed71a1/language-en) shows how data sharing enabled the excelleration of COVID-19 research to meet the challenges of the pandemic.

> ## Further watching, RDMbites on costs of not FAIRifying your data
> [Powerpoint link of the RDMbites](https://docs.google.com/presentation/d/1xywEzC84RMor46moZVC-H-o3rJqEYYk1/edit#slide=id.p1)
{: .callout}

> ## Further reading
> In this research paper, the authors assessed the [cost/benefit relationship of the FAIRification process](https://doi.org/10.1162/dint_a_00109)
> Ebtisam Alharbi, Rigina Skeva, Nick Juty, Caroline Jay, Carole Goble; Exploring the Current Practices, Costs and Benefits of FAIR Implementation in Pharmaceutical > Research and Development: A Qualitative Interview Study. Data Intelligence 2021; 3 (4): 507–527. doi: 10.1162/dint_a_00109
{: .keypoints}


## The misunderstandings of FAIR

![FAIR data do not have to be open](../fig/fairifying4.png)

The FAIR community use the phrase **“open as possible, closed as necessary”**, though **FAIR** data and **Open** data are different. As mentioned in the [Open Data handbook](http://opendatahandbook.org/guide/en/what-is-open-data/), open data is "data that can be freely used, reused and redistributed by anyone", which can be rejected by researchers where they have sensitive data or data subject to intellectual property.  Note though that in most cases, people following FAIR principles will be looking to share their data openly.  Sensitive data can be released through anonymisation and in many cases, sharing of sensitive data is subject to controlled access.  The FAIR Principles permit this by asking the owner of the data to define the methods by which controlled access operates and processes whereby data access could be requested.  

> ## Further watching
> <iframe width="560" height="315" src="https://www.youtube.com/embed/mVCDkhxxUgg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; 
> clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
> 
{: .keypoints}

> ## Further reading
>
> - https://www.go-fair.org/fair-principles/
> - https://faircookbook.elixir-europe.org/content/home.html
> - https://www.nature.com/articles/sdata201618
> 
{: .callout}
___
## Where does FAIR come from?
### The history of FAIR
A good overview of the origins of FAIR are given on page 11 of the 2018 "Turning FAIR data into reality: interim report" from the European Commission Expert Group on FAIR data (https://zenodo.org/record/1285272#.YshNncHMIqs).  The term FAIR originates from a 2014 FORCE11 Working Group, and in 2016 a Nature aricle was published with a specific focus on scientific data mangement and steweardship.  https://doi.org/10.1038/sdata.2016.18
The mention of FAIR data now appears routinely in the Life Sciences, including funder and gouverment literature .https://www.gov.uk/government/publications/open-research-data-task-force-final-report

### What data can be FAIRified?

Any data that can be shared and described by metdata, can be FAIRyfied. The ultimate goal of FAIR principles is that humans and machines can share and discover data efficiently and safely. Any data from tools, workflows or algorithms in the form of files or data objects, can be FAIRyfied.

> ## Further reading
> For more info about origins of FAIR see this (link)[https://zenodo.org/record/1285272#.Yp9oQHbMKUk]
> For further information about selecting your data, services and repositories for FAIRification see this (link)[https://zenodo.org/record/6345114#.YqDAsXbMKUk]
{: .callout}
___





