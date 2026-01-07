# African Seed Microbiome Analysis

This repository contains comprehensive code and resources for analyzing the microbiome of African seeds, including bacteria, archaea, and fungi. The analysis covers diversity, composition, and functional aspects of the seed microbiome.

## Project Overview

This research project investigates the microbial communities associated with African seeds, examining:
- Alpha and beta diversity patterns
- Taxonomic composition across different microbial groups
- Functional profiling of microbial communities
- Statistical comparisons between genotypes and conditions

## Authors

Oluwatosin Ajibade, Expedito Olimi, Wisnu Adi Wicaksono, Elijah Kolawole Oladipo, Julius. K. Oloke, Olubukola Monisola Oyawoye, Tomislav Cernava, Gabriele Berg

## Abstract

The seed microbiome is essential for plant health, development, and adaptation. This study investigates the microbial communities associated with African seeds, focusing on bacteria, archaea, and fungi in five Nigerian vegetable crops (Amaranthus hybridus, Solanum macrocarpon, Corchorus olitorius, Celosia argentea, and Telfairia occidentalis). The findings reveal diverse microbial communities, with plant species-specific seed microbial signatures for bacterial and fungal communities. The core seed microbiota includes potentially plant-beneficial taxa like Methanobrevibacter, Methylobacterium, Burkholderia-Caballeronia-Paraburkholderia, Bacillus, Paenibacillus, Stenotrophomonas, Pseudomonas, Serratia, Pantoea, Shingomonas, Lactobacillus, Aspergillus, and Fusarium. Random forest classification successfully resolved plant species-specific differences. The research highlights the importance of these microbial communities for plant sustenance in smallholder-dependent food production systems and provides a basis for conserving unique plant genetic resources.

## Repository Contents

### Analysis Scripts
- `African-seed.Rmd`: Main R Markdown file for data analysis and visualization
- `utilities.R`: Utility functions for data processing and analysis
- `plot_hierarchy.R`: Scripts for hierarchical plotting
- `RSCRIPT_parwise.adonis.txt`: Statistical analysis scripts
- `Run_lefse.txt`: LEfSe analysis scripts

### Data Files
- `Archaea_*`: Archaeal microbiome data (tables, taxonomy, metadata)
- `Bacteria_*`: Bacterial microbiome data (tables, taxonomy, metadata)
- `Fungi_*`: Fungal microbiome data (tables, taxonomy, metadata)
- `Archaea_Metadata.csv`: Metadata for archaeal samples
- `Bacteria_metadata.csv`: Metadata for bacterial samples
- `Fungi_Metadata.csv`: Metadata for fungal samples
- `diversity_data.csv`: Diversity metrics data
- `aggregate_top_taxa.txt`: Aggregated top taxa information
- `aggregate_rare.txt`: Rarefaction data

### Analysis Results & Outputs
- `*.tiff`: Figures and visualizations (alpha diversity, beta diversity, PCoA plots, etc.)
- `*.RData`: R workspace files containing processed data objects
- `RF*.csv`: Random Forest analysis results
- `Dunn*`: Statistical test results (Dunn tests)

### Specialized Tools & Functional Analysis
- `FAPROTAX_1.2.10/`: Functional annotation of prokaryotic taxa
- `FUNGuild/`: Fungal functional guild classification
- `uv/`: Additional analysis tools

### Figures and Visualizations
- `Figures/`: Directory containing various analysis figures
- `*.tiff`: Individual figure files for different analyses
- `*.pdf`: Compiled figure documents

## Getting Started

1. **Clone the repository**
   ```sh
   git clone https://github.com/yourusername/African-seed-microbiome.git
   ```

2. **Open the project in R/RStudio**
   Open `African-seed.Rmd` to view and run the analysis.

3. **Install required R packages**
   Make sure you have the following R packages installed:
   - `knitr`
   - `rmarkdown`
   - `phyloseq`
   - `ggplot2`
   - `dplyr`
   - `vegan`
   - `randomForest`
   - `adonis2`
   - And other packages used in your analysis

   Install them in R with:
   ```r
   install.packages(c("knitr", "rmarkdown", "phyloseq", "ggplot2", "dplyr", "vegan", "randomForest"))
   ```

4. **Run the analysis**
   Click the **Knit** button in RStudio to generate the report from `African-seed.Rmd`.

## Key Analyses Performed

- **Alpha Diversity**: Richness, Shannon diversity, and other diversity metrics
- **Beta Diversity**: Community composition differences between samples
- **Taxonomic Composition**: Analysis of bacterial, archaeal, and fungal communities at different taxonomic levels
- **Functional Profiling**: Functional predictions using FAPROTAX and FUNGuild
- **Statistical Comparisons**: Differential abundance analysis, Dunn tests, Adonis tests
- **Random Forest**: Machine learning-based classification and feature selection
- **Core Microbiome**: Identification of consistently present taxa

## Project Structure

```
.
├── African-seed.Rmd
├── README.md
├── .gitignore
├── data/
│   ├── metadata/
│   ├── processed/
│   └── raw/
├── r_objects/
├── results/
│   ├── figures/
│   └── tables/
└── scripts/
    ├── FAPROTAX_1.2.10/
    └── FUNGuild/
```

## Data Description

The repository contains comprehensive microbiome data for three major microbial groups:
- **Archaea**: Archaeal community composition and diversity
- **Bacteria**: Bacterial community composition and diversity
- **Fungi**: Fungal community composition and diversity

Each group includes:
- Taxonomic tables (`Table.txt`, `Taxonomy.txt`)
- Abundance data (`abundance.txt`)
- Richness and diversity metrics
- Statistical test results

## Dependencies

This analysis requires:
- R (>= 4.0)
- RStudio (optional, for interactive development)
- Various R packages (see installation instructions above)

## License

This project is for academic and research purposes only.