# Importance-Sampling Techniques for Variance Reduction

A Fall 2022 AMS 553 group project comparing importance sampling, stratified sampling, and stratified importance sampling for Monte Carlo integration.

## Problem

The project estimates

$$
\int_0^1 \frac{e^{-x}}{1+x^2}\,dx
$$

and studies how alternative sampling designs change estimator variance relative to uniform Monte Carlo sampling.

## Methods and findings

The report develops the estimators theoretically and evaluates them with repeated simulation:

- classical importance sampling with several proposal densities;
- equal-width stratification with 4, 10, and 50 strata; and
- stratified importance sampling combining both ideas.

In the reported experiment, proposal densities shaped more closely to the integrand substantially reduced variance. Equal-width stratification produced still larger reductions as the number of strata increased, and the combined estimator achieved the greatest reduction among the tested designs. These percentages are specific to the selected integrand, proposals, allocation rules, and simulation settings; they are not universal performance guarantees.

## Repository contents

- `AMS 553 Project.Rmd` — R simulation and figures
- `presentation.pdf` — slides
- `report.pdf` — final report

## Contributors

Kai Li, Wenbo Du, Zhe Zhou, and Zeyu Dong.
