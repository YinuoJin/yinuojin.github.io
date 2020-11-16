---
title: "PICASSO: Copy Number Inference from single-cell transcriptomics"
excerpt: "Phylogenetic Inference from Copy Number Variations (CNVs) in scRNA-seq data<br/><img src='/images/picasso.png' width="70%">"
collection: portfolio
---
##### Computational Biology Lab, Columbia University. Advisor: Prof. Itsik, Pe'er
<center><img src='/images/picasso.png' width="75%"></center><br><br>
We propose PICASSO (<b>P</b>hylogenetic <b>I</b>nference from <b>C</b>opy Number <b>A</b>lterations in <b>S</b>crna<b>S</b>eq <b>O</b>bservations), a novel iterative approach to infer subclonal structure from tumor scRNA-seq data based on CNV predictions. In each iteration, our model consists of two sections:
- Copy number profile prediction and refinement for each cell $i$, gene $g$ in the observation matrix with HMM
- Subclonal detection & phylogenetic analysis from breakpoints of the inferred CNVs with EM-clustering

The major novel features of our approach are the incorporation of cell types and the top-down clustering approach to learn the tumor phylogeny. Our model assumes differential gene expressions due to distinct cell types, which affect the CNV inference. For subclonal structure detection and intratumor heterogeneity analysis, we rely on the iterative, top-down EM-clustering instead of the conventional Hierarchical Clustering.<br> <br>

Besides the model itself, I designed a fully automated simulation pipeline facilitated by [Splatter](https://github.com/Oshlack/splatter), creating large-scale, synthetic observation matrices from the real scRNA-seq data. In each individual simulation, the pipeline generates a randomized binary tree representing the tumor phylogeny, and two scRNA-seq observations: a diploid reference matrix and a matrix containing multiple copy number alteration regions (both consist of multiple cell types). This greatly helps to benchmark the performance of our model and competing methods.
