# Group Linear non-Gaussian Component Analysis for Neuroimaging

This repository provides codes to implement the proposed algorithms (group LNGCA and non-Gaussian subspace dimension test/estimation) and reproduce the experiment results in the open-access paper published in Computational Statistics and Data Analysis, ["Group Linear non-Gaussian Component Analysis with Applications to Neuroimaging"](https://www.sciencedirect.com/science/article/pii/S0167947322000342/pdfft?md5=729eb4b951b220f68d883acb7c8c8c37&pid=1-s2.0-S0167947322000342-main.pdf). 

## Group LNGCA 
The group LNGCA algorithm, located in file fun_call_group_function.R, concists of three steps (1) Subject level LNGCA (2) Group level PCA/SVD (3) Group level ICA/LNGCA. The first step and third step are achieved using codes supporting the single subject LNGCA ["Linear non-gaussian component analysis via maximum likelihood"](https://www.tandfonline.com/doi/abs/10.1080/01621459.2017.1407772), which are included in file fun_LNGCA.R.

## NonGaussian Subspace Dimension Test
We include the implementation, in file fun_dimension_test.R, for (1) the resampling test for a specific hypothesis (2) the dimension estimation algorithm through binary search using dimension test.

## Simulation Reproduction
The file sim_group_comp_extractoin.R provides all codes to replicate our simulation results.
