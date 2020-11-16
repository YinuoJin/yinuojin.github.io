---
title: "Ancestral Sequence Reconstruction"
excerpt: "ASR with incorporation of structural constraints<br/><img src='/images/asr.png' width='70%'>"
collection: portfolio
---
##### Columbia University, COMS 4761 Computational Genomics S20, Final Project;
<center><img src='/images/asr.png' width="85%"></center><br><br>
In this project, my partner and I implemented multiple recently proposed algorithms for Ancestral Sequence Reconstruction (ASR), extending features to [TreeTime](https://github.com/neherlab/treetime), a phylogenetic analysis toolkit. [[PDF]](/files/asr_treetime.pdf) ⋅ [[Code]](https://github.com/YinuoJin/treetime)<br><br>
The original vanilla ASR implementation in TreeTime assumed fixed substitution rate and independent evolution process at different sites along any given sequence during the reconstruction. For marginal reconstruction, we implemented Among-site Rate Variations (ASRV) & site-specific constraints based on the inferred solvent accessibility or secondary structure for protein sequences. For joint reconstruction, we implemented the branch-and-bound algorithm proposed by Pupko <i>et al.</i> (2002), which obtains optimal reconstruction solution. The overview of the algorithms we implemented are summarized [here](https://github.com/YinuoJin/treetime/blob/master/docs/algorithms_summary.pdf) <br><br>
We tested our Python implementations of those features on both a lab generated Flurescent Protein phylogeny and multiple mitochondrial protein datasets. The method with ASRV and site-specific constraints outperformed the vanilla ASR, for either the actual accuracy or the log-likelihood scores. Currently we are trying to generalize the method with incorporation of structural constraints not limited to protein sequences (e.g. stem-loop structure in tRNA).
