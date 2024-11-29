# Snow algae 18S sequence analysis

This repository contains code detailing the analysis of 18S amplicon sequences from mixed communities of snow algae. 

This code is associated with the publication "Elevated light and CO2 levels increase photosynthetic rates of diverse snow algal communities from the North Cascades" by Brooke L. Weigel, Guadalupe Castillo, Honu K. Pata, Jodi N. Young, and Robin B. Kodner.

# Brief description of methods used in this code
DNA sequences were analyzed in QIIME2, version 2023.9.2 (https://qiime2.org/) (Bolyen et al. 2019). Amplicon sequence variants (ASVs) were generated using DADA2 (Callahan et al. 2016), which included quality control steps such as chimera detection and removal, sequence error elimination, singleton exclusion, and sequence trimming based on per-base-pair sequence quality graphs (forward and reverse reads were trimmed between 20 and 240-250 base pairs). Taxonomy was assigned to representative ASVs using RESCRIPt (Robeson et al. 2020) to build a custom reference taxonomy database of snow algal 18S sequences, as standard reference databases do not contain many snow algae sequences.

# These are the 18S primers used for this project:
  The V4 region (418-420 basepairs) of the small subunit ribosomal gene (18S) 
  Forward primers 454FWD1 5′-CCAGCA(G/C)C(C/T)GCGGTAATTCC-3′
  Reverse primers TAReukREV3 5′-ACTTTCGTTCTTGAT(C/T)(A/G)A-3′
