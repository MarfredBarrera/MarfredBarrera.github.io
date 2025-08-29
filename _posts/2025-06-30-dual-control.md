---
title: "Dual Control and Estimation for Batteries"
thumbnail: /assets/images/histograms.png

# categories:
#   - Blog
# tags:
#   - Post Formats
#   - readability
#   - standard
---

<figure>
  <img src="/assets/images/histograms.png" alt=""/>
  <figcaption>Simultaneous improvement in estimation and control.</figcaption>
</figure>



This [paper](https://arxiv.org/abs/2507.21300) was a joint project between the Safe Autonomous Systems Lab and Argonne National Laboratory. Here, we focused on the simultaneous improvement of both estimation and control for battery systems using nonlinear MPC and stochastic optimal control in systems with highly nonlinear observational models (i.e. SOC-OCV curves for batteries). This is achieved through deriving a deterministic surrogate to the stochastic
optimal control cost, parametrized by the mean and covariance of the state of charge of the system’s batteries. Although
our parametrization is independent of the type of filter, we
adopt the extended Kalman filter to approximate these statistics, due to its simplicity. We then use a randomized linear
parameter-varying model predictive control approximation to
solve for the control trajectory. We report an improvement
in control and state estimation that is more pronounced for
batteries with open circuit voltage models that deviate further
from linearity with respect to the state of charge, such as
lithium-sulfur batteries.