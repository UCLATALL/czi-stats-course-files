# CourseKata Learning Goals and Objectives

*Statistics and Data Science: A Modeling Approach*

## High-Level Performance Objective

At the end of the course students will be able to:

> Generate research questions that could be answered with data — whether collected by students or provided to them — and engage in the cycle of data analysis: exploring variation, modeling variation, evaluating their models, and communicating the results of what they have learned from data analysis.

To achieve this high-level objective, students master a wide range of learning objectives, organized under four high-level goals.

## Goals at a Glance

| Goal | Sub-goals | Objectives |
|------|-----------|------------|
| 1. Understand Data | Where data come from; organization of data; purpose of data | 25 |
| 2. Explore Variation | Sources of variation; distributions of data; relationships in data | 33 |
| 3. Model Variation | DATA = MODEL + ERROR; specifying, fitting, and assessing models; predictions and likelihood | 70 |
| 4. Evaluate Models | Sampling distributions; confidence intervals; model comparison with F | 48 |

If you teach a more traditional (non-modeling) course and want to see how these objectives line up with a conventional topic list — descriptive statistics, study design, t-tests, ANOVA, regression, inference — start with the [topic alignment guide](../topic-alignment/topic-alignment-book.md), which maps traditional topics to CourseKata chapters. Goals 1 and 2 correspond roughly to data collection, study design, and exploratory/descriptive statistics; Goal 3 covers statistical models (with the general linear model unifying what is traditionally taught as means, group comparisons, and regression); and Goal 4 covers statistical inference (sampling distributions, confidence intervals, and hypothesis testing framed as model comparison).

## How to Read This Document

Learning objectives are defined by a hierarchical system of high-level goals, sub-goals, and specific objectives:

- **High-level goals** are numbered 1–4 and shown as major sections below.
- **Sub-goals** are numbered 1.1, 1.2, etc., and further divided into fine-grained sub-goals numbered 1.1.1, 1.1.2, etc.
- **Learning objectives** are identified by codes combining letters and numbers: CM1, CM2, etc. The letters abbreviate important words in the sub-goal (e.g., CM = Concepts of Measurement). Codes are unique within the document; the machine-readable [CSV](learning-objectives.csv) also carries a fully numeric ID for each objective (e.g., CM1 = 1.1.1.1).
- **(R)** at the end of an objective indicates it requires effective use of R code.
- The **ABC / ABCD** column shows which chapters of the *Introductory Statistics with R (ABC)* and *Advanced Statistics with R (ABCD)* books address the objective, using the chapter numbering of book version 5 and later (verified against version 7.2). *JNBs* means the objective is addressed in the accompanying Jupyter notebooks rather than book pages.
- The **XCD** column shows the corresponding chapters in *Accelerated Statistics with R (XCD)*. XCD compresses ABCD chapters 1–9 into three accelerated chapters (XCD 1 ≈ ABCD 1–3; XCD 2 ≈ ABCD 4–6; XCD 3 ≈ ABCD 7–9), and its chapters 4–10 are identical in content to ABCD chapters 10–16. Because of that compression, some objectives are trimmed from XCD: a dash (—) means the objective is not substantially addressed there (for example, z-scores, correlation coefficients, the normal distribution as a model of error, the empirical rule, shuffling/simulation before the inference chapters, and path diagrams).
- Objectives marked ***(Part D only)*** (ABCD chapters 13–16; XCD chapters 7–10) appear only in the multivariate chapters. Students in courses using only parts A, B, and C will not encounter these. Wherever possible, multivariate objectives are categorized within the existing goal structure to emphasize the continuity of the modeling approach.

Every objective is aligned to specific assessment items embedded in the book (selected-response questions, R coding exercises, and short-answer items). The [CSV version](learning-objectives.csv) of this document includes the number of assessment items aligned to each objective.

## 1. Understand Data


### 1.1. Understand where data come from


