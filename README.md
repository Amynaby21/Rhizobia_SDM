**Phylogeographic distribution and climate-driven predictable habitat suitability of symbiotic nitrogen-fixing bacteria of cultivated grain legumes in Africa: A meta-synthesis**



This repository contains the R Markdown scripts and raw data used to model habitat suitability for current and future scenarios for rhizobia species in Africa using an ensemble Species Distribution Modelling (SDM) approach. The script runs only the pre-processing and modelling workflows, community driver analysis, and projections. For the study, we have used:

\* 477 georeferenced rhizobia isolates from root nodules of 04 legume crops (common bean, soybean, cowpea, and groundnut), 09 sub-Saharan countries (Angola, Eswatini, Ethiopia, Ghana, Kenya, Mozambique, Namibia, Senegal, and South Africa), 11 phylogenetic clusters (16S and 16-23S rRNA), aggregated to 134 sites for community analyses.

\* 09 clusters (lineages) with n >= 10 isolates are modelled, grouped into 03 genera: Bradyrhizobium (04 lineages), Rhizobium (04 lineages), and Martinezella (01 lineage: M. tropici cluster).

\* Ensemble SDMs (biomod2; GLM, GBM, RF, and MAXNET with default algorithm settings; 5-fold cross-validation x 5 repetitions) on 12 predictors (08 WorldClim 2.1 bioclimatic variables, 04 SoilGrids 2.0 soil variables) restricted to ESA WorldCover cropland.

\* Projections: CMIP6 SSP245 and SSP585 for 2050 and 2070. Suitability rasters are on a 0-1000 scale. Habitat is split into core and margin zones with two thresholds frozen on the current climate.

The analysis is split into two R Markdown documents.

\- Com\_analyses.Rmd for community drivers? analysis

\- SDM.Rmd for pre-processing, ensemble modelling, and projections.

Here is the repository layout

| Path | Content |

| scripts |

|| Com\_analyses.Rmd ||

|| SDM.Rmd ||

| data |

|| raw || metadata.csv

To perform these analyses, sufficient disk space for raster writing is required, as well as an internet connection for WordClim and SoilGrids downloads. The ESA Cropland was manually downloaded.





