---
layout: page
title: Restricted Search Space Graph MCMC
description: A summary of my work on restricted search space MCMC for graph inference, using birth-death processes.
img: assets/img/mcmc_auc_roc_comparison.png
importance: 3
category: misc
---

My primary research focuses on developing scalable MCMC methods for graph inference. This page summarizes the key contributions of my work, [Restricted Search Space Graph MCMC via Birth-Death Processes](https://arxiv.org/abs/2604.10863), joint with Kieran R. Campbell and Radu V. Craiu.

**Key contributions:**

- Sharp lower and upper bounds on the restricted search space error introduced by hybrid order MCMC methods
- A novel trans-dimensional sampler that places a prior directly on the set of search spaces
- A closed-form expression for this search space prior, which lets researchers explicitly control the tradeoff between posterior fidelity and computational scaling
- An efficient implementation of the sampler in R, available at [morrisgreenberg/RestrictedSearchMCMC](https://github.com/morrisgreenberg/RestrictedSearchMCMC)

<div class="row justify-content-sm-center">
    <div class="col-sm-10 mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/mcmc_auc_roc_comparison.png" title="ROC AUC across models and start spaces" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    ROC AUC of recovering true graph edges with synthetic data generated from Gaussian Structural Equation Models, using a fixed sparsity budget.
</div>
