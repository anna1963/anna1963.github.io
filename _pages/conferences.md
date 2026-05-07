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
Advancing Earth and Space Science (AGU23, December 13, 2023) [__awarded the Outstanding Student Presentation Awards (OSPA)__]

Anran Xu, Lindsey Justine Heagy and John Weis, University of British Columbia

You can find the e-poster and a video presentation (bottom right icon "VEDIO PRES") [here](https://agu23.ipostersessions.com/?s=C6-F6-87-20-DE-67-43-79-FD-E2-69-3E-7C-5A-FA-EF)

Abstract:

The recent emergence of artificial intelligence has garnered significant attention from researchers, particularly regarding the integration of machine learning algorithms into the inversion algorithm. Researchers in Computer Vision (CV) have discovered that the Convolutional Neural Network (CNN) architecture inherently enforces a prior knowledge that is advantageous for addressing diverse CV inverse problems, including de-noising and inpainting. This inherent regularization effect has been shown to improve models recovered through full waveform inversion of seismic data. Consequently, the utilization of trainable weights within the CNN to parameterize the subsurface map holds promise for potential applicability in other geophysical inversion problems. In this study, we examine the applicability to the inversion of DC resistivity data. The CNN maps an arbitrary vector to the model space (e.g. log-conductivity on the simulation mesh). The predicted subsurface model is fed into the SimPEG numerical simulation package to generate corresponding predicted measurements. Subsequently, the objective function value is computed by comparing these predicted measurements with the observed field measurements. The backpropagation algorithm is employed to update the trainable parameters of the CNN until convergence. Note that the CNN does not require training prior to the inversion, rather, the CNN weights are estimated in the inversion algorithm. Our preliminary work shows that we can recover models that are comparable to, and even superior to that obtained using a standard inversion. For example, we have found that relying on the implicit regularization of the CNN improves the recovery of the dip of a target when a standard L2 or L1 regularization is employed. This method is training-data-free, so it can be adapted to other EM inversion problems.

The follow-up work was published in IEEE Transactions on Geoscience and Remote Sensing, and you can find the link to the paper in the "Publications" section.

Leverage Neural fields to the geophysical inverse problems 
======
SIAM Conference on Mathematics of Data Science (MDS24, October 25, 2024)

Anran Xu, and Lindsey Justine Heagy, University of British Columbia

Abstract:

The recent surge in test time learning (TTL) has garnered substantial attention from researchers, particularly in the context of incorporating machine learning algorithms into the inversion process. The deep image prior (DIP) method and coordinate-based representations (e.g., neural fields) have shown that neural networks (NN), without any prior learning, can produce good inversion results. In this work, we will discuss the progress in utilizing neural fields in the geophysical inverse problems. Neural fields use neural networks to map a coordinate to the corresponding physical property value at that coordinate. We formulate the inverse problem in terms of the NN weights, which allows us to take advantage of searching over the high-dimensional space. Furthermore, parameterizing the inverse problems in a continuous setting naturally introduces smoothing effects. We demonstrate the use of neural fields in seismic tomography inversions and direct current resistivity inversions. The results show that this TTL approach can eliminate unwanted artifacts in the recovered subsurface physical property model caused by the sensitivity of the survey and physics. We also find that our results are better than the conventional inversion results in some cases in terms of the recovery of the boundaries and physical property values of the main targets. Our work illustrates that the inductive bias brought by neural fields can be beneficial in geophysical inversion.

Towards Understanding the Benefits of Neural Network Parameterizations in Geophysical Inversions: A Study With Neural Fields
======
KEGS  (KEGS25, March, 2025) [oral presentation]

Anran Xu, and Lindsey Justine Heagy, University of British Columbia

Abstract:

Recent research in test-time machine learning methods has shown that some machine learning models without any prior learning can improve the results of geophysical inversions. Some examples include the Deep Image Prior Inversions (DIP-Inv) and the Neural Fields Inversions (NFs-Inv), where the inverse problems are reparametrized by the weights of the machine learning models, and those weights are estimated during the inverse process. These methods utilize the implicit bias, which is inherent in the machine learning model structures, to impose a useful regularization effect on the geophysical inverse problems. However, the underlying mechanism of this implicit bias has not been fully explained. Recently, the generalization of modern supervised learning models in some inverse tasks in computer vision has been attributed to implicit bias as well. Considering that this implicit bias does not come from the training data set, we could utilize the analysis of that work to take one step further to explain the performance of the implicit bias and test-time learning methods in the geophysical inverse problems. In this work, we will show that the test-time machine learning methods can improve the geophysical inversion result by finding weights that can capture geometric structures in the physical property model (or so-called “geometry-adaptive harmonic bases”). We use neural fields, which use neural networks to map a coordinate to the corresponding physical property value at that coordinate, in a test-time learning manner. For a test-time learning method, the weights are learned during the inversion, as compared to traditional approaches which require a network be trained using a training data set. The test results for seismic tomography inversions and direct current resistivity inversions are shown first, followed by the eigen-decomposition analysis for both cases. The results show that the test-time learning approach can eliminate unwanted artifacts in the recovered subsurface physical property model caused by the sensitivity of the survey and physics; therefore, NFs-Inv improve the inversion results compared to the conventional inversion in some cases such as the recovery of the dip angle or the prediction of the boundaries of the main target. Our analysis will partly explain this phenomenon. Further works such as the applications in the field data and other theoretical analyses of the implicit bias are still in progress. By showing that the implicit bias brought by the Deep Neural Networks (DNNs) can benefit geophysical inversions, we also give insights into other machine learning methods in geophysics. 

Leveraging Implicit Regularization with Test-Time Machine Learning Methods for PDE-Constrained Optimization
======
SIAM Conference on Optimization (OP26, June, 2026) [**Session Chair**]

Anran Xu, and Lindsey Justine Heagy, University of British Columbia

Abstract:

We focus on geophysical inverse problems, which can be posed as a PDE-constrained optimization problem, for example, with Maxwell's equations or the seismic wave equation. Geophysical inversions are used for imaging subsurface structures and are an essential tool for mineral exploration and environmental studies. The solutions of these inverse problems are non-unique. Without explicit regularization, such as Tikhonov regularization, optimizing over the original mesh space often finds solutions with unwanted artifacts due to the survey sensitivity and physics. Test-time learning (TTL) methods change the optimization space from the mesh to the weights of a neural network. Unlike supervised learning, TTL leverages the implicit regularization of ML architectures and optimizers without requiring training data. We evaluate TTL methods in various synthetic and field data and find that the results do not have those unwanted artifacts. Our study shows that some inductive bias (from the architecture) and some implicit bias (from the optimizer), which has been illustrated in supervised learning models, can be observed and utilized in the setting without data. We find that the inductive bias, observed in the generative models, such as the geometry-adaptive harmonic basis, may also apply to TTL methods. We find the effect of different optimization methods on the sharpness of the convergence point in TTL methods, which is connected to the generalization in the supervised setting.