#### 1.1.1. Understand and apply concepts of measurement (CM)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CM1</td><td>Quantify variation in data by assigning numbers or categories to attributes</td><td>2</td><td>1</td></tr>
<tr><td>CM2</td><td>Differentiate quantitative and categorical levels of measurement</td><td>2</td><td>1</td></tr>
<tr><td>CM3</td><td>Recognize and explain the possibility of measurement error when looking at data collection or data visualizations</td><td>2</td><td>—</td></tr>
<tr><td>CM4</td><td>Identify the limitations of measurement, including measurement bias (and mistakes)</td><td>2</td><td>—</td></tr>
<tr><td>CM5</td><td>Define data</td><td>2</td><td>1</td></tr>
</table>

#### 1.1.2. Understand sampling methodology (SM)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>SM1</td><td>Explain that samples are the result of a sampling process and a data generating process (DGP)</td><td>2, 3</td><td>1</td></tr>
<tr><td>SM2</td><td>Define independent, random sampling and explain the consequences of violating independent, random sampling</td><td>2</td><td>—</td></tr>
<tr><td>SM3</td><td>Explain and apply the definition of sampling variation and consider it a possible explanation for observed group differences</td><td>2, 4</td><td>2</td></tr>
<tr><td>SM4</td><td>Recognize that samples (and even random samples) are not perfectly representative of the entire population</td><td>2</td><td>2</td></tr>
<tr><td>SM5</td><td>Recognize that samples are studied in order to find out about the population and the data generating process (DGP)</td><td>2</td><td>2</td></tr>
<tr><td>SM6</td><td>Recognize the limitations of sampling, including sampling bias</td><td>2</td><td>—</td></tr>
</table>

#### 1.1.3. Understand elements of research design (RD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>RD1</td><td>Distinguish outcome variables versus explanatory variables</td><td>2, 3, 4</td><td>1, 2</td></tr>
<tr><td>RD2</td><td>Differentiate observational and experimental studies and recognize the limitations of each</td><td>4</td><td>—</td></tr>
<tr><td>RD3</td><td>Differentiate random sampling and random assignment and explain the advantages of each</td><td>4</td><td>3</td></tr>
</table>

### 1.2. Understand the organization of data


#### 1.2.1. Understand data frames (DF)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>DF1</td><td>Interpret the structure of data: rows (i.e. observations) and columns (i.e. variables) (R)</td><td>2</td><td>1</td></tr>
<tr><td>DF2</td><td>Differentiate and interpret variables versus values in a data set</td><td>2</td><td>1</td></tr>
<tr><td>DF3</td><td>Differentiate and interpret levels of variables</td><td>2</td><td>1</td></tr>
</table>

#### 1.2.2. Manipulate data in a data frame (MD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>MD1</td><td>Write code to perform basic R commands</td><td>1–12</td><td>1–6</td></tr>
<tr><td>MD2</td><td>Create summary variables (R)</td><td>2</td><td>1</td></tr>
<tr><td>MD3</td><td>Aggregate variables across rows to create a new data frame (R)</td><td>2</td><td>1</td></tr>
<tr><td>MD4</td><td>Recode quantitative variables into categorical variables (e.g., using ntile(), boolean variables) (R)</td><td>2</td><td>1</td></tr>
<tr><td>MD5</td><td>Identify and decide how to handle missing data (R)</td><td>2</td><td>1</td></tr>
<tr><td>MD6</td><td>Filter, organize, and manipulate data in a data frame; interpret the results (e.g. arrange(), select()) (R)</td><td>2</td><td>1</td></tr>
</table>

### 1.3. Understand the purpose of data


#### 1.3.1. Imagine data that could answer a question (DQ)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>DQ1</td><td>Generate questions that could be answered with a given data set</td><td>1–12</td><td>1–6</td></tr>
</table>

#### 1.3.2. Generate questions you could ask of data (QD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>QD1</td><td>Evaluate appropriateness of data to specific questions and purposes</td><td>1–12</td><td>1–6</td></tr>
</table>

## 2. Explore Variation


### 2.1. Understand sources of variation


