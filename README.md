# Remote Sensing for Plant Diversity Prediction (R)

This three-day, hands-on course introduces ecologists and environmental data scientists to remote sensing workflows for predicting plant diversity using R. Participants will learn how to source, preprocess, and analyze satellite data, build predictive models, and communicate findings effectively.

## Audience
- Ecologists, botanists, and conservation practitioners working with spatial biodiversity data
- Data scientists interested in environmental applications
- Graduate students seeking practical experience with R-based geospatial analysis

## Prerequisites
- Working knowledge of R (data wrangling, basic plotting)
- Familiarity with GIS concepts and coordinate reference systems
- R 4.2+ with packages: `terra`, `sf`, `tidyverse`, `caret` (or `tidymodels`), and `rasterdiv`
- Optional: basic command-line experience for downloading datasets (e.g., `aria2`, `curl`, or `wget`)

## Learning Outcomes
By the end of the course, participants will be able to:
1. Acquire and preprocess multispectral satellite imagery for vegetation studies.
2. Derive spectral indices (e.g., NDVI, EVI) and texture metrics relevant to plant diversity.
3. Integrate field observations with raster predictors to build species richness models in R.
4. Evaluate and compare predictive models using cross-validation and spatial blocking.
5. Communicate and visualize model outputs (maps, uncertainty, and feature importance).
6. Package analyses into reproducible R Markdown or Quarto reports that can be shared with collaborators.

## Schedule Overview (3 Days)
### Day 1: Foundations of Remote Sensing in R
- Course orientation and data overview
- Accessing satellite data (Sentinel-2, Landsat) with `terra`
- Reprojection, mosaicking, and cloud masking workflows
- Computing spectral indices (NDVI, EVI) and raster statistics
- Lab: Build a reproducible preprocessing script for your study area
- Stretch goal: batch-download recent scenes for a region of interest using command-line tools

### Day 2: Feature Engineering and Model Design
- Linking plot-based plant diversity data with raster predictors using `sf`
- Creating habitat and landscape metrics (texture, fragmentation)
- Exploratory data analysis and collinearity checks
- Modeling species richness with `caret` / `tidymodels` (RF, GBM)
- Lab: Train baseline models and evaluate with k-fold and spatial cross-validation
- Stretch goal: compare model performance across spatial resolutions (10 m vs. 30 m)

### Day 3: Assessment, Mapping, and Communication
- Model diagnostics (variable importance, partial dependence)
- Uncertainty quantification and spatial residual analysis
- Generating prediction maps and tiling large areas
- Exporting outputs (GeoTIFF, map products) and reporting
- Capstone: End-to-end workflow on a chosen region using provided datasets
- Stretch goal: publish an interactive map using `leaflet` or `mapview`

## Deliverables and Assessment
- Daily lab notebooks (.Rmd) demonstrating preprocessing, modeling, and evaluation steps
- Final capstone report (R Markdown or Quarto) summarizing methods, results, and maps
- Optional peer review of capstone reports to practice communicating uncertainty and limitations

## Species Diversity R Markdown Template
- Use `species_diversity.Rmd` as a ready-to-run worksheet on common diversity metrics (richness, Shannon, Simpson, Hill numbers, Bray–Curtis dissimilarity)
- Swap in your own abundance table to reproduce the calculations and plots for your study plots
- Knit the notebook to share interactive HTML summaries or adapt chunks into course labs

## Logistics
- Format: Live online or in-person workshop with guided labs
- Duration: 3 days (6 hours per day, including breaks)
- Software: RStudio or VS Code with R extension; QGIS optional for validation
- Data: Sentinel-2/Landsat imagery, sample plot data, and provided shapefiles
- Support: Slack/Teams channel for Q&A between sessions
- Access: All slides, starter code, and datasets shared via a version-controlled repository

## Instructor Notes
- Provide datasets and starter scripts before Day 1
- Encourage participants to clone/download a template repo containing RMarkdown notebooks
- Ensure cloud masking and reprojection steps are demonstrated live with real data
- Include short daily check-ins to clarify questions on installation, data access, and modeling choices
