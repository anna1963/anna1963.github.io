---
layout: archive
title: "Conferences"
permalink: /conferences/
author_profile: true
redirect_from:
  - /conferences
---

Leveraging Convolutional Neural Networks for implicit regularization
======
Advancing Earth and Space Science (AGU23, December 13, 2023) [awarded the Outstanding Student Presentation Awards (OSPA)]

Anran Xu, Lindsey Justine Heagy and John Weis, University of British Columbia

You can find the e-poster and a video presentation (bottom right icon "VEDIO PRES") [here](https://agu23.ipostersessions.com/?s=C6-F6-87-20-DE-67-43-79-FD-E2-69-3E-7C-5A-FA-EF)

Abstract:

The recent emergence of artificial intelligence has garnered significant attention from researchers, particularly regarding the integration of machine learning algorithms into the inversion algorithm. Researchers in Computer Vision (CV) have discovered that the Convolutional Neural Network (CNN) architecture inherently enforces a prior knowledge that is advantageous for addressing diverse CV inverse problems, including de-noising and inpainting. This inherent regularization effect has been shown to improve models recovered through full waveform inversion of seismic data. Consequently, the utilization of trainable weights within the CNN to parameterize the subsurface map holds promise for potential applicability in other geophysical inversion problems. In this study, we examine the applicability to the inversion of DC resistivity data. The CNN maps an arbitrary vector to the model space (e.g. log-conductivity on the simulation mesh). The predicted subsurface model is fed into the SimPEG numerical simulation package to generate corresponding predicted measurements. Subsequently, the objective function value is computed by comparing these predicted measurements with the observed field measurements. The backpropagation algorithm is employed to update the trainable parameters of the CNN until convergence. Note that the CNN does not require training prior to the inversion, rather, the CNN weights are estimated in the inversion algorithm. Our preliminary work shows that we can recover models that are comparable to, and even superior to that obtained using a standard inversion. For example, we have found that relying on the implicit regularization of the CNN improves the recovery of the dip of a target when a standard L2 or L1 regularization is employed. This method is training-data-free, so it can be adapted to other EM inversion problems.

The follow-up work was published in IEEE Transactions on Geoscience and Remote Sensing, and you can find the link to the paper in the "Publications" section.

Leverage Neural fields to the geophysical inverse problems 
======
SLAM Conference on mathematics of Data Science (MDS24, October 25, 2024)

Anran Xu, and Lindsey Justine Heagy, University of British Columbia

Abstract:

The recent surge in test time learning (TTL) has garnered substantial attention from researchers, particularly in the context of incorporating machine learning algorithms into the inversion process. The deep image prior (DIP) method and coordinate-based representations (e.g., neural fields) have shown that neural networks (NN), without any prior learning, can produce good inversion results. In this work, we will discuss the progress in utilizing neural fields in the geophysical inverse problems. Neural fields use neural networks to map a coordinate to the corresponding physical property value at that coordinate. We formulate the inverse problem in terms of the NN weights, which allows us to take advantage of searching over the high-dimensional space. Furthermore, parameterizing the inverse problems in a continuous setting naturally introduces smoothing effects. We demonstrate the use of neural fields in seismic tomography inversions and direct current resistivity inversions. The results show that this TTL approach can eliminate unwanted artifacts in the recovered subsurface physical property model caused by the sensitivity of the survey and physics. We also find that our results are better than the conventional inversion results in some cases in terms of the recovery of the boundaries and physical property values of the main targets. Our work illustrates that the inductive bias brought by neural fields can be beneficial in geophysical inversion.

Paper in progress


