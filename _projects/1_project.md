---
layout: page
title: Machine-Learning Classification to Predict the Dimensionality of Hybrid Organic-Inorganic Halide Perovskites
description:
img: assets/img/ml_cover.jpg
importance: 1
category: Research
related_publications: true
---

Low-dimensional hybrid perovskites have demonstrated remarkable performance in photovoltaic applications, primarily due to their exceptional optical and electronic properties. As the search for potential candidates for novel materials continues, understanding the structure of these materials is crucial for investigating their stability. In this study, we implement a framework to find novel material based on a machine-learning model. The machine learning model was trained to predict the dimensionality of the polyhedral network based on the connectivity of the polyhedral network in different directions. The polyhedral connectivity of low-dimensional structures can be classified into three dimensions: 0D, 1D, and 2D. This ML model was trained on 588 unique experimentally reported structures and these structures include halide perovskites as well as related, non-perovskite halometallate structures. These structures contain 65 unique B-X combinations and 315 different organic cations. The ML model achieves a precision of 96%, 87%, and 95% for 0D, 1D, and 2D, respectively for a stratified 20% test set using a graph representation from a self-supervised message passing transformer (GROVER) to represent the organic cations and a set of 7 features to represent the inorganic/halide elements. This ML model is then used to fill in the gap of the missing compounds. In total, the ML model is used to predict the dimensionality of 40556 new HOIPs based on the combination of organics, inorganic /halide combinations across different element compositions and B/X ratios. 

{% include figure.html path="assets/img/ml_pb.jpg" title="probabilitymap" class="img-fluid rounded z-depth-1" %}
The probability of each composition to get predicted as a 0D,1D,2D. probability calculated from existing structural data


Finally, to identify interesting organic cations that have not yet been examined for HOIPs, we used the GROVER representation and performed a similarity search to select potentially interesting organic cations and predict their corresponding dimensionality.
iii
We screened a set of 6 molecules to find the similarity from two different molecular cases to find novel materials. This organic cation identification is demonstrated on: chiral molecules and large conjugated systems derived from pyrene, thiophenes and cyclopentadiene molecules.