#### 2.1.1. Categorize sources of variation (SV)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>SV1</td><td>Recognize that variation can be divided into explained and unexplained; unexplained variation into real (i.e. a product of the system) or induced; induced variation into measurement error, sampling error, or mistakes</td><td>4</td><td>2</td></tr>
</table>

#### 2.1.2. Understand what it means to explain variation (EV)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>EV1</td><td>Explain and apply an intuitive definition of ‘explaining variation’</td><td>4</td><td>2</td></tr>
<tr><td>EV2</td><td>Identify within and between group variations in a graph</td><td>4</td><td>2</td></tr>
<tr><td>EV3</td><td>Apply the definition of explaining variation to graphs (e.g. scatterplots, faceted histograms)</td><td>4</td><td>2</td></tr>
</table>

#### 2.1.3. Understand correlation, causation, and confounding (CCC)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CCC1</td><td>Recognize that explaining variation does not always mean the relationship is causal</td><td>4</td><td>3</td></tr>
<tr><td>CCC2</td><td>Identify and apply the concepts of confounding variables and the problem of directionality</td><td>4, 8, 9</td><td>3</td></tr>
<tr><td>CCC3</td><td>Differentiate experimental from observational designs; understand which research design can lead to causal conclusions</td><td>4, 8, 9, 10, 11, 12</td><td>3, 4, 5, 6</td></tr>
<tr><td>CCC4</td><td>Recognize that randomness can cause an apparent relationship in data</td><td>4, 8, 9, 10, 11, 12</td><td>3, 4, 5, 6</td></tr>
</table>

### 2.2. Describe distributions of data


#### 2.2.1. Understand concept of distribution (CD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CD1</td><td>Define a distribution as the pattern of variation in a variable or combination of variables</td><td>3</td><td>1</td></tr>
<tr><td>CD2</td><td>Describe a distribution using shape, center, and spread, and reason about the possible causes of a distribution's characteristics</td><td>3</td><td>1</td></tr>
<tr><td>CD3</td><td>Reason about measures of central tendency</td><td>5</td><td>2</td></tr>
</table>

#### 2.2.2. Understand that distributions of data are generated by DGP, which is usually unknown (DGP)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>DGP1</td><td>Recognize that populations are the long-run result of a host of causal processes we call the DGP</td><td>3</td><td>1</td></tr>
<tr><td>DGP2</td><td>Simulate samples of data from a DGP; anticipate what the data may look like (R)</td><td>3, 4, 8, 9, 10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>DGP3</td><td>Generate hypotheses about the DGP based on distributions of data; recognize limitations</td><td>3, 4</td><td>1, 2</td></tr>
<tr><td>DGP4</td><td>Recognize the role of randomness and the law of large numbers in interpreting distributions of data</td><td>3</td><td>—</td></tr>
</table>

#### 2.2.3. Represent univariate distributions in tables and graphs (RUD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>RUD1</td><td>Create and interpret frequency tables and relative frequency tables (e.g., tally) (R)</td><td>3</td><td>1</td></tr>
<tr><td>RUD2</td><td>Create and interpret box plots, histograms, and bar graphs to visualize univariate data (R)</td><td>3</td><td>1</td></tr>
<tr><td>RUD3</td><td>Choose the appropriate visualization to represent a given variable</td><td>3</td><td>1</td></tr>
<tr><td>RUD4</td><td>Create and interpret a five-number summary (i.e., favstats()) (R)</td><td>3</td><td>1</td></tr>
<tr><td>RUD5</td><td>Find and interpret the interquartile range (IQR)</td><td>4</td><td>1</td></tr>
<tr><td>RUD6</td><td>Identify outliers and decide how to handle them</td><td>3</td><td>1</td></tr>
</table>

#### 2.2.4. Interpret tables and graphs of univariate distributions (IUD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IUD1</td><td>Interpret the axes of a histogram: know that frequency is represented on the y axis; variable is represented on the x axis</td><td>3</td><td>1</td></tr>
<tr><td>IUD2</td><td>Interpret bar graphs and understand why shape, center, and spread are not meaningful characteristics for these visualizations</td><td>3</td><td>1</td></tr>
<tr><td>IUD3</td><td>Know the differences and similarities between a frequency histogram and a relative frequency histogram</td><td>3</td><td>—</td></tr>
</table>

