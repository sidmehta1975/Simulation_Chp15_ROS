# Simulation_Chp15_ROS
Learning fake data simulation from Regression & other stories. This repo was created on the 9th March 2025.

I've been struggling to interpret the bayesian credible intervals appropriately and read the following : https://sites.stat.columbia.edu/gelman/research/published/Uncertainty.pdf

This proved to be useful and essentially highlights the following logic to determine the interpretation from baysesian cerdible intervals.

If we were to compare the credible interval with a ROPE (region of probability equivalence), we will encounter 5 scenarios:

1) Credible intervals are completely to the right of ROPE
2) Credible intervals are completely to the left of ROPE
3) Credible intervals completely overlap with the ROPE
4) Credible intervals overlap with the ROPE byt have a large probbability to the right of ROPE
5) 4) Credible intervals overlap with the ROPE byt have a large probbability to the left of ROPE

Interpretation:
- In the case of 1 and 2, we have strong evidence that the estimate of effect varies from ROPE with certainty.
- In the case of 3, we have strong evidence that the estimate matches ROPE. There is a variation to this which will be highlighted below as scenario-6
- In the case of 4 and 5, we can assess the esteent to which the credible intervals match the ROPE ie what proportion of the CI is higher or lower than the ROPE. These scenarios clearly highlight uncertaintly but allows us to estimate this and gude our judgment about the effect size.

There is a sixth potential scenario, in which the CI and ROPE overlap, but the CI is wide such that the overlap region is a small proportion of the CI. This suggests that there is very high uncertainty about the effect estimate and that the information (data/ model) are insufficient to inform our conclusion.

The article also highlights the power of fake data simulation as a precursor to actual analyses. Gelman (& others) in his blog suggests learning about this from two books - 
1) Regression & other stories; 2) Gelman & Hill book on multilevek modeling (2007)

Inspiring blog-posts about the usefulness of fake data simulation:

* https://statmodeling.stat.columbia.edu/2019/03/23/yes-i-really-really-really-like-fake-data-simulation-and-i-cant-stop-talking-about-it/
* https://statmodeling.stat.columbia.edu/2020/08/05/somethings-do-not-seem-to-spread-easily-the-role-of-simulation-in-statistical-practice-and-perhaps-theory/

