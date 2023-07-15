---
title: ReRAM Sequence Aligner Accelerator
date: 2023-7-14 09:52:00 +0800
categories: [Circuit Design, Speech]
tags:  [Accelerator]     # TAG names should always be lowercase
---

# Introduction:
![About me picture](../pic/genome_process.PNG)

Genomic sequence analysis has contributed significantly  to  the  ﬁelds  of  medicine  and  science,  yet  it  remains constrained  by  computational  capabilities  and  memory  band- width. The primary bottleneck in this process is the approximate string  matching  (ASM)  during  read  mapping,  which  involves handling vast amounts of data. 

Processing  in  memory  (PIM)  architecture  presents a  potential  solution  by  conducting  computations  within  the memory itself, minimizing data movement and enhancing efﬁciency. PIM architecture can manage large data volumes with high  bandwidth,  extensive  parallelism,  and  energy  efﬁciency, thereby streamlining genomic sequence analysis. 

# Motivation:
## 1. Improving  compute  parallelism:  
We propose leveraging ReRAM-based hardware
accelerators  to  achieve  higher  parallelism.
## 2. Reducing  the  average  computation  workload  through  adjustable error distance:
We suspect that the maximum error tolerance used in the Bitap algorithm may be too high for efﬁcient  read  mapping.  By  adjusting  the  maximum  error tolerance, we can potentially reduce the computation workload required for read mapping, thereby improving the efﬁciency of read mapping for large-scale genomic data sets.

# Hardware Design
![About me picture](../pic/reram_hardware.PNG)