### 2.3. Describe relationships in data


#### 2.3.1. Represent bivariate relationships in tables and graphs (RBR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>RBR1</td><td>Create two-way contingency tables (e.g. using tally function) (R)</td><td>4</td><td>1</td></tr>
<tr><td>RBR2</td><td>Create scatterplots, faceted histograms, box plots, jitter plots to visualize bivariate data (R)</td><td>4</td><td>2</td></tr>
<tr><td>RBR3</td><td>Choose the appropriate visualization to represent a bivariate relationship</td><td>4</td><td>2</td></tr>
</table>

#### 2.3.2. Interpret tables and graphs of bivariate relationships (IBR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IBR1</td><td>Interpret bivariate relationship presented in tables, scatter plots, faceted histograms, and boxplots</td><td>4</td><td>2</td></tr>
<tr><td>IBR2</td><td>Visually evaluate the strength of relationships in scatter plots, faceted histograms, box plots</td><td>4, 7, 8, 9</td><td>2, 3</td></tr>
</table>

#### 2.3.3. Represent multivariate relationships in visualizations using faceted scatterplots, fill, size, etc (RMR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>RMR1</td><td>Visualize multivariate relationships, e.g., faceted scatterplots</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

#### 2.3.4. Interpret visualizations of multivariate relationships (IMR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IMR1</td><td>Interpret multivariate relationships represented in visualiations</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

#### 2.3.5. Represent relationships in word equations (WE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>WE1</td><td>Create path diagrams to represent bivariate relationships</td><td>4</td><td>—</td></tr>
<tr><td>WE2</td><td>Write word equations to represent relationships between explanatory and outcome variables</td><td>4</td><td>2, 3</td></tr>
</table>

## 3. Model Variation


### 3.1. Understand data = model + error


#### 3.1.1. Understand concept of statistical models (USM)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>USM1</td><td>Map DATA = MODEL + ERROR in different contexts</td><td>4, 5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>USM2</td><td>Define and use the concept of a statistical model as a function that produces a predicted score for each observation</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>USM3</td><td>Differentiate between the empty model and a more complex model</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>USM4</td><td>Identify the most appropriate model to use based on how variables are measured (e.g., group versus regression models)</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>USM5</td><td>Distinguish between a model of data and a model of DGP</td><td>5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>USM6</td><td>Conceptually explain additive (i.e., main effects) and non-additive (i.e., interaction) models; contrast these models</td><td>14, 15, 16 <em>(Part D only)</em></td><td>8, 9, 10</td></tr>
<tr><td>USM7</td><td>Explain that in an interaction, the relationship between a predictor and an outcome depends on the value of a second predictor</td><td>15, 16 <em>(Part D only)</em></td><td>9, 10</td></tr>
</table>

#### 3.1.2. Understand concept of error (CE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CE1</td><td>Visually intuit/ compare which models or distributions show more error</td><td>5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>CE2</td><td>Define, calculate, and reason about residuals from models</td><td>5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>CE3</td><td>Recognize that residuals aggregate to measures of error</td><td>6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>CE4</td><td>Know that error from the empty model is all of the unexplained variation</td><td>5, 6</td><td>2</td></tr>
</table>

#### 3.1.3. Understand partitioning error (UPE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>UPE1</td><td>Know that sum of squares from the empty model (SS total) can be partitioned into error and model sums of squares</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>UPE2</td><td>Recognize that SS total is determined by the outcome variable and so total variation for an outcome variable will be the same regardless of explanatory variables included in the model</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>UPE3</td><td>Interpret visual representations of SS error, SS model, and SS total from empty, group, and regression models</td><td>7, 8, 9</td><td>3</td></tr>
</table>

