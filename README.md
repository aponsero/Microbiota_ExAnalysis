# Example of a microbiota analysis

Scripts of an example of microbiota overview analysis. The dataset is composed of 19 mice fecal 16SrRNA amplicon sequencing samples, which were originally published in [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3753973/].

## Requirements

The script requires the following libraries: 

- tidyverse
- microbiome
- mia
- ggpubr
- vegan
- factoextra
- ranacapa
- taxonomizr
- scater
- Maaslin2

## Overview

The script "Data_Check.Rmd" runs classic data sanity check and creates a PhyloSeq object containing the dataset. 
- Comparing expected and observed composition of the Mock community
- Taxonomic annotation quality overview
- Contaminants
- Rarefaction curves

The script "Data_Analysis.Rmd" runs a broad overview analysis.
- Global composition overview
- Alpha-diversity, Richness and eveness overview
- Beta-diversity analysis (Bray-Curtis)
- Beta-diversity analysis (Aitchinson)
- Differential abundance analysis using MaAslin2 (LM)
