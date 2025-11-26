# Remote Sensing for Plant Diversity Prediction (R)

This hands-on course introduces students to remote sensing workflows for predicting plant diversity using R. Participants will learn how to source, preprocess, and analyze satellite data, build predictive models, and communicate findings effectively. As this is the last chapter (Topic of our Adcance remte sensing course (https://eol.pages.cms.hu-berlin.de/geo_advrs/syllabus.html))

## Audience
- Bachelor students seeking practical experience with R-based geospatial analysis

## Prerequisites
- Working knowledge of R (data wrangling, basic plotting)
- Familiarity with GIS concepts and coordinate reference systems
- R 4.2+ with packages: `terra`, `sf`, `tidyverse`, `caret` (or `tidymodels`), and `rasterdiv`

## Learning Outcomes
By the end of the course, participants will be able to:
1. understand what are the diversity metrics and how to calculate them.
1. Acquire and preprocess multispectral satellite imagery for vegetation studies.
2. Derive spectral indices (e.g., NDVI, EVI) and specture divesity metrics and texture metrics relevant to plant diversity.
3. Integrate field observations with raster predictors to build species richness models in R.
4. Evaluate and compare predictive models using cross-validation and spatial blocking.
5. Communicate and visualize model outputs (maps, uncertainty, and feature importance).

## Schedule Overview (3 weeks, 2hours per week)
### Week 1: Calculate species divesity in R
- Course orientation and data overview
- Cumpute speceis divetsity metrics 
- Computing spectral indices (NDVI, EVI) and raster statistics
- Lab: Build a reproducible preprocessing script for your study area

### Week 2: Feature Engineering and Model Design
- Linking plot-based plant diversity data with raster predictors using `sf`
- Creating habitat and landscape metrics (texture, fragmentation)
- Exploratory data analysis and collinearity checks
- Modeling species richness with `caret` / `tidymodels` (RF, GBM)
- Lab: Train baseline models and evaluate with k-fold and spatial cross-validation

### Week 3: Assessment, Mapping, and Communication
- Model diagnostics (variable importance, partial dependence)
- Uncertainty quantification and spatial residual analysis
- Generating prediction maps and tiling large areas
- Exporting outputs (GeoTIFF, map products) and reporting
- Capstone: End-to-end workflow on a chosen region using provided datasets

## Deliverables and Assessment
- Weekly lab notebooks (.Rmd) demonstrating preprocessing, modeling, and evaluation steps
- Final capstone report (R Markdown) summarizing methods, results, and maps

## Logistics
- Format: In-person workshop with guided labs
- Duration: 3 days (6 hours per day, including breaks)
- Software: RStudio; QGIS optional for validation
- Data: Sentinel-2/Landsat imagery, sample plot data, and provided shapefiles

## Instructor Notes
- Provide datasets and starter scripts before Day 1
- Encourage participants to clone/download a template repo containing RMarkdown notebooks
- Ensure cloud masking and reprojection steps are demonstrated live with real data