#### 3.1.4. Understand how transforming variables can help build models (TV)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>TV1</td><td>Use difference scores to model paired samples (JNBs)</td><td>JNBs</td><td>JNBs</td></tr>
<tr><td>TV2</td><td>Use standardized variables (e.g., z-scores) to compare the strengths of linear relationships between different sets of variables</td><td>6, 9</td><td>—</td></tr>
<tr><td>TV3</td><td>Calculate and interpret Pearson’s R, and estimate correlation coefficients from scatterplots</td><td>9</td><td>—</td></tr>
<tr><td>TV4</td><td>Link transformed variables to visualizations (e.g., scatterplots, linear representations of models)</td><td>9</td><td>—</td></tr>
<tr><td>TV5</td><td>Explain which parameter estimates change and do not change as a function of standardizing variables in a bivariate distribution</td><td>9</td><td>3</td></tr>
<tr><td>TV6</td><td>Explain how and why to transform variables in order to center the predictor</td><td>15 <em>(Part D only)</em></td><td>9</td></tr>
<tr><td>TV7</td><td>Explain what features of a model do and don't change as a result of centering a variable</td><td>15 <em>(Part D only)</em></td><td>9</td></tr>
</table>

### 3.2. Specify models


#### 3.2.1. Write models using GLM notation (GLM)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>GLM1</td><td>Use and interpret GLM notation to represent models of data, the DGP, and sampling distributions</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>GLM2</td><td>Flexibly use GLM notation to represent group and regression models in different contexts</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>GLM3</td><td>Differentiate between variables and parameters in GLM equations</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>GLM4</td><td>Use dummy codes to model multi-group data in GLM</td><td>7, 8</td><td>3</td></tr>
<tr><td>GLM5</td><td>Specify and interpret GLM notation for multivariate models</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

#### 3.2.2. Interpret parameter estimates in context (IPE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IPE1</td><td>Map GLM components to contexts, graph, and word equations</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>IPE2</td><td>Interpret GLM components computationally</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
</table>

### 3.3. Fit models


#### 3.3.1. Understand what it means to fit a model (FM)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>FM1</td><td>Know that fitting a model means to calculate best fitting parameter estimates</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>FM2</td><td>Identify that the mean acts as a balancing point for (error) residuals in a distribution</td><td>5</td><td>2</td></tr>
<tr><td>FM3</td><td>Recognize that the best fitting model minimizes the appropriate measure of error (in this course, sum of squares; SS)</td><td>6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>FM4</td><td>Understand the concept of “overfitting” a model</td><td>8</td><td>—</td></tr>
</table>

#### 3.3.2. Estimate parameters (EP)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>EP1</td><td>Differentiate between parameters and statistics; know why a statistic is our best estimate of a (usually) unknowable parameter</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>EP2</td><td>Estimate parameters for empty models, group models, regression models, multivariate models (i.e., fit models) (R)</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>EP3</td><td>Represent and interpret empty and complex models on scatterplots, histograms, boxplots (e.g. gf_model())</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>EP4</td><td>Map parameter estimates to features of multivariate model visualizations</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

#### 3.3.3. Interpret estimates (IE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IE1</td><td>Interpret model output of lm() for empty, group, and regression models</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>IE2</td><td>Interpret parameter estimates for group and regression models in context</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>IE3</td><td>Write best fitting model based on lm() output</td><td>5, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>IE4</td><td>Interpret parameter estimates for multivariate models (e.g., the output of lm())</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
<tr><td>IE5</td><td>Represent and interpret additive and interaction models on scatterplots, histograms, boxplots (e.g. gf_model())</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

### 3.4. Assess model fit


#### 3.4.1. Use residuals to assess model fit (UR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>UR1</td><td>Recognize that the empty model is made up of all unexplained variation</td><td>5</td><td>2</td></tr>
<tr><td>UR2</td><td>Recognize that a residual from the empty model can be partitioned into error and model</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>UR3</td><td>Identify and interpret residuals on a graph of data for empty, group, and regression models</td><td>6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>UR4</td><td>Plot and interpret distributions of residuals (R)</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>UR5</td><td>Generate and analyze predictions and residuals from a model (R)</td><td>5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>UR6</td><td>Generate, identify, and analyze predictions and residuals from multivariate models</td><td>13, 14 <em>(Part D only)</em></td><td>7, 8</td></tr>
</table>

