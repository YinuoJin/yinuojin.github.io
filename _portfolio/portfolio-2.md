---
title: "Cell segmentation & Spatial profiling with multiplexed images"
excerpt: "<img src='/images/segmentation_figure.png' width="70%">"
collection: portfolio
---
##### Computational Cancer Biology Lab, Columbia University. Advisor: Prof. Elham Azizi
<center><img src='/images/spatial_profiling.png' width="75%"></center><br><br>
With recent advances in multiplexed imaging and spatial transcriptomic and pro-
teomic technologies, cell segmentation is becoming a crucial step in biomedical im-
age analysis. In recent years, Fully Convolutional Networks (FCN) have achieved
great success in nuclei segmentation in in vitro imaging. Nevertheless, it remains
challenging to perform similar tasks on in situ tissue images with more cluttered
cells of diverse shapes. To address this issue, we propose a novel transfer learning, cell segmentation framework incorporating shape-aware features in a deep learning model, with
multi-level watershed and morphological post-processing steps. Our results show
that incorporation of geometric features improves generalizability to segmenting
cells in in situ tissue images, using solely in vitro images as training data. <br><br>
Our extended abstract has been accepted to Learning Meaningful Representation of Life (LMRL) Workshop at NeurlPS 2020. The poster and presentation video is under preparation. Currently, we are investigating the potential direction of adding topological-aware priors to the segmentation, and are refining our framework to count single-molecule transcript represented by mRNA markers on the multiplexed images for further spatial profiling analysis.
