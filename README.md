# Remote Sensing for Plant Diversity Prediction (R)

This hands-on module introduces students to remote sensing workflows for **predicting plant diversity using R**. Participants will learn how to source, preprocess, and analyse satellite data, build predictive models, and communicate findings effectively.

This topic is designed as the **final chapter of the Advanced Remote Sensing course**  
(see main course page: https://eol.pages.cms.hu-berlin.de/geo_advrs/syllabus.html).

---

## Audience

- Bachelor students seeking practical, hands-on experience with **R-based geospatial analysis**.

## Prerequisites

- Working knowledge of R (data wrangling, basic plotting).
- Familiarity with GIS concepts and coordinate reference systems (CRS).
- R 4.2+ with packages:

```r
install.packages(c(
  "terra",
  "sf",
  "tidyverse",
  "caret",      # or tidymodels if preferred
  "rasterdiv"
))

