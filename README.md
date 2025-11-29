# Compound Process Simulation

Interactive R Shiny app for simulating and visualizing the Compound Poisson Process:

$$
S(t) = \sum_{i=1}^{N(t)} X_i
$$

where  
- \(N(t)\) is a Poisson process with rate \(\lambda\)  
- \(X_i\) are i.i.d. Exponential(\(\theta\)) jump sizes  



## Overview

This project allows users to simulate \(S(t)\) at different times and understand how the process changes when the arrival rate (\(\lambda\)) and jump size rate (\(\theta\)) vary.

The Shiny app provides:
- Histograms of \(S(t)\)  
- Adjustable parameters \(\lambda\), \(\theta\), and time \(t\)  
- Interactive sensitivity analysis  

---

##  Impact of Parameters

### 1. Inter-arrival parameter (λ)
- Controls how frequently events occur.  
- Higher λ → more jumps → larger values of S(t).  
- Lower λ → fewer jumps → S(t) has more mass near zero.  

### 2. Jump-size parameter (θ)
- Controls the size of each jump.  
- Larger θ → smaller average jump size → S(t) grows slowly.  
- Smaller θ → bigger jumps → S(t) becomes more spread out.  

In summary:  
- λ affects HOW MANY jumps happen  
- θ affects HOW BIG each jump is

---

## Setup Instructions

### 1. Install R and RStudio

Download and install:

- R: https://cran.r-project.org  
- RStudio: https://posit.co/download/rstudio-desktop/

---

### 2. Install Required Packages

```r
install.packages("shiny")


