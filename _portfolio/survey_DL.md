---
title:      "Survey of Dictionary Learning"
collection: portfolio
permalink: /portfolio/DL
excerpt:    '<img src="/images/Survey_DL/DL.jpg"  alt="drawing" height="300"/>'
date:       2018-07-06
tags:
  - dictionary learning
---

<center>
<img src="/images/Survey_DL/DL.jpg"  alt="drawing" height="300"/>
</center>

<center>
	<a href="/files/Survey_Dictionary_Learning.pdf" target="_blank" class="btn btn-danger">
		<span style="font-size: 120%;">
		Technical Report
		</span>
	</a>
</center>

**Dictionary learning (DL)** is an algorithm to learn the basis set from the given data set, 
so these data can be expressed in sparse linear combination.
Many applications illustrate that DL can achieve state-of-the-art performance in both denoising and classification.
In this technical report, we reviewed the statistical guarantee, namely the generalization bound, 
of reconstructive dictionary learning (RDL) and predictive dictionary learning(PDL).
In addition, we also summarized the state-of-the-art optimization algorithms, such as 
**method of optimal directions (MOD)**, **K-SVD** and **online dictionar learning (ODL)** for RDL, 
and **task-driven dictionary learning (TDDL)** for PDL.
We also put emphasis on the sparse coding optimization algorithms, such as 
**iterative shrinkage-thresholding algorithm (ISTA)** and its extension **fast iterative shrinkage-thresholding algorithm (FISTA)**.
Furthermore, we studied their convergence rates and compared them to **Nesterov's accelerated gradient descent**.
