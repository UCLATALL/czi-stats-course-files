# Topic Alignment, by Book (Book Version 7+)

This guide is for instructors who teach introductory statistics with a more traditional (non-modeling) set of topics and want to know where to find those topics in the CourseKata books. Chapter and page numbers refer to version 7.2 of the college books: *Introductory Statistics with R (ABC)* and *Advanced Statistics with R (ABCD)*.

## Traditional Topics at a Glance

| Traditional topic | Where to find it |
|---|---|
| Types of variables; measurement | Chapter 2 (2.5–2.7) |
| Sampling; samples vs. populations | Chapter 2 (2.8); Chapter 3 (3.10–3.13) |
| Frequency tables | Chapter 2 (2.4) |
| Histograms, box plots, five-number summary | Chapter 3 (3.2–3.8) |
| Shape, center, and spread | Chapter 3 (3.4) |
| Bar graphs; categorical variables | Chapter 3 (3.9); Chapter 4 (4.6) |
| Scatterplots | Chapter 4 (4.2) |
| Contingency tables | Chapter 4 (4.7) |
| Study design: correlational vs. experimental | Chapter 4 (4.10) |
| Mean and median | Chapter 5 (5.2–5.4) |
| Sum of squares, variance, standard deviation | Chapter 6 (6.1–6.4) |
| z-scores | Chapter 6 (6.5–6.6) |
| Normal distribution; empirical rule | Chapter 6 (6.7–6.11) |
| Independent samples t-test (as model comparison) | Chapter 7 (model); Chapters 10–11 (inference) |
| One-way ANOVA (as model comparison) | Chapter 8 (model); Chapter 11 (inference) |
| Regression and correlation | Chapter 9; inference in Chapters 10–12 |
| Sampling distributions | Chapter 10 (10.2–10.3); Chapter 11 (11.2–11.3) |
| Hypothesis testing, p-value, alpha | Chapter 10 |
| t-distribution | Chapter 10 (10.7); Chapter 11 (11.7); Chapter 12 (12.7) |
| Type I and Type II error | Chapter 11 (11.9) |
| Pairwise/multiple comparisons | Chapter 11 (11.11–11.12); Chapter 12 (12.12) |
| Chi-square test of independence | Chapter 11 (11.13) |
| Confidence intervals; bootstrapping; standard error | Chapter 12 |
| ANCOVA, factorial ANOVA, multiple regression, interactions | Chapters 13–16 (ABCD only) |

## Topics Covered in Introductory Statistics with R (ABC)

- Chapter 1 - Welcome to Statistics: A Modeling Approach
  - Introduction to the materials and the goals of the course
  - Introduction to R: functions, arguments, and R objects
- Chapter 2 - Understanding Data
  - From numbers to data; data frames (tidy data)
  - Frequency tables and sorting data
  - Measurement and types of variables (quantitative and categorical)
  - Sampling from a population
  - Missing data; creating and recoding variables
- Chapter 3 - Examining Distributions
  - Univariate visualizations: histograms, box plots, bar graphs
  - Shape/center/spread of distributions; outliers
  - Five-number summary and quartiles
  - Samples versus Populations/Data Generating Processes (DGPs)
  - Law of large numbers
  - Sampling with and without replacement
- Chapter 4 - Explaining Variation
  - Outcome and explanatory variables
  - Bivariate visualizations: scatterplots/jitter plots, box plots, faceted histograms, bar graphs, contingency tables
  - Research design: correlational v. experimental
  - Introduction to random simulation: randomness as a possible DGP; shuffling
- Chapter 5 - A Simple Model (the empty model)
  - The mean as a model; median versus mean
  - Predictions and residuals; DATA = MODEL + ERROR
  - Introduction to General Linear Model (GLM) notation
- Chapter 6 - Quantifying Error
  - SAD, sum of squares, variance, standard deviation
  - z-scores
  - Normal distribution as a model of error; using it to make predictions (probability)
  - The empirical rule
