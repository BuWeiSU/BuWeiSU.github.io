---
layout: archive
permalink: /medication/
title: "Medication"
author_profile: true
redirect_from: 
  - /medication_recommendation/
  - /medication_recommendation.html
---

这个文档是我阅读药物推荐领域的相关论文的总结与梳理，旨在阐明药物推荐领域的发展脉络，为药物推荐领域综述书写打下较为良好的基础。

### Change Matter: Medication Recommendation with Recurrent Residual Networks, Chaoqi Yang,IJCAI-21

Motivation:
Change in different visits should be noticed to conduct medicaiton recommendation more human-like. Therefore, the author builds a model to achieve the reconstruction medication substraction results using 
corresponding patient representation substraction results.

Methods:
It runs 1.5 times faster and achieves 3.5% improvement on the best baselines.

Comments:
- When conducting experiments, the author disregard patients' first visit record to suit his model. This make the structure of this paper less parctical.
- The result of this paper is strange because GAMENet achieves lower result than the orginal paper with more time dependencies.



### Self-suprivised Adversarial Distribution Regularization for Medication Recommendation, Yanda Wang, IJCAI-21

Motivation:
The author thinks most existing ways to tune down DDI rate are constraining and limits models.
Methods:
The author puts up a new way to split patients. He trains patient with lower DDI first and then use GAN to make other patient representations intimate the former group to reduce DDI level. When training the net for med, the author uses memory bank and multi-hop techniques.

This method achieves lower DDI rate and achieves better results.

Comments:
- what about the cost of this model, temporal and space?
- any side effects of this regularization?

### Debiased Longitudinal and Coordinated Drug Recommendation through Multi-Visit Clinic Records
