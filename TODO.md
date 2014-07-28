## Data Structures

1. $B$ - set of biofilms
1. $N_b = |B|$ - number of biofilms such as 100
1. $C$ - set of cells comprising biofilm i
1. $N_c =|C|$ - number of cells in a biofilm such as 200
1. Cells $S \subseteq C$ represent the initial propagule size and these always compete to reproduce until the fixed number of cells per biofilm of $N_c$ is produced
1. A minimum of $F \in \mathbb{N}$ functions must be present within a given biofilm for the biofilm to be viable
1. Each c in C has a genome of length 3200
1. Each gene is 20 bases in length. This requires the definition of particular sequences such as "01010101010101111101" which are necessary in order to perform one of the F functions
1. The contribution of a single gene to survival probability is determined by a non-linear function applied to the distance between a given gene and its optimal form
1. Genes are potentially negatively regulated as determined by the presence vs absence of tags, which are like promoters, of length 6
1.

## Algorithm

Genes: p_i
Cells: (p_1,p_2,...p_n) byte string represents genome, genome contains tags
Biofilms: fitness f = \prod_i p_i - \alpha/N \sum_j g(p^j)
i runs over components of the overall phenotype
j runs over individuals
g is a function that favors specialists

## Code



## Figures

1. functions per cell vs heterogeneity
1. spore size vs time
