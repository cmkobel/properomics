# properomics
Link tendencies across multiple omics layers using principal components.


Properomics orders samples on principal components, and correlates the ordering across several omic-layers.

This pipeline is a generalization of the workflow used in https://www.biorxiv.org/content/10.1101/2024.12.05.626740v1


## Workflow

1. Input validation
2. Transform
3. Filter
4. (Optional: Statistics)
5. Principal Component Analysis and sample ordering
6. Correlation across omic-layers


## Input 

Properomics is designed to handle any type of properomic setup. This means that you need at least two independent omic layers. The omic layers can be identical on the molecular level (transcriptomics-transcriptomcs) as long as they're from different sample locations. (Needs more generalization)

### metadata.tsv:

samples (n in N) x factors (f in F)
