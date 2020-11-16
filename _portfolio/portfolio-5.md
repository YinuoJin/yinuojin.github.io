---
title: "Evaluating gene-gene co-operations in Pancreatic scRNA-seq data"
excerpt: "Gene co-expression network inference via Deep Learning & SHAP interactions and WGCNA<br/><img src='/images/wgcna.png' width='70%'>"
collection: portfolio
---
##### Columbia University, COMS 4995 Machine Learning for Functional Genomics F19, Final Project

<center><img src='/images/wgcna.png' width="85%"></center> <br><br>
In this project, our team investigated gene-gene dependencies from a SC-islets scRNA-seq dataset. We aimed at finding more modest cell-type specific genes which work cohesively with well-studied cell-type "housekeeping" genes and their interactions. <br><br>
We first trained a neural networks with Antoencoder (dimensional reduction with the bottleneck layer) to "fit" the cell type labels obtained by the original authors via unsupervised learning. Then we used SHAP to extract crucial features captured by the model and constructed the gene co-expression networks. To evaluate the robustness of our model, we parallelly constructed a gene co-expression networks via WGCNA, and further compared our networks, WGCNA results and well-documented, canonical gene dependency pathways. By comparison, our method captured a few novel interactions haven't been documented, while maintaining many known interactions as well.