#### 3.4.2. Quantify aggregate error around a model (AE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>AE1</td><td>Quantify aggregate error as Sum of Absolute Deviations (SAD), Sum of Squares (SS), variance, and standard deviation, and interpret these measures (R; e.g., supernova)</td><td>6</td><td>2</td></tr>
<tr><td>AE2</td><td>Explain how sums of squares are constructed from residuals</td><td>6</td><td>2</td></tr>
<tr><td>AE3</td><td>Recognize the pros and cons of different methods of quantifying error</td><td>6</td><td>2</td></tr>
<tr><td>AE4</td><td>Calculate and interpret z-scores within a distribution or across distributions</td><td>6</td><td>—</td></tr>
<tr><td>AE5</td><td>Interpret and reason about shared variance (covariance) in multivariate relationships (including in visualizations, and ANOVA tables)</td><td>14 <em>(Part D only)</em></td><td>8</td></tr>
</table>

#### 3.4.3. Compare the fit of two models (CF)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CF1</td><td>Use SS, PRE, and F statistic to compare models appropriately</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>CF2</td><td>Calculate (e.g., find ANOVA tables; R) and interpret PRE and F statistic (R)</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>CF3</td><td>Interpret a t distribution and relate the critical t to critical z</td><td>10</td><td>4</td></tr>
<tr><td>CF4</td><td>Interpret PRE similarly across ANOVA models and regression models; know that these two measures express the same thing</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>CF5</td><td>Explain the concept of degrees of freedom</td><td>8, 9</td><td>3</td></tr>
<tr><td>CF6</td><td>Fill in values in ANOVA table; explain the relationships between values of an ANOVA table</td><td>7, 8, 9</td><td>3</td></tr>
<tr><td>CF7</td><td>Interpret F, PRE, p-value, and SS appropriately for multivariate models</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
<tr><td>CF8</td><td>Conduct multivariate model comparisons; Understand what simple model is serving as the basis for comparison (R)</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

#### 3.4.4. Understand and calculate different measures of effect size (ES)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>ES1</td><td>Describe and determine appropriate measures of effect size such as difference of means, PRE, Cohen’s d</td><td>7, 8, 9</td><td>3</td></tr>
</table>

### 3.5 Use models to generate predictions


#### 3.5.1. Make point predictions based on parameter estimates (PE)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>PE1</td><td>Use parameter estimates in functions to make point predictions from the empty, group, and regression models (R)</td><td>5, 6, 7, 8, 9</td><td>2, 3</td></tr>
<tr><td>PE2</td><td>Use multivariate models as functions to make predictions (including interactions)</td><td>13, 14, 15, 16 <em>(Part D only)</em></td><td>7, 8, 9, 10</td></tr>
</table>

### 3.6 Use models to estimate likelihood


#### 3.6.1. Use the normal distribution to model variation (ND)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>ND1</td><td>Explain why the normal distribution may be used to model variation in the DGP/population</td><td>6</td><td>—</td></tr>
<tr><td>ND2</td><td>Identify the features of a normal distribution and use data to construct best fitting normal model of variation (e.g., defined by mean and standard deviation)</td><td>6</td><td>—</td></tr>
</table>

#### 3.6.2. Make likelihood predictions based on theoretical probability distributions (PD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>PD1</td><td>Explain the concept of probability distribution as a model of a random DGP</td><td>6, 8, 9, 10, 11, 12</td><td>—</td></tr>
<tr><td>PD2</td><td>Explain the relationship between a discrete (e.g. data, simulated normal distributions) and continuous probability distribution</td><td>6</td><td>—</td></tr>
<tr><td>PD3</td><td>Use the empirical rule to estimate the likelihood of scores under a normal distribution</td><td>6</td><td>—</td></tr>
<tr><td>PD4</td><td>Use the distribution of data to predict likelihood of future observations falling within a specified range</td><td>6</td><td>—</td></tr>
<tr><td>PD5</td><td>Use the normal distribution to estimate likelihood of future observations falling within a specified range (R)</td><td>6</td><td>—</td></tr>
</table>

