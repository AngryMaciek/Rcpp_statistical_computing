# Maciej Bak
# Swiss Institute of Bioinformatics

This is a very small repository that presents the libraries needed for efficient statistical computing in R interfacing to C++.

This software is tested on R version 3.5.1

Required R libraries:
* tictoc
* Rcpp
* numDeriv

This repository contains six files:
* README.md (this file)
* tests.R - the executable R script with example calls of C++ functions
* tests.cpp - C++ functions that call optimization-related algorithms
* zeroin.c - C routine underlying R code for root finding of a single-argument function
* modified_optim.c - modified version of the C file underlying R code with a method to minimize a given multivariate function

These libraries and functions should be enough to implement complex Bayesian models, fit the parameters efficiently and optimize the runtime on big datasets. Functions' logic and interfaces are described within the files above.