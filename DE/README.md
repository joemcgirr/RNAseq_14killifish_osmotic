## Conserved_and_Diverged_Expression.Rmd
Main notebook summarizing expression patterns across the 14 killifish species.

## PGLS
Perform a mean-variance stabilization on read counts following [Rocke et al 2015](https://doi.org/10.1101/018739). Use transformed counts and perform phylogenetic least squares regression to identify genes showing different expression responses between species.

## Count thresholds
Genes with low expression across samples were dropped from the analysis. The function `filterByExpr` was used on the raw counts matrix. For each `condition_physiology` group (regardless of species), each sample must have a minium count of 10, and a group minimum total count of 100 (/counts_threshold_lisa) or 30 (/counts_threshold_new).


