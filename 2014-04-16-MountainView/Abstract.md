## Computational methods for mixed-effects models
### Douglas Bates, University of Wisconsin-Madison

In statistics, "mixed-effects" models extend linear or generalized
linear models by allowing for some of the categorical covariates to be
be modeled using random effects, as opposed to fixed-effects
parameters.  The names should refer to "levels" instead of "effects"
because the distinction is whether the levels of a covariate stay
fixed across the experiments or studies (e.g. 'sex' with levels 'male'
and 'female') or represent a sample from a population of possible
levels (e.g. 'participant' or 'item'). We describe the formulation of
linear mixed models used in the _lme4_ package for _R_ and in the
_MixedModels_ package for _Julia_.  The log-likelihood or the REML
criterion to be optimized by the parameter estimates can be expressed
surprisingly succinctly, leading to effective computational methods.
However, applying these methods at "Google scale" requires much more
care than for small data sets.  We describe the current methods for
different model configurations and directions in which they could be
parallelized.  Extensions to generalized linear mixed models (GLMMs)
for binary or count responses provide even greater challenges at large
scale, as we will describe.
