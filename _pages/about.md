---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a graduate student in the Master of Science in Geophysics program at the University of British Columbia. I obtained my Honours Bachelor of Science degree (Mathematics & Its Applications Specialist (Physical Science); Physics Major) at the University of Toronto.

My research interests include AI for physics and applications of machine learning models to inverse problems. In my Master's thesis, I focus on leveraging test time learning ML methods to the geophysical inverse problems. I'm also broadly interested in inverse problems in other subfields of physics such as earthquake (worked under the supervision of Prof. Qinya Liu at UofT), cosmology (worked under the supervision of Dr. Keir Rogers at UofT), and fluorescence microscope (worked under the supervision under Luca Calatroni and Laure Blanc-Féraud at CNRS).

You can find my publications, conference abstracts, and my CV above.

You can find out more about my recent research below.

Leveraging convolutional neural networks for implicit regularization in DC resistivity inversions (DIP-Inv) 
======
Regularization is critical for solving ill-posed geo- physical inverse problems. Explicit regularization is often used, but there are opportunities to explore the implicit regularization effects that are inherent in a Neural Network structure. Re- searchers have discovered that the Convolutional Neural Network (CNN) architecture inherently enforces a regularization that is advantageous for addressing diverse inverse problems in computer vision, including de-noising and in-painting. In this study, we examine the applicability of this implicit regularization to geophysical inversions. The CNN maps an arbitrary vector to the model space. The predicted subsurface model is then fed into a forward numerical simulation to generate corresponding predicted measurements. Subsequently, the objective function value is computed by comparing these predicted measurements with the observed measurements. The backpropagation algorithm is employed to update the trainable parameters of the CNN during the inversion. Note that the CNN in our proposed method does not require training before the inversion, rather, the CNN weights are estimated in the inversion process, hence this is a test- time learning (TTL) approach. In this study, we choose to focus on the Direct Current (DC) resistivity inverse problem, which is representative of typical Tikhonov-style geophysical inversions (e.g. gravity, electromagnetic, etc.), to test our hypothesis. The experimental results demonstrate that the implicit regularization can be useful in some DC resistivity inversions. We also provide a discussion of the potential sources of this implicit regularization introduced from the CNN architecture and discuss some practical guides for applying the proposed method to other geophysical methods.

You can find more details in the github repo: https://github.com/anna1963/DIP-Inv

<img src='/images/AGU23.png'>

Leverage Neural fields to the geophysical inverse problems 
======
The recent surge in test time learning (TTL) has garnered substantial attention from researchers, particularly in the context of incorporating machine learning algorithms into the inversion process. The deep image prior (DIP) method and coordinate-based representations (e.g., neural fields) have shown that neural networks, without any prior learning, can produce good inversion results. In this work, we will discuss the progress in utilizing neural fields in the geophysical inverse problems. Neural fields use neural networks to map a coordinate to the corresponding physical property value at that coordinate. We formulate the inverse problem in terms of the NN-weights, which allows us to take advantage of searching over the high-dimensional space.  Furthermore, parameterizing the inverse problems in a continuous setting naturally introduces smoothing effects. We integrate the neural fields into seismic tomography inversions and direct current resistivity inversions. The results show that this TTL approach can eliminate unwanted artifacts in the recovered subsurface physical property model caused by the sensitivity of the survey and physics. We also find that our results are better than the conventional inversion results in some cases in terms of the recovery of the boundaries and physical property values of the main targets. Our work illustrates that the inductive bias brought by a neural field can be beneficial in geophysical inversion. 



