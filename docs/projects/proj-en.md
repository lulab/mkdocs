---
title: Research Projects @ Lu Lab
---

# Research Projects @ Lu Lab

\[ **English**  \|[中文](proj.md) \]

---

## Goals 

>  <div align="middle"><img src="../img/RNAcompute.webp" style="max-width: 50%" /> <br> [“**RNA**, not DNA, is **the computational engine of the cell.**”](https://www.scientificamerican.com/article/revolutionary-genetics-research-shows-rna-may-rule-our-genome/)  <br> <small> (Revolutionary Genetics Research Shows RNA May Rule Our Genome \| *Scientific American*, 2024.7. Cover Story) </small></div>
>

> Life sciences are undergoing a profound paradigm shift:
> From **Observational Biology** to **Programmable Biology**.
> Over the past several decades, the central mission of biology has been to identify and describe the components of living systems and their interactions. In the future, however, a more fundamental question will emerge:
> **How will a biological system respond and evolve when subjected to a defined perturbation?**
> Against this backdrop, a strategically important field is beginning to take shape:
> *RNA Perturbation Science*.
> Its central question is:
> **Given an RNA input, how will the state of a biological system change?**
> At a deeper level, what we are ultimately trying to understand is:
> **The Projection from Biological State to RNA.**
> This involves not only how RNA reflects biological states (*Sensing*), but also how RNA alters those states (*Perturbation*), ultimately enabling the prediction (*Prediction*) and control (*Control*) of living systems.
>
> The convergence of **AI × RNA × Programmable Therapeutics** is likely to become one of the most transformative frontiers in life science over the coming decade.
> RNA is particularly well suited to this era because it possesses several unique properties:
>
> * **Designable**
> * **Computable**
> * Strong **Sequence–Structure Coupling**
> * Highly compatible with **High-Throughput Experimentation**
> * Rapid **Iteration and Validation Cycles**
> * Naturally suited for **Foundation Models** and **Representation Learning**
>
> Compared with many protein-centered problems, RNA is inherently more **AI-friendly**, making it an ideal bridge between artificial intelligence and the life sciences.
>
> The scientists who will have the greatest long-term impact in the future will not merely observe biological systems; they will be those who can transform living systems into **predictable, designable, and programmable systems**.
> RNA is likely to be one of the most promising entry points toward this vision.
> Therefore, the long-term vision of our laboratory is:
> **Predictive & Programmable Biological Systems Based on RNA**
> Namely: **From Reading Biology to Programming Biology**
>
> — ChatGPT, 2026.06.01



We develop **bioinformatics** technology on **noncoding RNAs** from multiple perspectives/models of RNA structure and post-transcriptional regulation (e.g., splicing and editing); and explore its practice in the precise diagnosis and treatment of complex diseases. We utilize bioinformatics based on **new AI technologies** and **multi-omics data** to explore novel targets in the form of noncoding RNA in complex diseases such as **cancer and autoimmune diseases**, through cooperation with front-line doctors and experts.  While studying RNA regulation network, some targets can be used as biomarkers for personalized and precise diagnosis and treatment, and some targets can be used as drug targets for drug design through AI. 


<div align="middle">
<img src="../img/goals.webp" style="zoom:50%;" />
</div>


## Projects & Subgroups

We work on two major research projects centered on noncoding RNA (ncRNA): I. Bioinfo-Driven **Precision Medicine**, II. AI-Driven **RNA Modeling & Drug Design**. 

<div align="middle">
  <img src="../img/projects.webp" style="width:300px;" />
  <img src="../img/directions.webp" style="width:300px;" />
  <br>
</div>

---

[TOC]

---

### A1. RNAfinder

***Discoverying novel noncoding RNAs.*** With the advancement of sequencing technology, especially the development and maturity of sequencing technology at the single-cell and single-molecule level, we have the ability to discover new noncoding RNAs from more species, more tissues, and more cell types. For example, we can discover and study new noncoding RNAs under different environments and conditions from **Transposable Elements** of human genome, **Meta-transcriptome** of diverse microbial communities. These studies will not only expand our understanding of the diversity of life, but may also reveal new biological mechanisms cross-species.

see more in [Background](background-en.md)


### A2. RNAfinder - Applications

#### A2.1 [**Medicine**] Precision Medicine


***cell-free RNA (cfRNA).*** The cfRNA content in clinical plasma samples is very low and fragmented. Therefore, it is necessary to solve the problems of low signal-to-noise ratio and high cost of sequencing data. We apply technologies such as TSO, early barcoding, UMI, and CRISPR-Cas9 to develop novel cfRNA-seq technologies that reduce the cost of high-throughput sequencing, and improve the signal-to-noise ratio of sequencing data.

> In clinical studies like liquid biopsy, **exRNA** (extra-cellular RNA) is also called **cfRNA** (cell free RNA). Many exRNAs are **noncoding RNAs** (**ncRNAs**), like miRNA, lncRNA, srpRNA, circRN, etc. 


<div align="middle">
<img src="../img/exRNA-seq.jpg" style="zoom:33%;" />
<br>
<small>Different NGS (next-generation sequencing) libraries of cfRNAs</small>
</div>


***Clinical applications.*** By applying the above methods to liquid biopsy, we help many clinical studies like cancer screen.

By integrating transcriptomics data with other multiomics data, we aim to explain development of complex diseases based on an integrative, multi-dimensional level.  We develop sequencing and bioinformatics methods to study cellular and extracellular transcriptome of **coding and noncoding RNAs (ncRNAs)** for varous immune cells of patients at the single-cell level and multi-molecular level. 

Accurately selecting the best diagnosis and treatment plan is important but difficult for complex diseases. For instance, some targeted drugs have been approved for many complex diseases, but the which benefit groups of different drugs are not yet clear, requiring accurate biomarkers. Therefore, by combining the immune cell data m with cfDNA/cfRNA in plasma and clinical data, we develop a drug-efficacy prediction model to provide a multi-modal biomarker for a precise drug instruction in the treatment of complex diseases. Meanwhile, we explore deep learning, transfer learning, similarity network fusion and other bioinformatics analysis techniques for these data. 

We apply the above methods to precision medicine, focusing on two types of diseases:  **1) Immune-medicated diseases；2) Cancer**.

