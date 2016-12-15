Multiple Factor Analysis Using R
========================================================
author:Saurabh Belsare, Ankush Desai, Jieun Kim and Allen Tang
date: 2016-12-14
autosize: true
width: 1400
height: 1100

Introduction
========================================================

**MFA Package**
- The package `"mfa"` implements a statistical multivariate technique called Multiple Factor Analysis (MFA)

- In addition to the main `"mfa"` function, it provides a set of complementary functions and methods to compute summaries of eigenvalues, contributions, coefficients to study the between-table structure (both $R_V$ and $L_g$), and bootstrapping to estimate the stability of the compromise factor scores.



- For visualization, the package includes functions for five types of plots:
  + a bar-chart for the eigenvalues,
  + a scatterplot of the common factor scores,
  + a scatterplot of the partial factor scores by block and by observation,
  + a scatterplot of the loadings of given dimensions (i.e., components), and
  + a bar-chart for bootstrap ratios.


- A Shiny App is available for an interactive visualization.

Main Function: Creating a `mfa` object
========================================================
The first step is to create a `"mfa"` object with the function `mfa()`:


```r
mymfa <- function(data, sets, supplData, ncomps = NULL, center = TRUE, scale = TRUE)
```

This is the main mfa function that implements all the calculations for performing the Multiple Factor Analysis. The function takes six arguments:

- `data`: the input data, which contains only the assessor inputs,
- `sets`: the column number list demarcating columns for each assessor,
- `supplData`: the list of supplementary data for an additional factor analysis,
- `ncomps`: the number of components for the MFA,
- `center`: a boolean flag which decides whether to center the data,
- `scale`: a boolean flag which decides whether to scale the data.

Main Function: return value of mfa
========================================================
The function returns an object of type `mfa` that contains a list containing all the output information computed by the MFA analysis. It includes:

- **Main Output**: the eigenvalues, compromise factor scroes, matrix loadings, and contributions (by observation, variable, and table);
- **Additional information**: labels, column names of the data, sets, bootstrap ratios, and the number of components;
- **Supplementary Output**: eigenvalues, compromise factor scores, matrix loadings, and the number of components.


Complementary Functions
=======================================================
## Print basic information about mfa object
The package provides a print method to display basic information about mfa object: the numbers of blocks and components.























```
Error in library("MFAg") : there is no package called 'MFAg'
```
