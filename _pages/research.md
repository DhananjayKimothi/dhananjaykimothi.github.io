---
title: "My - Research"
layout: textlay
excerpt: "My -- Research"
sitemap: false
permalink: /research/
---

# Research

Alignment based techniques dominate sequence (DNA, protein) comparison in bioinformatics, but the inability of these techniques to produce desirable results when sequences are divergent but functionally similar, and the quadratic complexity of the algorithms, has motivated researchers to work on alternative ‘alignment-free’ approaches. One of the more common ideas in this direction is to use a bag-of- words based approach, a representation based on a vector of <em>kmer</em> (sub sequences) counts. Such vectors are easy to compute but are of very high dimension, sometimes even larger than the sequence itself. The other noted criticism of bag-of- word based approaches is their limited capability of incorporating contextual information, which can otherwise be very useful. A step forward in this direction is to develop approaches which map sequences in a low dimensional vector space, while keeping the biological relations intact (i.e. functionally similar sequences are mapped closer together in the vector space than others). Recent developments in representation learning research (specifically in NLP) have opened the possibility to explore similar techniques for biological sequences. Such techniques offer advantages in terms of their capability to include contextual information while computing low dimensional representations. An additional advantage of these techniques is the possibility to include prior knowledge (such as class information), ​which is sometimes not explicitly evident in sequences, for example, apparently divergent sequences may belong to the same class. Furthermore, employing such information rich representations, as an input to machine learning algorithms, improves their performance when applied to solve a given task. Summary of some of the works is given below:


<p style="color:#FF5733"> Learning distributed representation for biological sequence analysis </p>
<hr style="margin-top:-0.5em; height:2px;border-width:0;color:Yellow;background-color:black">
Keywords: Representation Learning, Alignment free methods, Classification

Biological sequences are an array of alphabets and hence are not in the desirable form to be used directly with machine learning algorithms. Thus, it is essential to develop efficient approaches to generate the vector embeddings that may capture biological information directly from the sequences. In this project, we develop a word-embedding based representation learning framework, Seq2Vec, that can be trained to generate the embeddings for any given biological sequences. As an outcome of the project, we demonstrated the applications of such embeddings for protein family classification tasks.

<p style="color:#FF5733"> Metric Learning on Biological Sequences Embeddings </p>
<hr style="margin-top:-0.5em; height:2px;border-width:0;color:Yellow;background-color:black">
Keywords: Metric Learning, Classification, Retrieval

Machine learning algorithms that rely on distance metrics are computationally efficient and can handle large datasets; however, default distances in the embedded space often yield inadequate accuracy. In this work, we propose a framework that doesn't rely on default distance metrics (euclidean, cosine) instead uses Mahalanobis distance - that is learned using the available class label information. As an outcome of the work, we show performance improvements gained using Mahalanobis distance over the default Euclidean metric in both retrieval and classification tasks.

<p style="color:#FF5733"> Supervised approach for learning embeddings for biological sequences </p>

<hr style="margin-top:-0.5em; height:2px;border-width:0;color:Yellow;background-color:black">
Keywords: Supervised learning, Alignment free approaches, Retrieval, Classification

In this project, we introduce novel supervised representation learning methods <em>SuperVec</em> and <em>SuperVecX</em> that incorporate class label information along with the contextual information for learning sequence embeddings. We also provide a hierarchical approach on top of these embedding methods, specifically for <em>homologous sequence retrieval</em> tasks. The other contribution of this work is to introduce <em>hybrid-approaches</em> that uses standard alignment-based (<em>BLAST</em>) and alignment-free (<em>SuperVec(X)</em>) retrieval methods together for improving the sequence retrieval performance. As an outcome of the project, we showed the success of the proposed methods in terms of retrieval performance and computational efficiency for the <em>homologus sequence retrieval</em> task. We also showed that such embeddings could prove to be useful for other downstream bioinformatics applications such as various <em>protein classification</em> tasks.


<!-- ![]({{ site.url }}{{ site.baseurl }}/images/dk/suvec.png){: style="width: 300px; float: right; border: 10px"}

