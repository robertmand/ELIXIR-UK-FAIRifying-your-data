---
title: Example of FAIRification, Using a public repository
teaching: 40
exercises: 10
questions:
- Making an RNAseq dataset FAIR

objectives:
- Show a real example of data FAIRification through submitting data to a public repository
- Show how community standards are used to curate metadata
keypoints:
- Ten FAIR principles are applicable to a broad types of data, software and most training material.
- Applying FAIR to the training material will optimise the reuse of data, increase visibility of research and add to > saving of time and money
---

## FAIRification of a RNAseq dataset

[RNA sequencing](https://en.wikipedia.org/wiki/RNA-Seq) is chosen here as an example of how to FAIRify data for a popular assay in the Life Sciences. RNAseq data can be shared and curated in designated public repositories using established ontologies for describing protocols and biological material.

FAIRification of RNAseq data can be best achieved through submitting your data to one of the 2 international repositories. 
> - ArrayExpress: [how to submit your data](https://www.youtube.com/watch?v=ANr2PTVy7JA)
> - (GEO database)[https://www.ncbi.nlm.nih.gov/gds]

By submitting data to public repository, it is becomes openly accessible, searchable and annotated with rich metadata.  Note, both repositories belong to the (FAIRsharing database registry)[https://fairsharing.org/search?fairsharingRegistry=Database] which can help you find public repositories for all types of Life Science data.

This lesson will take you through a publicly available RNAseq dataset in ArrayExpress and show you how it meets FAIR principles using the checklist published in Nature (https://www.nature.com/articles/sdata201618) 


## Describing the data and metadata for an RNAseq dataset

We will use the following human RNAseq dataset for this practical: [E-MTAB-8316](https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316).  This hosts all metadata and links to downloadable raw and transformed data.

![The data and metadata for an RNAseq dataset](../fig/rnaseq1.png)


## Fairification: finding and accessing an RNAseq dataset

In this section, the following FAIR Guiding Princples are discussed:
- **(F1) (Meta)data are assigned a globally unique and persistent identifier**
- **(F4) (Meta)data are registered or indexed in a searchable resource**
- **(A1) (Meta)data are retrievable by their identifier using a standardised communications protocol**
- **(A1.1) The protocol is open, free, and universally implementable**

> ## Exercise
> The RNAseq dataset we are using has been published in Nature Medicine, [Link](https://doi.org/10.1038/s41591-020-0939-8).  By searching this publication, can you find the globally unique and persistent identifier for the RNAseq data and data descriptions (metadata)?
> **(F1) (Meta)data are assigned a globally unique and persistent identifier**
>[Link](https://doi.org/10.1038/s41591-020-0939-8)
{: .challenge}

> ## Solution
> Under the heading “Data and code availability” I am told the following.
> 
> ![Photo from paper https://www.nature.com/articles/s41591-020-0939-8](../fig/rnaseq2.png)
> 
> Note, that the dataset's unique and persistent (unchanging) identifier is E-MTAB-8316, and could also be expressed as the full URL
> [https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316](https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316)
> Note that there are 2 other identifiers given, which refer to 2 other single cell RNAseq datasets.  For the purpose of this lesson, we are only considering the bulk RNAseq dataset.
{: .solution}

> ## Exercise
> Here we will use a URL to access this dataset.  This URL is a concatenation of the URL of the data repository and the unique identifier: [https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316] 
> **(A1) (Meta)data are retrievable by their identifier using a standardised communications protocol**
> **(A1.1) The protocol is open, free, and universally implementable** **
{: .challenge}

> ## Solution
> You should see the following webpage hosted at the EBI(www.ebi.ac.uk).  In the context of FAIR, this means you have now accessed this RNAseq data using a weblink employing the https protocol. Note that https is a standardised communications protocol, or "way of getting data from somewhere else onto my laptop", that is open, free and universally implementable.
> ![Photo from paper https://www.nature.com/articles/s41591-020-0939-8](../fig/rnaseq5.png)
{: .solution}

> ## Exercise
> Alternatively, use the search box in ArrayExpress to find the same dataset.  Use the following link to (access ArrayExpress)[https://www.ebi.ac.uk/biostudies/arrayexpress/studies/] and then type **E-MTAB-8316** into the search bar.
> **(F4) (Meta)data are registered or indexed in a searchable resource**
{: .challenge}

> ## Solution:
> Note here that data access is gained through searching the database, and not via a direct URL.  In the context of FAIR, this RNAseq dataset is indexed in a searchable resource **(F4)**.  
> ![](../fig/rnaseq3.png)
>
{: .solution}

> ## Exercise
> Alternatively, use the same search menu in ArrayExpress to search again for the same dataset using the words “macrophage rheumatoid arthritis” in combination with selecting “rna-seq of coding rna” on the left-hand search bar.
> **(F4) (Meta)data are registered or indexed in a searchable resource**
{: .challenge}

> ## Solution:
> Here, the dataset we are using is not the first in the list, but appears in later in the search results.  Note that data access
> is gained this time through searching metadata (data about the experiment), and not the ID directly.**(F4)**.  
> ![](../fig/rnaseq4.png)
{: .solution}

## Fairification: learning about the experiment and dataset from reading the metadata

In this section, the following FAIR Guiding Princples are discussed:
- **(F1) (Meta)data are assigned a globally unique and persistent identifier**
- **(F2) Data are described with rich metadata**
- **(F3) Metadata clearly and explicitly include the identifier of the data they describe**


> ## Exercise:
> Start looking at the dataset webpage.  Try to find the unique, persistent identifier in the record:
> (https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316)
> **(F1) (Meta)data are assigned a globally unique and persistent identifier**
{: .challenge}

> ## Answer:
> THe persistent identifier is circled in red, and the first thing in the record. **(F1)**.  All metadata (descriptions about the data) and the actual raw data files are linked from this page.  Here metadata clearly and explicitly include the identifier of the data they describe **(F3)**.  
> ![](../fig/rnaseq5.png)
> 
> Here data are described with rich metadata **(F2)**, which allows a person to reuse data appropriately by reducing ambiguity around what the data mean or how they are derived. 
{: .solution}

Note that rich metadata enable people to search for datasets of interest, since all metadata are indexed and made searchable by ArrayExpress.
Metadata are added by the person submitting the data and is further curated by the ArrayExpress curation team.  Metadata curation is performed via a web-based submission interface, which aids rich curation.  Rich metadata curation makes use of existing ontologies and controlled vocabularies, which is discussed in the next section.

> ## Exercise:
> (https://www.ebi.ac.uk/biostudies/ArrayExpress/studies/E-MTAB-8316)
> familiarise yourself with the page layout.  Noting there are links to all protocols, data, sample metadata and assay type.
> How many samples are in this dataset?
{: .challenge}

> ## Answer:
> 12 (assay count)
> ![](../fig/rnaseq6.png)
{: .solution}

> ## Exercise
> What data provenance can you find? i.e. what processes have been performed to create the data linked from this page?
{: .challenge}

> ## Answer:
> The final 2 protocols detail all data transformations for the raw and transformed data.
> ![](../fig/rnaseq7.png)
{: .solution}


## Fairification: metadata and community standards

In this section, the following FAIR Guiding Princples are discussed:
- **(I1) (Meta)data use a formal, accessible, shared, and broadly applicable language for knowledge representation.**
- **(I2) (Meta)data use vocabularies that follow FAIR principles.**
- **(R1) (Meta)data are richly described with a plurality of accurate and relevant attributes. **
- **(R1.3) (Meta)data meet domain-relevant community standards.**

We have mentioned ontologies in the previous section.  In its simplest form, an ontology can be viewed as a dictionary of terms you can use to annotate a piece of data.  For example, the NCBI taxonomy database is probably something you have used and can be viewed as a collection of organism names you can use to annotate species within a dataset.  An ontology, though, will also define relationships between terms.  So in the taxonomy example, the term “Homo sapiens” will belong to parent terms such as  Primate, Mammal and so on.  Importantly, by using an ontology you can ensure you are using interoperable and searchable terms with your data.

Published ontologies are linked from the ArrayExpress data submission tool, so this work is done for you.  ALthough, if you wish to start using ontologies to annotate your data at the point it is produced, the [FAIRsharing Standards registry] (https://fairsharing.org/search?fairsharingRegistry=Standard)  is a place to start.  Importantly, when an ontology is published it itself becomes findable and reusable in the context of the FAIR principals **(I2) (Meta)data use vocabularies that follow FAIR principles.**.

Metadata using published ontologies permit interoperability since you can match identical annotations across data and databases **(I1 & I2)**, and be understood by communities of practice **(R1, R1.3)**.


> ## Exercise
> Look at the page again. Identify any metadata that originated from an existing, published ontology.   Note, we have mentioned one already: “Homo sapiens” as part of 
> (taxonomy)[https://www.ncbi.nlm.nih.gov/taxonomy].
{: .challenge}

> ## Answer
> There's a lot.  There are more metadata annotations than there are free text. There are obvious ontologies under Source Characteristics such as “Developmental stage”, Disease, Organism part, cell type... etc. These ontologies are curated at the time of data submission and depend on the type of data.
> 
> ![](../fig/rnaseq9.png)
> 
> There are also others that are not so obvious.  Under “Protocols”, a protocol ontology is used under the column” type” as well as a hardware ontology under 
> “Hardware”.  By selecting the blue > node-and-edge icon next to the protocol type, you are taken to the 
> (Expertimental factor ontology)[https://www.ebi.ac.uk/ols/ontologies/efo] at the EBI.
> >
> ![](../fig/rnaseq8.png)
>
{: .solution}


## Fairification: data provenance and licensing


In this section, the following FAIR Guiding Princples are discussed:
- **(R1) (Meta)data are richly described with a plurality of accurate and relevant attributes. **
- **(R1.1) (Meta)data are released with a clear and accessible data usage license.**
- **(R1.2) (Meta)data are associated with detailed provenance.**

Data provenance refers to information explaining how and why a piece of data is produced.  Commonly, metadata provenance is used to verify the origin of a piece of information or data.  Data Licensing refers to how a third party can use data.

> ## Exercise:
> Search for and locate the licensing options for (arrayexpress)[https://www.ebi.ac.uk/arrayexpress/]
> {: .source}
{: .challenge}

> ## Answer:
> Go to the bottom of the page, select Licensing and it gets you to [here](https://www.ebi.ac.uk/licencing). You will notice that EBI uses the CC0 licence. 
> In our RDMbites about R in FAIR, we explained what are different types of copyright licences. Creative Commons is the most widely used and widely available free licencing model. There are four components to the licence that are arranged to give six licence options.
> For more detailed explanation, check (this link)[https://pitt.libguides.com/copyright/licenses]
> {: .source}
{: .solution}


> ## Exercise:
> What provenance can you find on this page?  Note you are looking for information about where data came from.
> {: .source}
{: .challenge}

> ## Answer:
> There are a couple of examples worth mentioning. Submitters name and option to submit ORCID ID, and protocols  describing the data and how it was produces. You 
> will also notice the name of university where the data where produced.  **THIS PROBABLY NEEDS MORE EXAMPLES OF WHERE WE CAN FIND provencace, e.,g in the protocols ... the data transformations**
> ![](../fig/prov.png)
> {: .source}
{: .solution}

## Fairification: downloading raw data for reuse

One of the benefits of FAIR is that it makes your data resuable. Here all items on the checklist we are using are relevant.

For instance, in this dataset, Metadata can be downloaded from the MAGETAB link. Data can be downloaded from the ENA **(I3)**. The data and metadata are accurately described **(R)**. There is accession number at the top of the page that any person can use to easily retrieve the data **(A1)**
![](../fig/rrnaseq.png)

Even when raw data is not available, these data nonetheless adhere to FAIR principles, specifically **A2** metadata is accessible, even when the data is no longer available. 


## Test your knowledge

> ## Exercise:
> Have a look at another RNAseq dataset in the other public repository, GEO.  How is the dataset aligned with the FAIR principles? [GSE207314](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE207314).
> 
{. :challenge}

> ## Answer:
> - F: the dataset is assigned a unique ID, the data are described with rich metadata, both data and metadata are indexed in public database (GEO database)
> - A: The dataset is accessible by a standardized communication protocol (https), but also programmatically through the SRA-Toolkit (https://hpc.nih.gov/apps/sratoolkit.html)
> - I: metadata makes use of published ontologies
> - R: There is a clear description of data usage licence and for each sample there is detailed description of protocols and provenance.
> 
{. :solution}

___