## 4. Evaluate Models


### 4.1. Model the distributions of estimates


#### 4.1.1. Understand the concept of sampling distribution (CSD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CSD1</td><td>Explain the concept of a sampling distribution</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD2</td><td>Explain the problem a sampling distribution solves, i.e. that it helps to make sense of a particular estimate given sampling variation</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD3</td><td>Interpret sampling distributions in specific contexts</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD4</td><td>Recognize that sampling distributions can depict the random distribution of any statistic (not just the sample mean) from some DGP</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD5</td><td>Recognize that sampling distributions are imaginary</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD6</td><td>Recognize how and why to break the relationship in bivariate data to model a random DGP (R)</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CSD7</td><td>Recognize the significance and model implications of a DGP in which Beta1 = 0</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
</table>

#### 4.1.2. Understand features of sampling distributions (FSD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>FSD1</td><td>Describe the shape, center, and spread of a sampling distribution of estimates, including SDoM, b0, b1, F, and PRE</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>FSD2</td><td>Explain how the shape/center/spread of population and sample size are related to sampling distributions, and how the population's features will affect shape/center/spread of sampling distributions</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>FSD3</td><td>Define and calculate standard error</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>FSD4</td><td>Identify standard error visually</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
</table>

#### 4.1.3. Construct sampling distributions (R) (SDR)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>SDR1</td><td>Construct and reason about sampling distributions by resampling (bootstrapping), simulation, randomization, and using mathematical probability distributions (R)</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>SDR2</td><td>Be able to predict the center and shape of a sampling distribution depending on the method used to construct it</td><td>10, 11, 12</td><td>—</td></tr>
</table>

#### 4.1.4. Interpret sampling distributions (ISD)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>ISD1</td><td>Calculate and evaluate the likelihood of selecting a random sample with a certain sample statistic, (e.g., a t distribution; calculate a p-value) (R)</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>ISD2</td><td>Identify what questions can and cannot be addressed using sampling distributions; i.e. questions about individual observations require a population distribution whereas questions about samples require a sampling distribution</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
</table>

### 4.2. Use confidence intervals to compare models


#### 4.2.1. Understand confidence intervals (CI)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CI1</td><td>Recognize that just as a fixed DGP could produce a range of estimates, a single estimate could be produced by a range of DGPs.</td><td>10, 11, 12</td><td>4, 5, 6</td></tr>
<tr><td>CI2</td><td>Recognize that a confidence interval represents a range of parameter values that could, with some degree of likelihood, have produced your estimate</td><td>12</td><td>6</td></tr>
<tr><td>CI3</td><td>Define margin of error and be able to find it</td><td>12</td><td>6</td></tr>
<tr><td>CI4</td><td>Recognize how standard error relates to confidence intervals</td><td>12</td><td>6</td></tr>
<tr><td>CI5</td><td>Know that the upper and lower bounds of a confidence interval represent the highest and lowest parameter values beyond which our sample would have been unlikely</td><td>12</td><td>6</td></tr>
</table>

#### 4.2.2. Construct a confidence interval around an estimate (R) (CCI)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>CCI1</td><td>Construct confidence intervals using simulation, bootstrapping, and the mathematical probability distribution (i.e., z, t) for various estimates (e.g., b0, b1) (R)</td><td>12</td><td>6</td></tr>
<tr><td>CCI2</td><td>Explain how level of confidence, sample size, and variance impact the size of a confidence interval</td><td>12</td><td>6</td></tr>
</table>