> **Cancer and autoimmune diseases are like two sides of a coin**: if cancer cells escape the immune system's surveillance through some mechanism and cannot be eliminated, malignant tumors begin to grow; and when normal cells break the body's original immune tolerance mechanism for some reason, autoimmune diseases may be caused. "  
> -- Reverse Vaccine: A Miraculous Solution to Autoimmune Diseases, *Scientific American*, 2024.12.


<div align="middle">
<img src="../img/research.webp" style="zoom:50%;" />
</div>




---


#### A2.2 [**Biology**] Synthetic Biology

**_RNA structure prediction._**  We develop structure prediction models and algorithms for RNA. The accurate prediction of RNA structure will help us better understand its regulation and function, thus improving RNA-based enzyme and vaccince design. For instance, mRNA, as well as other RNAs like circular RNA, can be used as RNA vaccines. In the design of RNA vaccines, the design of RNA structure, codons and modifications are very important research directions. Improving the stability of RNA in storage and transportation, and the effectiveness and targeting of delivery to cells and the human body are very important and cutting-edge research directions.



**_RNA Design._**  The introduction of new methods and new thinking in different fields can often lead to breakthrough progress in this discipline, so we pay special attention to introducing new technologies and new thinking in the latest computing field (such as **new AI technologies** based on large language models) into biological data. We develop novel RNA models to explore basic scientific questions such as the structure, regulation and target of RNA, especially **noncoding RNA** (**ncRNA**). Finally, these novel models will bring us a new era of **enzyme, vaccine and drug design**.

<div align="middle">
  <img src="../img/rna-structure-prediction.webp" style="zoom:20%;" />
  <br>
  <small>Prediction of 2D and 3D structure of RNA</small>
</div>


---




### B1. RNAtalk