- Chapter 7 - Adding an Explanatory Variable to the Model (specifically two groups; i.e., situations that correspond to an independent samples t-test)
  - Adding a categorical explanatory variable (with two levels) to a model
  - Two means as a model
  - GLM notation; prediction; residuals
  - SS Total = SS Model + SS Error
  - PRE (also called partial eta squared)
- Chapter 8 - Digging Deeper into Group Models (beyond two groups; i.e., situations that correspond to ANOVAs)
  - Adding a categorical explanatory variable (with more than two levels) to a model
  - GLM notation; prediction; residuals; SS Total = SS Model + SS Error
  - PRE and the F ratio; measures of effect size
  - Modeling the DGP; shuffling to compare empty model against group model
- Chapter 9 - Models with a Quantitative Explanatory Variable (regression)
  - Adding a quantitative explanatory variable to a model
  - GLM notation; interpreting parameter estimates; prediction; residuals
  - Sums of squares in the ANOVA table; PRE and F
  - Correlation coefficient (Pearson's r)
  - Shuffling to interpret the slope of a regression line
- Chapter 10 - The Logic of Inference (also called hypothesis testing; corresponds to t-test)
  - Simulating the sampling distribution of b₁ (a group difference or a regression slope)
  - t-distribution as a mathematical model of the sampling distribution of b₁
  - alpha; p-value; what affects the p-value
  - Hypothesis testing for group models and regression models
- Chapter 11 - Model Comparison with F (corresponds to ANOVA)
  - Simulating sampling distributions of PRE and F
  - F-distribution as a model of these sampling distributions; relation of F to t
  - Type I and Type II error
  - Comparing multiple groups; pairwise comparisons; the problem of simultaneous comparisons
  - Chi-square test of independence
- Chapter 12 - Parameter Estimation and Confidence Intervals
  - Bootstrapping sampling distributions of parameter estimates; standard error
  - Constructing confidence intervals with the t-distribution
  - Connecting confidence intervals with model comparison/hypothesis testing
  - Confidence intervals for the intercept, the slope of a regression line, and pairwise comparisons
  - What affects the width of confidence intervals
- Chapter 13 - What You Have Learned (ABC only)
  - Review of the three big ideas of the course: exploring variation, modeling variation, and evaluating models

## Topics Additionally Covered in Advanced Statistics with R (ABCD)

(Same as ABC up to Chapter 12; instead of ABC's review chapter, adds four chapters focused on multivariate statistics)

- Chapter 13 - Introduction to Multivariate Models (models with two explanatory variables)
  - ANCOVA-type additive models (one categorical and one quantitative explanatory variable; no interactions)
  - Parameter estimates, predictions, residuals
  - Venn diagrams for conceptualizing sums of squares, PRE, and F
  - Model comparison between empty model and multivariate model
- Chapter 14 - Multivariate Model Comparisons
  - Targeted model comparisons: one-variable model versus multivariate model
  - Deciding which predictors to include in a model
  - Models with multiple categorical predictors (factorial ANOVA, no interactions)
  - Models with multiple quantitative predictors (multiple regression)
- Chapter 15 - Models with Interactions
  - ANCOVA-type interaction models (one categorical and one quantitative explanatory variable; with interactions)
  - Parameter estimates, predictions, residuals; centering predictors
  - Model comparison between additive model and interaction model
- Chapter 16 - More Models with Interactions
  - Interactions with two quantitative predictors (multiple regression with interactions)
  - Interactions with two categorical predictors (factorial ANOVA with interactions)

## Notable Changes from the 5.4–6.2 Version of This Guide

- Chapter titles now reflect the official version 7 titles (e.g., Chapter 5 is "A Simple Model" rather than "Empty model").
- Frequency tables are introduced in Chapter 2 (with data frames) rather than Chapter 3.
- Chapter 10 is now organized around the sampling distribution of b₁ (a single framework covering both group differences and regression slopes), rather than sampling distributions of means and mean differences.
- ABC now ends with a review chapter (Chapter 13 - What You Have Learned), which is not in ABCD.
