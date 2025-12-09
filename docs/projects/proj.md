---
title: 清华大学・鲁志实验室 科研课题 
---

# 清华大学・鲁志实验室 科研课题 

\[ [English](proj-en.md) \| **中文** \]

---

## Projects & Subgroups

我们围绕非编码 RNA（ncRNA）在两个主要的科研方向上进行探索和研究：I. 生信驱动的**精准医疗**；II. AI驱动的**核酸模型和药物设计**。

<div align="middle">
  <img src="../img/projects.webp" style="zoom:20%;" />
  <br>
</div>


### A1. **RNAfinder**

***Discoverying novel noncoding RNAs:*** 随着测序技术的进步，尤其是单细胞、单分子水平的测序技术的发展和成熟，我们有能力从更多物种、更多组织、更多细胞类型中发现新的非编码RNA。例如，我们可以从人类基因组的各类重复区域（**Transposable Elements**）、纷繁复杂的微生物群落的宏转录组（**Meta-transcriptome of Microbes**）中发现和研究不同环境和条件下的新非编码 RNA。这些研究不仅将扩大我们对生命多样性的理解，还可能揭示新的、跨物种的生物学机制。

***cell-free RNAs (cfRNAs):*** 临床血浆样本中的 cfRNA 含量很低且碎片化，需要解决测序数据信噪比低、成本昂贵等问题。我们应用模板转换、早期标记、分子标签和CRISPR-Cas9等技术，开发新型 cfRNA-seq 技术，降低构建高通量测序文库的经济成本并提高了测序数据的信噪比。

> **exRNA** (extra-cellular RNA) 在很多临床研究尤其是液体活检研究中又称为 **cfRNA** (cell free RNA) ，包括了很多**非编码 RNA** (**ncRNA**)，如 miRNA，lncRNA，srpRNA，circRNA等。

<div align="middle">
<img src="../img/exRNA-seq.jpg" style="zoom:33%;" />
<br>
<small>Different NGS (next-generation sequencing) libraries of cfRNAs</small>
</div>


***double-stranded RNA (dsRNA):*** 著名的非编码RNA有miRNA/siRNA/piRNA这三类small RNA，他们是通过双链RNA（dsRNA）加工生成的不同RNA类型。双链RNA（double stranded RNA, dsRNA）是一种由两条互补RNA链组成的分子，RNA干扰的启动通常需要双链RNA（dsRNA），这些双链RNA可以是外源（如病毒）引入的，也可以是内源（如人类基因组里的重复序列）产生的。随着科研的进展，人们发现双链RNA（dsRNA）远不止上述3种。这些不同的dsRNAs在免疫系统中具有重要作用，尤其是在抗病毒和抗肿瘤免疫反应中。比如，srpRNA就通过癌症微环境的外泌体运输发挥细胞间的调控功能。

More Reading: [**dsRNA code**](https://book.ncrnalab.org/teaching/part-v.-assignments/3.rna-regulation-dsrna)

<div align="middle">
<img src="../img/dsRNA.webp" style="zoom:50%;" />
<br>
<small>Different types of dsRNAs in immune response</small>
</div>





### A2. RNAfinder - Applications

#### A2.1 [**Medicine**] Precision Medicine

***Clinical applications:*** 我们将上述方法应用在液体活检上，助力解决临床问题，例如癌症早筛。

通过将转录组学数据与其他多组学数据整合，我们旨在从综合的、多维的水平上去解释复杂疾病的发展。 我们开发测序和生物信息学方法来研究**编码和非编码 RNA (ncRNA)** 的细胞和细胞外转录组，从单细胞水平和多分子水平研究患者各种免疫细胞内外编码和非编码基因的调控图谱。

对于复杂疾病来说，准确选择最佳的诊疗方案很重要，但也很困难。 例如，一些靶向药物已被批准用于许多复杂疾病，但不同药物的受益人群尚不清楚，需要准确的生物标志物。 因此，通过将免疫细胞数据与血浆中的cfDNA/cfRNA数据以及临床数据相结合，我们开发药效预测模型，为治疗复杂疾病的精确药物指导提供多模态标志物模型。同时，我们针对这些数据探索深度学习、迁移学习、相似性网络融合，以及其他生物信息学分析技术。

我们将上述方法应用于精准医疗，重点关注两类疾病：**1）自身免疫疾病；2）癌症**。

> “**癌症和自身免疫疾病，这两者就像硬币的两面**：若癌细胞通过某种机制逃脱了免疫系统监视、无法被清除，恶性肿瘤便开始滋长；而当正常细胞因某种原因打破了身体原本的免疫耐受机制，就可能引发自身免疫疾病。” 
> -- 反向疫苗：自身免疫病奇解《环球科学》(*Scientific American*) 2024年12月号


<div align="middle">
<img src="../img/research.webp" style="zoom:50%;" />
</div>


***Multi-modal data integration:***  我们可以由cfRNA-seq等高通量测序方法通过生物信息分析计算得到多模态数据（例如表达、剪接、编辑、融合等）。对于这些多维度、多模态的高通量数据（例如 cfRNA-seq分析得到的多模态数据，以及multi-omics数据），我们需要进行4个步骤来进行机器学习等分析，包括 1) Data Cleaning, 2) Feature extraction and engineering, 3) Model Fitting, 4) Classifier。我们针对这4个步骤开发相应的生物信息学方法、软件、数据库等工具，例如，我们探索和利用大语言模型和深度学习模型等新型AI 技术，进行多模态数据整合。