<div align="middle">
  <img src="../img/RNA-Talk.webp" style="zoom:20%;" />
  <br>
  <small>RNAs Talk: Language of RNA</small>
</div>


***RNA-RNA interaction (trans-pair)*** (RNA targeting RNA) plays a crucial role in various biological processes, including gene regulation, RNA processing, and viral replication. Predicting RNA-RNA interactions involves identifying and characterizing the binding sites between two RNA molecules, which can provide insights into their functional relationships and regulatory mechanisms. It's important to note that predicting RNA-RNA interactions remains a challenging problem due to the complexity of RNA structures, the vast sequence space, and the limited availability of experimentally validated interaction data. Therefore, the accuracy of predictions can vary depending on the specific method used and the quality of input data. We develop and refine computational approaches for predicting RNA-RNA interactions, aiming to improve the understanding of RNA biology and facilitate the discovery of new therapeutic targets and RNA-based regulatory mechanisms.



---



### B2. RNAtalk - Applications

#### B2.1 **RNAi and AIVC**

**_siRNA prediction._** Small interfering RNA (siRNA) has become a widely used experimental approach for post-transcriptional regulation and is increasingly showing its potential as future targeted drugs. However, the prediction of highly efficient siRNAs is still hindered by dataset biases, the inadequacy of prediction methods, and the presence of off-target effects. To overcome these limitations, we develop novel AI approaches for the prediction and design of efficient siRNA.

**_RNAi screen for therapy development in AIVC._**  "One challenge in developing successful therapies is the difficulty in incorporating the full underlying genetic, molecular and cellular basis of disease during drug discovery and development. These context-specific underpinnings are not fully specified and often vary between human patients and model systems used in pre-clinical studies. By integrating biological data from various sources relevant to specific disease contexts, the **AIVC (AI Virtual Cell)** could generate an environment for testing different therapeutic interventions in silico and identify approaches for engineering cells to reverse disease phenotypes, while accounting for the effects of varying both treatments and patient profiles. By representing the overall disease phenotype specific to patient populations (rather than one specific biochemical target at a time), the AIVC can enable virtual phenotypic screens. Although in silico experiments may not always be fully accurate, by prioritizing virtual hits with higher chances of success, the AIVC can lower experimentation costs and accelerate the process." (*2024 Cell - How to build the virtual cell with artificial intelligence - Priorities and opportunities*)



<div align="middle">
<img src="../img/AIVC-screen.jpg" style="zoom:30%;" />
<br>
<small>modified from "2024 Cell - How to build the virtual cell with artificial intelligence - Priorities and opportunities"</small>
</div>




#### B2.2 **Small-molecule** Drug Design

**_Small molecule drug design targeting RNA._** The number of human proteins that can be used as small-molecule drug targets is very limited：Of the ~20 thousand protein-coding genes in human (~1.5% of human genome sequence),  about 10%-15% are directly related to diseases; among these genes, it is estimated that less than 700 protein products are druggable (only ~0.05% of human genome sequence). On the other hand, ~70% or more of the human genome  are transcribed into RNAs. Most of them are **noncoding RNAs** (**ncRNAs**). In recent years, more and more researchers have tried to use RNA as a drug target, and initially proved the feasibility of this strategy. In particular, it is worth noting that Coronavirus (COVID-19) is an RNA virus, and its genome itself is also promising as a drug target. In addition, using noncoding RNA for disease treatment is also a promising research direction, for example, siRNA-based RNA interference (RNAi) system has aleady been used to develop new gene therapy methods. Due to the high complexity and variability of RNA structure and the limitations of experimental methods, our current understanding of the three-dimensional structure of RNA is still very limited, and the development of RNA-targeting drugs is still in its infancy. We will use the latest artificial intelligence technologies such as deep learning to integrate various information,  and subsequently to design drugs targeting RNAs. 


<div align="middle">
  <img src="../img/drug_rna.webp" style="zoom:30%;" />
  <br>
  <small>The potential RNA-targeted druggable genome (Warner, et al., <i>Nature Reviews | Drug Discovery</i>  2018)</small>
</div>
  