#### 4.2.3. Interpret a confidence interval (ICI)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>ICI1</td><td>Interpret confidence intervals in regression and grouping models for various estimates (e.g., b0, b1)</td><td>12</td><td>6</td></tr>
<tr><td>ICI2</td><td>Explain why you might reject the empty model when a confidence interval for b1 contains zero</td><td>12</td><td>6</td></tr>
<tr><td>ICI3</td><td>Interpret a confidence interval correctly</td><td>12</td><td>6</td></tr>
</table>

### 4.3. Compare models using the F distribution


#### 4.3.1. Understand F (F)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>F1</td><td>Define F as a measure of the strength of a relationship per parameter used in a model; and as a ratio of variation explained to variation unexplained</td><td>8, 11</td><td>3, 5</td></tr>
<tr><td>F2</td><td>Use simulation to explore which statistics can be modeled with the F distribution. (R)</td><td>11</td><td>5</td></tr>
<tr><td>F3</td><td>Interpret an F distribution, and distinguish the F statistic from the F distribution</td><td>11</td><td>5</td></tr>
<tr><td>F4</td><td>Recognize that the shape of the F distribution depends on the degrees of freedom for model and for error</td><td>11</td><td>5</td></tr>
</table>

#### 4.3.2. Conduct model comparison (MC)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>MC1</td><td>Conduct F tests for ANOVA and regression models in some context for some purpose</td><td>11</td><td>5</td></tr>
<tr><td>MC2</td><td>Identify the region that corresponds to p-value in a sampling distribution of F, PRE, or b1</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>MC3</td><td>Define p-value as the probability of obtaining an F, PRE, or b1 statistic as extreme or more extreme than the one observed given the truth of the empty model</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>MC4</td><td>Explain how the numbers in an ANOVA table are calculated and what they mean</td><td>7, 8, 9, 10, 11</td><td>3, 4, 5</td></tr>
<tr><td>MC5</td><td>Recognize and apply the mathematical equivalent of what the statistical community deems “unlikely”</td><td>6, 10, 11</td><td>2, 4, 5</td></tr>
</table>

#### 4.3.3. Interpret results of model comparison (IMC)

<table>
<tr><th width="80">Code</th><th width="540">Learning objective</th><th width="140">ABC / ABCD</th><th width="140">XCD</th></tr>
<tr><td>IMC1</td><td>Explain what it means to "reject the empty model"</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>IMC2</td><td>Determine which statistics can be used to compare two group or three group models versus an empty model</td><td>7, 8, 10, 11</td><td>3, 4, 5</td></tr>
<tr><td>IMC3</td><td>Recognize the limitations of the F test in a three group model</td><td>11</td><td>5</td></tr>
<tr><td>IMC4</td><td>Explain the relationship between an F test and a t test</td><td>11</td><td>5</td></tr>
<tr><td>IMC5</td><td>Recognize and explain the need for simple effects tests</td><td>11</td><td>5</td></tr>
<tr><td>IMC6</td><td>Use the results of ANOVA tables to make predictions about confidence intervals</td><td>12</td><td>6</td></tr>
<tr><td>IMC7</td><td>Explain the problem of simultaneous comparisons and how it is addressed by the bonferroni correction</td><td>11</td><td>5</td></tr>
<tr><td>IMC8</td><td>Conduct and interpret pairwise comparisons in R</td><td>11</td><td>5</td></tr>
<tr><td>IMC9</td><td>Explain the inherent risk of statisticians’ p hacking; calculate likelihood of p-hacking</td><td>11</td><td>5</td></tr>
<tr><td>IMC10</td><td>Explain and recognize Type I error and why its probability of occurring is never zero</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>IMC11</td><td>Explain the use of an alpha level and how it relates to type I and type II error</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>IMC12</td><td>Explain and recognize Type II error</td><td>10, 11</td><td>4, 5</td></tr>
<tr><td>IMC13</td><td>Use the F statistic to compare models; intuit about effect size based on size of F ratio</td><td>8</td><td>3</td></tr>
<tr><td>IMC14</td><td>Interpret a p-value and link to the assumed Data Generating Process</td><td>10, 11</td><td>4, 5</td></tr>
</table>
