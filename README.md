# SEM-based Genetic Nurture Analysis Pipeline

This repository provides a **two-step structural equation modeling (SEM) pipeline** for investigating **genetic nurture effects**, with a focus on **maternal and paternal contributions to offspring outcomes**.

---

## Overview

###  Step 1 – Parent-of-Origin Effects (PoE) Analysis
- Estimates maternal and paternal transmitted and non-transmitted PGS effects on offspring outcomes.  
- Models are fit using robust maximum likelihood (MLR) estimation.  
- Family clustering (e.g., sibling relatedness) is accounted for to obtain robust standard errors.  
- Missing data are handled using Full Information Maximum Likelihood (FIML).  
- Genetic assortative mating is explicitly modeled by estimating covariances among parental PRS.  
- Wald tests compare maternal versus paternal effects for transmitted and non-transmitted components.  

###  Step 2 – Mediation Analysis
- Extends PoE models to test mediating pathways via parental phenotypes or family environmental factors.  
- Uses bootstrapped standard errors to obtain robust confidence intervals for mediated effects.  
- Estimates maternal and paternal mediation pathways in parallel, enabling formal tests of maternal vs. paternal mediation.  
- Explicitly accounts for assortative mating by modelling covariance among parental transmitted and non-transmitted PGS, as well as parental phenotype covariance.  
- Tests differences in maternal vs. paternal mediated effects.  

---

##   Key Features
- **Two-step modular design**: PoE analysis + mediation analysis.  
- **Robust estimation**: MLR with clustered SEs and FIML missing data handling.  
- **Explicit modeling of assortative mating** through PGS and phenotype covariances.  
- **Parent-specific contrasts**: Wald tests (PoE) and mediated effect comparisons (mediation).  
- **Export-ready outputs**: effect estimates, fit indices, R², indirect effects, and statistical tests.  

---

##    Citation
If you use this code or build on this pipeline in your own work, please cite:

> Luo, M., Trindade Pons, V., Gillespie, N. A., & van Loo, H. M. (2025). *Evidence for Genetic Nurture Effects on Substance Use*. **medRxiv**, 2025-08. doi: https://doi.org/10.1101/2025.08.28.25334658 

---
