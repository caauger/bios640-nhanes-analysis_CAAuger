# BIOS 640 - NHANES Analysis

Coursework repository for BIOS 640 (Introduction to Health Data Science
Methods), McGill University. The project explores demographic and blood
pressure data from the National Health and Nutrition Examination Survey
(NHANES), using R Markdown for reproducible reporting.

## Repository structure

| Folder | Contents |
|---|---|
| `data/` | Raw input datasets: the cleaned NHANES extract and a small longitudinal diet dataset. |
| `figures/` | Figures exported from the analysis reports as `.png`. |
| `reports/` | R Markdown sources and their rendered outputs (HTML and PDF). |
| `dashboard/` | The `flexdashboard` source and its rendered HTML. |

## Reproducing the outputs

1. Clone the repository.
2. Open `bios640-nhanes-analysis.Rproj` in RStudio. This sets the working
   directory to the project root, which every file path depends on.
3. Install the required packages:

```r
install.packages("pacman")
pacman::p_load(here, rio, tidyverse, forcats, scales, cowplot,
               ggpubr, DT, flexdashboard, knitr, kableExtra)
```

4. Knit any `.Rmd` file in `reports/` or `dashboard/`.

All file paths are built with `here()`, so the code runs from any location
as long as the project is opened through the `.Rproj` file.

## Data source

Centers for Disease Control and Prevention (CDC), National Center for Health
Statistics (NCHS). National Health and Nutrition Examination Survey.
Hyattsville, MD: U.S. Department of Health and Human Services.