<div align="middle">
<img src="../img/multiomics.webp" style="zoom:50%;" />
<br>
<small>Multi-dimensional data for liquid biopsy of cancer (Heitzer et al., Nature Reviews 2019) </small>
</div>


---


#### A2.2 [**Ribozyme**] Structure Prediction & Ribozyme Design


<div align="middle">
  <img src="../img/rna-structure-prediction.webp" style="zoom:20%;" />
  <br>
  <small>Prediction of 2D and 3D structure of RNA</small>
</div>

**_RNA structure prediction:_** 我们开发针对 RNA结构的预测模型和算法，对 RNA 结构的准确预测，将帮助我们更好地理解 RNA 的调控和功能，并应用于基于 RNA酶和RNA疫苗的设计。例如，mRNA，以及环装RNA（circular RNA）等，可以用来做为RNA疫苗。在 RNA 疫苗设计中，RNA 结构、密码子和修饰的设计都是非常重要的研究方向。不论是 RNA干扰还是RNA疫苗，提高RNA 在存储和运输中的稳定性，递送到细胞和人体内的有效性和靶向性，都是非常重要和前沿的研究方向。


**_RNA Design:_**  不同领域的新方法和新思维的引入，往往能带来本学科的突破性进展，所以我们尤其注意将最新的计算领域的新技术和新思维（例如基于大语言模型的**新型 AI 技术**）引入到生物数据的研究上。我们针对RNA，尤其是 **非编码 RNA** (**ncRNA**），的结构、调控和靶标等问题，开发新型的核酸模型。最终，这些新型的模型将会带领我们进入一个崭新思维的**酶设计、疫苗设计和药物设计**的新时代。



---




### B1. **RNAtalk**


<div align="middle">
  <img src="../img/RNA-Talk.webp" style="zoom:20%;" />
  <br>
  <small>RNAs Talk: Language of RNA</small>
</div>


***RNA-RNA interaction (trans-pair)*** : RNA靶向RNA在各种生物过程中发挥着至关重要的作用，包括基因调控、RNA加工和病毒复制。 预测 RNA-RNA 相互作用涉及识别和表征两个 RNA 分子之间的结合位点，这可以深入了解它们的功能关系和调控机制。 值得注意的是，由于 RNA 结构的复杂性、巨大的序列空间以及经过实验验证的相互作用数据的有限性，预测 RNA-RNA 相互作用仍然是一个具有挑战性的问题。 因此，预测的准确性可能会根据所使用的具体方法和输入数据的质量而有所不同。 我们开发和完善用于预测 RNA-RNA 相互作用的计算方法，旨在提高对 RNA 生物学的理解，并促进新的治疗靶点和基于 RNA 的调控机制的发现。



---



### B2. RNAtalk - Applications

#### B2.1 **siRNA** Drug Design

**_siRNA design:_** siRNA已成为一种广泛使用的转录后调控实验方法，并且越来越显示出其作为未来靶向药物的潜力。 然而，高效siRNA的预测仍然受到数据集偏差、预测方法的不足以及脱靶效应的存在的阻碍。为了克服这些限制，我们开发新的人工智能方法来预测和设计高效的siRNA。


#### B2.2 **Small-molecule** Drug Design

**_Small molecule drug design targeting RNA:_** 可作为小分子药物靶标的人类蛋白数量非常有限：在人类的2万个左右的蛋白编码基因（占人类基因组总长度的1.5%左右）中，大约有 10%-15%与疾病直接相关；而在这些基因中，据估计仅有不到 700 个的蛋白产物是可以成药的 （仅占人类基因组总长度的 0.05%左右）。另一方面，人类基因组的~70%甚至更多都会被转录成 RNA，其中大多是**非编码 RNA** (**ncRNA**)。因此，近年开始有越来越多的研究者试图将 RNA 作为药物靶标，并初步证明了这一策略的可行性。尤其值得我们注意的是，新冠病毒就是 RNA 病毒，其基因组本身也有希望被作为药物靶标。此外，利用非编码RNA进行疾病治疗也是一个有前景的研究方向，例如，基于 siRNA 的RNA干扰（RNA interference, RNAi）系统等已经被用于开发新的基因治疗方法。由于 RNA 结构的高度复杂性和可变性，以及实验方法的限制，目前我们对于 RNA 的三维结构的了解仍非常有限，靶向 RNA 的药物研发也处在起步阶段。 我们将充分发挥人工智能的优势，利用深度学习等最新的计算技术整合多方面的信息，设计新药物靶标RNA。

<div align="middle">
  <img src="../img/drug_rna.webp" style="zoom:30%;" />
  <br>
  <small>The potential RNA-targeted druggable genome (Warner, et al., <i>Nature Reviews | Drug Discovery</i>  2018)</small>
</div>
