# Topic Alignment, by Book (Book Versions 5.4–6.2)

> **Archived version.** This guide covers CourseKata book versions 5.4–6.2 (college). For the current book, see [topic-alignment-book.md](topic-alignment-book.md).
>
> This guide is for instructors who teach introductory statistics with a more traditional (non-modeling) set of topics and want to know where to find those topics in the CourseKata books.

## Topics Covered in Introductory Statistics with R (ABC)

- Chapter 1 - Introduction to materials and R
- Chapter 2 - Data
  - Sampling
  - Measurement and types of variables
  - Organizing data (tidy data)
- Chapter 3 - Univariate distributions
  - Univariate visualizations: histograms, box plots, bar graphs, frequency tables
  - Shape/center/spread of distributions
  - Samples versus Populations/Data Generating Processes (DGPs)
  - Law of large numbers
  - Sampling with and without replacement
- Chapter 4 - Bivariate distributions
  - Bivariate visualizations: faceted histograms, box plots, scatterplots/jitter plots, bar graphs, contingency tables
  - Research design: correlational v. experimental
  - Introduction to random simulation
- Chapter 5 - Empty model
  - The mean as a model
  - Introduction to General Linear Model (GLM) notation
  - Predictions and residuals
- Chapter 6 - Quantifying and modeling error
  - SAD, Sum of squares, variance, standard deviation
  - Normal distribution
  - z-score
  - Probability distributions
- Chapter 7 - Group model (specifically two groups; i.e., situations that correspond to an independent samples t-test)
  - Adding a categorical explanatory variable (with two levels) to a model
  - Two means as a model
  - GLM notation; prediction; residuals
  - SS Total = SS Model + SS Error
  - PRE (also called partial eta squared)
- Chapter 8 - Group model generalized (beyond two groups; i.e., situations that correspond to ANOVAs)
  - Adding a categorical explanatory variable (with more than two levels) to a model
  - GLM notation; prediction; residuals; SS Total = SS Model + SS Error
  - PRE and F
  - Simulation to compare empty model against group model
- Chapter 9 - Regression model
  - Adding a quantitative explanatory variable to a model
  - GLM notation; prediction; residuals; SS Total = SS Model + SS Error; PRE and F
  - Correlation coefficient
  - Simulation to compare empty model against regression model
- Chapter 10 - Model comparison between empty/null model and a model with one explanatory variable (also called hypothesis testing; corresponds to t-test)
  - simulating sampling distributions of mean differences and means
  - t-distributions as mathematical models of these sampling distributions
  - alpha
  - p-value
  - model comparison of empty model versus group model
  - model comparison of empty model versus regression model
- Chapter 11 - Model comparison between empty/null model and a model with one explanatory variable (corresponds to ANOVA)
  - simulating sampling distributions of PRE and F
  - F-distributions as models of these sampling distributions
  - type I and type II error
  - problem of simultaneous comparisons; pairwise comparisons
  - chi-square
- Chapter 12 - Parameter estimation and confidence intervals
  - bootstrapping sampling distributions of parameter estimates
  - connecting confidence intervals with model comparison/hypothesis testing
  - what affects confidence intervals

## Topics Additionally Covered in Advanced Statistics with R (ABCD)

(Same up to chapter 12; adds on 4 additional chapters focused on multivariate statistics)

- Chapter 13: Additive Models (starting with models that have two explanatory variables)
  - ANCOVA (one categorical and one quantitative explanatory variable; no interactions)
  - Parameter estimates, predictions, residuals
  - Model comparison between empty model and multivariate model
- Chapter 14: Models with two explanatory variables compared to models with one
  - Model comparison between one-variable model and multivariate model
  - Extension to models with more than 2 variables
  - Extension to factorial ANOVA and multivariate regression
- Chapter 15: Models with interactions
  - ANCOVA (one categorical and one quantitative explanatory variable; with interactions)
  - Parameter estimates, predictions, residuals
  - Model comparison between additive model and interaction model
- Chapter 16: More models with interactions
  - Factorial ANOVA (with interactions)
  - Multiple regression (with interactions)
