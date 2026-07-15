# Using ABC/ABCD Teaching Materials with XCD

The CourseKata [teaching materials](https://github.com/UCLATALL/teaching-materials) (Overview, Mini, and Investigation Jupyter notebooks, projects, and tests) are organized by the chapters and page ranges of the ABC/ABCD books, because ABC is the most widely used book. This guide tells instructors teaching from *Accelerated Statistics with R (XCD)* which XCD pages correspond to each ABC/ABCD section, so they can tell when to use each set of materials.

Verified against version 7.2 of both books.

## The Big Picture

- **XCD Chapters 1–3** compress ABC/ABCD Chapters 1–9 into three accelerated chapters (XCD 1 ≈ Chapters 1–3; XCD 2 ≈ Chapters 4–6; XCD 3 ≈ Chapters 7–9). The XCD pages are rewritten and condensed, not copied, and some topics are trimmed entirely (see notes below).
- **XCD Chapters 4–10** are identical in content to ABCD Chapters 10–16, page for page: just subtract 6 from the ABCD chapter number (ABCD 11.3 = XCD 5.3). Materials for ABCD Chapters 10–16 can be used with XCD as-is.

**A caveat on datasets:** the condensed XCD chapters often use different running examples than ABC/ABCD. For example, XCD Chapter 1 works with `TipExperiment` and `Ames` (home sales), and XCD Chapter 3 builds the `PriceK ~ Neighborhood` and `PriceK ~ HomeSizeK` models from `Ames`, where ABCD Chapter 7 uses `TipExperiment` and Chapter 9 the thumb-length/height model. The concepts align, but materials that lean on a specific dataset may need light adaptation.

## Section-by-Section Mapping

Sections below match the page ranges used in the teaching-materials file names (e.g., `OverviewJNB-2.1-2.7`, `miniJNB-5.5-5.7`). A dash (—) means the section's content is not substantially covered in XCD; those materials can still be used as supplements if you want to add the topic back in.

| ABC/ABCD section | Use with XCD pages | Notes |
|---|---|---|
| 1.1–1.7 | 1.1–1.4 | Welcome and R basics, condensed |
| 2.1–2.7 | 1.5–1.6, 1.11 | Data frames and variable types; frequency tables are in 1.11; measurement (2.5) is not covered in XCD |
| 2.8–2.11 | 1.7–1.9 | Structure of data, missing data, recoding; sampling (2.8) is only touched on (XCD 2.8) |
| 3.1–3.4 | 1.10 | Distributions, histograms, shape/center/spread |
| 3.5–3.9 | 1.10–1.11 | Five-number summary, box plots, outliers; categorical variables in 1.11 |
| 3.10–3.13 | — | The DGP/populations/samples arc is cut; DGP appears only in passing (XCD 2.4, 2.8) |
| 4.1–4.2 | 2.1–2.3 | Outcome/explanatory variables; scatter plots are in 2.3 |
| 4.3–4.5 | 2.2–2.3 | Box plots, faceted histograms for relationships |
| 4.6–4.9 | 2.2–2.4 | Color/multiple explanatory variables (2.2), sources of variation (2.4); contingency tables only briefly (1.9) |
| 4.10–4.13 | — | Research design and shuffling are cut; random assignment and confounding appear briefly in 3.13 |
| 5.1–5.4 | 2.4–2.5 | What a model is; mean (and median) as a model |
| 5.5–5.7 | 2.6, 2.9 | Fitting the empty model; predictions and residuals are in 2.9 |
| 5.8–5.10 | 2.7–2.8 | GLM notation; parameters and estimates |
| 6.1–6.3 | 2.9–2.10 | Quantifying error; sum of squares; variance briefly |
| 6.4–6.6 | 2.10 | Standard deviation briefly; z-scores (6.5–6.6) are not covered |
| 6.7–6.11 | — | Normal distribution as a model of error and the empirical rule are cut |
| 7.1–7.4 | 3.1–3.4 | Group model (XCD uses `PriceK ~ Neighborhood`), GLM notation, predictions |
| 7.5–7.8 | 3.4–3.5 | Residuals and error reduced by the model |
| 7.9–7.10 | 3.10–3.12 | Partitioning sums of squares; PRE |
| 8.1–8.3 | — | Three-group models are cut; multiple-group comparisons first appear at XCD 5.10 |
| 8.5–8.7 | — | Effect size, modeling the DGP, and shuffle are cut from the X chapters (8.4's F ratio is at XCD 3.13) |
| 9.1–9.4 | 3.6–3.8 | Regression model (XCD uses `PriceK ~ HomeSizeK`) |
| 9.5–9.7 | 3.9–3.13 | Error from the model, ANOVA tables, PRE and F; correlation (9.8–9.9) is not covered |
| 10.1–10.4 | 4.1–4.4 | Identical content |
| 10.5–10.7 | 4.5–4.7 | Identical content |
| 11.1–11.5 | 5.1–5.5 | Identical content |
| 12.1–12.5 | 6.1–6.5 | Identical content |

For any other range in Chapters 10–16, the rule is the same: subtract 6 from the chapter number and keep the page numbers (ABCD 11.9 = XCD 5.9; ABCD Chapters 13–16 = XCD Chapters 7–10).

## Page-by-Page Mapping (Chapters 1–9)

For finer-grained planning, this table maps each content page of ABC/ABCD Chapters 1–9 to the XCD page(s) covering the same ground (chapter review pages omitted). Mappings are based on matching page titles and content of version 7.2; because XCD condenses heavily, a single XCD page often absorbs several ABC pages, usually in less depth.

| ABC/ABCD page | XCD page(s) |
|---|---|
| 1.1 Welcome to Statistics | 1.1 |
| 1.2 What is Understanding? | 1.1 |
| 1.3 Doing Statistics with R | 1.2 |
| 1.4 Introduction to R Functions | 1.3 |
| 1.5 Save Your Work in R Objects | 1.4 |
| 1.6 What You Can Store in R Objects | 1.4 |
| 1.7 Goals of This Course | 1.1 (brief) |
| 2.1 Starting with a Bunch of Numbers | 1.5 |
| 2.2 From Numbers to Data | 1.5 |
| 2.3 A Data Frame Example | 1.5 |
| 2.4 Frequency Tables and Sorting Data Frames | 1.8, 1.11 |
| 2.5 Measurement | — |
| 2.6 Quantitative and Categorical Variables | 1.6 |
| 2.7 Values and Variables | 1.6 |
| 2.8 Sampling from a Population | — (touched on in 2.8) |
| 2.9 The Structure of Data | 1.5, 1.7 |
| 2.10 Missing Data | 1.8 |
| 2.11 Creating and Recoding Variables | 1.9 |
| 3.1 The Concept of Distribution | 1.10 |
| 3.2–3.3 Histograms | 1.10 |
| 3.4 Shape, Center, Spread, and Weird Things | 1.10 |
| 3.5–3.7 Five-Number Summary, Quartiles, Box Plots | 1.10 |
| 3.8 Outliers on a Box Plot | 1.10 |
| 3.9 Exploring Variation in Categorical Variables | 1.11 |
| 3.10–3.13 The DGP, Populations, and Samples | — |
| 4.1 Outcome and Explanatory Variables | 2.1 |
| 4.2 Visualizing Relationships with Scatter Plots | 2.3 |
| 4.3 Categorical Explanatory Variables | 2.2–2.3 |
| 4.4 Using Box Plots to Explore Relationships | 2.3 |
| 4.5 Faceted Histograms | 2.2 |
| 4.6 Categorical Outcomes | — |
| 4.7 Contingency Tables | 1.9 (brief) |
| 4.8 Adding More Explanatory Variables to a Plot | 2.2 |
| 4.9 Sources of Variation | 2.4 |
| 4.10 Research Design | — |
| 4.11–4.13 Randomness and Shuffling | — |
| 5.1 What is a Model, and Why Would We Want One? | 2.4 |
| 5.2 Modeling a Distribution as a Single Number | 2.5 |
| 5.3 Median vs. Mean as a Model | 2.5 |
| 5.4 Exploring the Mean | 2.5 |
| 5.5 Fitting the Empty Model | 2.6 |
| 5.6 Generating Predictions from the Empty Model | 2.6, 2.9 |
| 5.7 Thinking About Error | 2.6, 2.9 |
| 5.8 The World of Mathematical Notation | 2.7–2.8 |
| 5.9 DATA = MODEL + ERROR: Notation | 2.7–2.8 |
| 5.10 Summarizing Where We Are | — |
| 6.1 Quantifying Total Error Around a Model | 2.9 |
| 6.2 The Beauty of Sum of Squares | 2.10 |
| 6.3 Variance | 2.10 (brief) |
| 6.4 Standard Deviation | 2.10 (brief) |
| 6.5–6.6 Z-Scores | — |
| 6.7–6.11 The Normal Distribution and Empirical Rule | — |
| 7.1 Explaining Variation | 3.1 |
| 7.2 Using R to Fit the Group Model | 3.2 |
| 7.3 GLM Notation for the Group Model | 3.3 |
| 7.4 How the Model Makes Predictions | 3.3–3.4 |
| 7.5 Error Leftover From the Group Model | 3.4 |
| 7.6 Graphing Residuals From the Model | 3.4 |
| 7.7 Error Reduced by the Group Model | 3.5 |
| 7.8 Using SS Error to Compare Group to Empty Model | 3.5 |
| 7.9 Partitioning Sums of Squares into Model and Error | 3.10–3.11 |
| 7.10 Using PRE to Compare Two Models | 3.12 |
| 8.1–8.3 Three-Group Models | — |
| 8.4 The F Ratio | 3.13 |
| 8.5 Measures of Effect Size | — |
| 8.6 Modeling the DGP | — (brief in 3.5, 3.13) |
| 8.7 Using Shuffle to Compare Models of the DGP | — |
| 9.1 Using a Quantitative Explanatory Variable in a Model | 3.6 |
| 9.2 Specifying the Model with GLM Notation | 3.7 |
| 9.3 Interpreting Parameter Estimates for a Regression Model | 3.8 |
| 9.4 Comparing Regression Models to Group Models | 3.6–3.8 |
| 9.5 Error from the Model | 3.9 |
| 9.6 Sums of Squares in the ANOVA Table | 3.10 |
| 9.7 Assessing Model Fit with PRE and F | 3.11–3.13 |
| 9.8–9.9 Correlation and Pearson's R | — |
| 9.10 Using Shuffle to Interpret the Slope | — |
| 9.11 Limitations to Keep in Mind | — |

## Related Documents

- [Topic alignment guide](../topic-alignment/topic-alignment-book.md) — traditional intro-stats topics mapped to chapters of all three books
- [Learning objectives](../learning-objectives/learning-objectives.md) — objective-by-objective chapter coverage in ABC/ABCD and XCD
