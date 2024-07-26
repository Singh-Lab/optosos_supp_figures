# optosos_supp_figures
Code to generate supplementary figures for optos paper. First run preprocess.ipynb (1+ hour) and then supplement_figures.Rmd. Requires approximately 3.5GB of harddrive space because of background phosphoproteome generation. Intermediate files are stored in "out" directory and can be deleted once figures are generated. The large figure (denogram/heatmap/z-score) needs to be screenshoted from RStudio because aligment is somewhat dependent on screen resolution. 

# Tested on

python3 version 3.10.12

R version 4.4.1

Rstudio 2024.04.2 Build 764

# Requirements

## Jupyter

## Python

python-calamine 

pandas

biopython

numpy

requests

tqdm

mpire

scipy

statsmodels

statistics

xlsxwriter

## R

readr

ggplot2

mclust

ggdendro

tidyverse

tibble

vegan

dendextden

colorspace

xlsx

# File Descriptions
input/early_fly_proteome.fasta : fasta file of expressed proteins in fly embryo

input/uniprotIDs_fly_homologs_non_transmembrane_johnson_kinases.xlsx : human orthologs of expressed kinases in fly embryo

input/siteQuant_optosos10m_fracnofrac_combined_no_scan_scrambling_motifsuniquepaste.xlsx : Optosos dataset

preprocess.ipynb : Jupyter notebook to generate all raw data required to make figures. Reads optosos dataset, matches phosphopeptides to kinases, and performs enrichment analysis

supplement_figures.Rmd : R Studio markdown file to generate figures in supplement
