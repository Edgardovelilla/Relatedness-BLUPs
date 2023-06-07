# Relatedness & BLUPs: Supplementary Material for Efficient Prediction of Dominance Effects in Large Breeding Populations

## Overview
This repository contains essential supplementary material for the research paper "Efficient Prediction of Dominance Effects in Large Breeding Populations: Unveiling the Power of Mixed-Model Methodology." This valuable resource comprises a comprehensive collection of R functions specifically developed to enhance the research pipeline. These functions support breeding program simulations and genetic evaluations focused on quantitative traits.

## Features

### Breeding Program Simulations
The functions included in this repository enable the simulation of a breeding program for a quantitative trait using stochastic simulation based on an infinitesimal model (Fisher 1918; Bulmer 1980). The simulation incorporates both additive and dominance genetic effects, while assuming that the contribution of epistatic sources of variance is negligible. The simulation process involves the following steps:

1. **Base Population**: Founder individuals are sampled from an ideal random mating base population that exhibits no inbreeding and maintains Hardy-Weinberg linkage equilibrium.

2. **First-Generation Simulation**: Open-pollinated progenies are generated, representing half-sib families. Selection is then conducted based on the performance of the best-performing half-sib families.

3. **Subsequent Generations**: Parents are randomly mated using a half-diallel design. The additive genetic effects are computed based on parental values and the additive Mendelian sampling deviation. Furthermore, an individual's dominance genetic effect, adjusted for the average effect of inbreeding on the mean, is computed following the method described by Hoeschele & VanRaden (1991).

4. **Phenotypic Value Simulation**: Phenotypic values are simulated by incorporating the expected mean phenotypic value in the first generation, as well as additive and dominance effects, inbreeding depression, and environmental factors.

### Genetic Relatedness Matrices
Generate the dominance- and family-relatedness matrices using two approaches:
*	Jacquard's nine condensed coefficients of identity (Jacquard, 1974) which quantify accuratelly the genetic relationships among individuals.
*	Coancestry coefficients based on the approach by Cockerham (1954).

### Predictions
Get the best linear unbiased estimate (BLUE) and best linear unbiased predictor (BLUP) by solving the mixed model equations under an animal model (Henderson, 1950).

## Usage
To use the functions, follow these steps:
* Install R programming language (https://www.r-project.org/) and ensure it is properly set up.
* Clone or download this repository.
* Load the required functions into your R environment using the appropriate import statements.
Refer to the documentation and examples provided within each function to understand the input requirements and usage guidelines.

## References
Bulmer, M. G. (1980). The mathematical theory of quantitative genetics. Oxford Univ. Press, Oxford, UK.   

Cockerham, C.C. (1954). An extension of the concept of partitioning hereditary variance for analysis of covariances among relatives when epistasis is present. Genetics, 39, 859–882.

Fisher, R. A. (1918). The correlation between relatives on the supposition of Mendelian inheritance. Trans. R. Soc. Edin. 52, 399-433.

Henderson, C.R. (1950). Estimation of Genetic Parameters. Annals of Mathematical Statistics, 21, 309-310.

Jacquard, A. (1974). The Genetic Structure of Populations. Springer-Verlag, New York.

Please ensure to appropriately cite the relevant publications and authors mentioned in the description.
Feel free to explore the functions and modify them to suit your specific research needs.
If you have any questions or encounter any issues, please open an issue on this repository.
Note: You can provide additional information such as installation instructions, examples, and a license file within the repository to make it more comprehensive and user-friendly.








