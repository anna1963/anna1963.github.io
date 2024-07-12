---
permalink: /
title: "Anran Xu's academic personal websites"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a graduate student who are in the Master of Science in Geophysics program at the University of British Columbia. Before that I obtained my Honours Bachelor of Science degree (Mathematics & Its Applications Specialist (Physical Science); Physics Major) at the University of Toronto.

My research interests include AI for physics, optimizations, and applications of machine learning models to inverse problems. In my Master's thesis, I focuses on leveraging test time learning ML methods to the geophysical inverse problems. I'm also bordly interested in inverse problems in the subfields of physics such as cosmology and fluorescence image super-resolutions.

##Leveraging convolutional neural networks for implicit regularization in DC resistivity inversions (DIP-Inv)
======
The recent emergence of artificial intelligence has garnered significant attention from researchers, particularly regarding the integration of machine learning algorithms into the inversion algorithm. Researchers in Computer Vision (CV) have discovered that the Convolutional Neural Network (CNN) architecture inherently enforces a prior knowledge that is advantageous for addressing diverse CV inverse problems, including de-noising and inpainting. This inherent regularization effect has been shown to improve models recovered through full waveform inversion of seismic data. Consequently, the utilization of trainable weights within the CNN to parameterize the subsurface map holds promise for potential applicability in other geophysical inversion problems. In this study, we examine the applicability to the inversion of DC resistivity data. The CNN maps an arbitrary vector to the model space (e.g. log- conductivity on the simulation mesh). The predicted subsurface model is fed into the SimPEG numerical simulation package to generate corresponding predicted measurements. Subsequently, the objective function value is computed by comparing these predicted measurements with the observed field measurements. The backpropagation algorithm is employed to update the trainable parameters of the CNN until convergence. Note that the CNN does not require training prior to the inversion, rather, the CNN weights are estimated in the inversion algorithm. Our preliminary work shows that we can recover models that are comparable to, and even superior to that obtained using a standard inversion. For example, we have found that relying on the implicit regularization of the CNN improves the recovery of the dip of a target when a standard L2 or L1 regularization is employed. This method is training-data-free, so it can be adapted to other EM inversion problems.

<img src='/images/AGU23.png'>

##Leverage Neural fields to the geophysical inverse problems 
======
The recent surge in test time learning (TTL) has garnered substantial attention from researchers, particularly in the context of incorporating machine learning algorithms into the inversion process. The deep image prior (DIP) method and coordinate-based representations (e.g., neural fields) have shown that neural networks, without any prior learning, can produce good inversion results. In this work, we will discuss the progress in utilizing neural fields in the geophysical inverse problems. Neural fields use neural networks to map a coordinate to the corresponding physical property value at that coordinate. We formulate the inverse problem in terms of the NN-weights, which allows us to take advantage of searching over the high-dimensional space.  Furthermore, parameterizing the inverse problems in a continuous setting naturally introduces smoothing effects. We integrate the neural fields into seismic tomography inversions and direct current resistivity inversions. The results show that this TTL approach can eliminate unwanted artifacts in the recovered subsurface physical property model caused by the sensitivity of the survey and physics. We also find that our results are better than the conventional inversion results in some cases in terms of the recovery of the boundaries and physical property values of the main targets. Our work illustrates that the inductive bias brought by a neural field can be beneficial in geophysical inversion. 