![]({{ site.url }}{{ site.baseurl }}/images/dk/hrerchical_approach.png){: style="width: 300px; float: left; border: 10px"} -->


<p style="color:#FF5733" > Protein-Protein Interaction Prediction </p>
<hr style="margin-top:-0.5em; height:2px;border-width:0;color:Yellow;background-color:black">
Keywords: Paired-input problem, Prediction, Sequence embeddings

PPI prediction is a paired input problem in which the prediction is made for two objects together. In this ongoing work, we explore the usability of representation learning approaches as a feature constructor of paired samples. Such features can give the computational and performance advantage compared to the prevalent high dimensional embeddings that rely on physicochemical properties on this problem. We establish that the low dimensional representations for protein pair generally gives better performance than the physicochemical properties based feature vectors. The success of such methods would also help in extending them for including the meta-information from the protein interaction networks or annotations from the Gene Ontology graph.

<p style="color:#FF5733"> Semi-supervised framework for representation learning </p>
<hr style="margin-top:-0.5em; height:2px;border-width:0;color:Yellow;background-color:black">
Keywords: Representation Learning, Semi-Supervised approach, Alignment-free approach

Acquiring the quality labels (such as functional annotations) for biological sequences is generally costly and time taking process because of which, for many sequences, we do not have the desired annotations available. Considering the limited availability of labels (annotations), in this work, our focus is to develop a semi-supervised representation learning approach that can generate the quality embedding of sequences, requiring only few labels for training the model. We expect such approach to improve upon the unsupervised methods and give comparable results to the supervised methods for downstream bioinformatics tasks such as sequence retrieval and protein family classification.









































































<!--
Our overarching goal is to explore and understand new quantum states of electronic matter on the atomic scale. To do so, we use and develop novel spectroscopic-imaging scanning tunneling microscopy (SI-STM) tools to visualize the relevant quantum mechanical degrees of freedom.

Questions of interest include: (i), How does the Mott state collapse upon doping and how is this related to the complex phase diagram of high-temperature superconductors? (ii), What is the strange metal phase seen in correlated electron systems? Is this an exotic long-range entangled state? What is the mechanism of dissipation in that state? (iii), Why is the transition temperature in high-temperature superconductors so high?

![]({{ site.url }}{{ site.baseurl }}/images/respic/layers_real.jpg){: style="width: 300px; float: right; border: 10px"}

Currently, our instrument of choice  is SI-STM.  State-of-the-art SI-STM measures an array of tunneling spectra on a given sample, registered to the atomic sites with picometer precision. Each is proportional to the local density of states at a given location. Ideally, the recorded spectra are so tightly packed that the measurement yields a three-dimensional mapping of the local density of states as a function of locations and energy. This is shown on the image on the right-hand side (10x10 nm2), and its Fourier transform, below.

The quantum materials which we will investigate encapsulate some of the great unsolved mysteries of physics. They include high-temperature superconductors, quantum-critical compounds, graphene, and topological electronic matter that can be used for error-resistant quantum computing.

![]({{ site.url }}{{ site.baseurl }}/images/respic/layers_fft.jpg){: style="width: 300px; float: left; border: 10px"}

A main goal is to use modern technology to build the new instrumentation needed to understand these quantum materials. I learned my trade in [Seamus Davis’ SI-STM lab](http://davisgroup.lassp.cornell.edu/) and with [Felix Baumberger](http://dpmc.unige.ch/gr_baumberger/index.html), and later moved as an [ETH fellow](http://www.ethfellows.ethz.ch/) to [Andreas Wallraff’s qudev lab](http://www.qudev.ethz.ch/) where we investigated coupled cavity arrays in circuit QED. This allowed me to learn new techniques such as high frequency measurements, low temperature noise-free amplification, and quantum-limited measurements. The goal is to combine these with SI-STM.

This will enable the instrumental capabilities to visualize the different quantum mechanical degrees of freedom needed to understand next-generation quantum materials. STM will be the main method, but we use different spectroscopic-imaging techniques to visualize not only the topography, but also the density of states, spins, and other degrees of freedom hidden below the surface. -->
