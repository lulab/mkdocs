# Background and Methodology


\[ **English**  \|[中文](background.md) \]

---


## Background

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



***noncoding RNA (ncRNA).*** About 20 thousand protein-coding genes in human were transcribed and tranlsated from only ~1.5% of human genome sequence. On the other hand, ~70% or more of the human genome  are transcribed into RNAs. Many of them are **noncoding RNAs** (**ncRNAs**), which are not well studied yet.

“By 2020 the ENCODE project said it had identified around 37,600 noncoding genes—that is, DNA stretches with instructions for RNA molecules that do not code for proteins. That is almost twice as many as there are protein-coding genes. Other tallies vary widely, from around 18,000 to close to 96,000. … In a 2024 commentary for the journal *Science*, the duo described these findings as part of an <u>RNA revolution</u>. … they undercut the way we think our biology works. Ever since the epochal discovery about DNA’s double helix and how it encodes information, the bedrock idea of molecular biology has been that there are precisely encoded instructions that program specific molecules for particular tasks. But **ncRNAs seem to point to a fuzzier, more collective, logic to life**. It is a logic that is harder to discern and harder to understand. But if scientists can learn to live with the fuzziness, this view of life may turn out to be more complete.” ( [Revolutionary Genetics Research Shows RNA May Rule Our Genome \| *Scientific American*](https://www.scientificamerican.com/article/revolutionary-genetics-research-shows-rna-may-rule-our-genome/) 2024.7. Cover Story)



***double-stranded RNA (dsRNA).*** Three well-known types of noncoding RNA include miRNA, siRNA, and piRNA. These are distinct RNA types generated through double-stranded RNA (dsRNA) processing. Double-stranded RNA (dsRNA) is a molecule composed of two complementary RNA strands. RNA interference typically requires dsRNA, which can be introduced exogenously such as viruses (**microbes**) or produced endogenously such as repetitive sequences (**Transposable Elements**) in human genome. Advances in research have revealed that there are far more than just these three types of dsRNA. These diverse dsRNAs play important roles in the immune system, particularly in antiviral and anti-tumor immune responses. For example, srpRNAs exert intercellular regulatory functions through exosome trafficking within the cancer microenvironment.

***Microbial RNA (mbRNA).*** Research on microbial RNA has revealed that bacteria, viruses, and other microorganisms produce diverse RNA molecules that influence host health and disease. Small RNAs (sRNAs) in bacteria regulate virulence genes, stress responses, and antibiotic resistance, contributing to infections such as tuberculosis and sepsis. Viral RNAs, including microRNA-like molecules encoded by viruses such as Epstein–Barr virus, can modulate host immune pathways and promote oncogenesis in diseases like lymphoma. Advances in high-throughput sequencing (**Meta-genomics and Meta-transcriptomics**) have enabled the identification of microbial RNA signatures associated with conditions ranging from inflammatory bowel disease to cancer. Understanding these RNA-mediated mechanisms is guiding the development of RNA-based diagnostics, vaccines, and targeted antimicrobial therapies.


More Reading: [**dsRNA code**](https://book.ncrnalab.org/teaching/part-v.-assignments/3.rna-regulation-dsrna)

<div align="middle">
<img src="../img/dsRNA.webp" style="zoom:50%;" />
<br>
<small>Different types of dsRNAs in immune response</small>
</div>


***RNA regulation in immune system.*** RNAs are dynamicly regulated during transcription. In addition, after RNA is transcribed, it will also have very complex and fine post-transcriptional regulation, such as alternative splicing (AS), alternative polyadenylation (APA), degradation, editing, modification, cellular localization and so on. These are closely related to the structure of RNA itself and the proteins that recognize RNA sequence and structure. At the same time, RNAs, especially noncoding RNAs (ncRNAs), also regulate other macromolecules, thus playing important roles in innate immune response to viruses and cancer immunity. We explore these complex regulatory processes in complex diseases such as **cancer and autoimmune diseases**, which are applied to immunotherapy.


<div align="middle">
<img src="../img/RNAreg.webp" style="max-width:50%;"  />
<br>
<small>RNA Regulation: Post-transcriptional Regulation</small>
</div>



## Methods

***RNA Modeling.*** Leveraging new **AI technologies** for **RNA modeling** (i.e., RNA-Talk models) that tokenize information at **sequence** and/or **structure** levels, we discover and decipher the various molecular interactions and biological regulatory networks mediated by RNA. 


<div align="middle">
  <img src="../img/modeling.webp" style="zoom:50%;" />
  <br>
  <small>RNA Modeling</small>
</div>

***Multi-modal data integration.*** Furthermore, multiple regulation events (e.g., expression, splicing, editing, fusion) can be quantified by bioinformatic analysis from NGS data like cfRNA-seq.  For the multi-modal data, such as cfRNA-seq derived multi-view data and/or multi-omics data, we need 4 steps for machine learning analysis, including 1) Data Cleaning, 2) Feature extraction and engineering, 3) Model Fitting, 4) Classifier. We develop corresponding bioinformatics method, software, database and other tools for these four steps. For instance, we integrate these multi-modal data using new AI technologies like large language and deep learning models. 

<div align="middle">
<img src="../img/multiomics.webp" style="zoom:30%;" />
<br>
<small>Multi-dimensional data for liquid biopsy of cancer (Heitzer et al., Nature Reviews 2019) </small>
</div>


***Virtual Cells & Digital Twins:***  Even further, we can build computational models that integrate multi-omics, imaging, and clinical data to simulate cellular and physiological behaviors in silico. Virtual cell models seek to capture gene regulation, signaling, metabolism, and cell–cell interactions, enabling hypothesis testing and mechanism discovery without exhaustive wet-lab experiments. Digital twins extend this concept to patient-specific models, allowing simulations of disease progression and treatment response for precision medicine. Virtual cells and digital twins are transforming drug discovery, biomarker identification, and personalized therapeutic decision-making.

<div align="middle">
<img src="../img/AIVC-DT.jpg" style="zoom:38%;" />
<br>
<small>2024 Cell - How to build the virtual cell with artificial intelligence - Priorities and opportunities</small>
</div>