# Advanced Data Analysis with R

## NUSC Summer School 2025

![NUSC Summer School Banner](https://via.placeholder.com/800x200)

Welcome to the Advanced Data Analysis with R workshop for the NUSC Summer School 2025! This repository contains all the materials needed to master statistical analysis, visualisation, and modelling with R.

## Workshop Overview

This workshop comprehensively explores advanced data analysis techniques using R and its ecosystem. Participants will learn statistical modelling, data visualisation, and machine learning implementation in R, emphasising real-world applications.

### Learning Objectives

By the end of this workshop, participants will be able to:

- Apply advanced statistical methods to analyse complex datasets
- Create publication-quality visualizations with ggplot2
- Implement various modelling techniques, including regression, classification, and clustering
- Perform reproducible research using R Markdown
- Master data manipulation with tidyverse packages
- Develop interactive dashboards with Shiny

## Prerequisites

- Basic understanding of R programming
- Familiarity with fundamental statistical concepts
- Experience with data manipulation and basic plotting in R
- A laptop with R (4.1+) and RStudio installed

## Workshop Schedule

### Day 1: Advanced Data Manipulation and Visualisation
- 09:00 - 10:30: Data Wrangling with dplyr, tidyr, and purrr
- 10:45 - 12:15: Advanced Data Visualisation with ggplot2
- 13:30 - 15:00: Creating Interactive Visualisations with plotly
- 15:15 - 16:45: Reproducible Research with R Markdown

### Day 2: Statistical Modelling
- 09:00 - 10:30: Linear and Generalised Linear Models
- 10:45 - 12:15: Mixed-Effects Models for Hierarchical Data
- 13:30 - 15:00: Time Series Analysis and Forecasting
- 15:15 - 16:45: Bayesian Analysis with Stan

### Day 3: Machine Learning in R
- 09:00 - 10:30: Machine Learning with tidymodels
- 10:45 - 12:15: Feature Engineering and Model Tuning
- 13:30 - 15:00: Building Interactive Applications with Shiny
- 15:15 - 16:45: Final Project and Group Presentations

## Setup Instructions

### Option 1: Using RStudio (Recommended)

```r
# Install required packages
install.packages(c("tidyverse", "rmarkdown", "shiny", "plotly", 
                  "lme4", "forecast", "rstan", "tidymodels"))
```

### Option 2: Using RStudio Cloud

You can work with R in the cloud without any local installation:

1. Visit [Posit Cloud](https://posit.cloud/) (formerly RStudio Cloud)
2. Create a free account or log in
3. Create a new project
4. In the console, run:
   ```r
   # Clone this repository
   system("git clone https://github.com/nusc-summer-school/advanced-data-analysis-r.git")
   setwd("advanced-data-analysis-r")
   
   # Install required packages
   source("install-packages.R")
   ```

### Option 3: Using Docker

```bash
# Clone this repository
git clone https://github.com/nusc-summer-school/advanced-data-analysis-r.git
cd advanced-data-analysis-r

# Run the Docker container with RStudio
docker pull rocker/verse
docker run -d -p 8787:8787 -v $(pwd):/home/rstudio/workshop -e PASSWORD=workshop rocker/verse
```

Then visit http://localhost:8787 in your browser (login with username: rstudio, password: workshop)

## Repository Structure

```
advanced-data-analysis-r/
├── data/                   # Datasets used in the workshop
├── examples/               # Example R scripts and notebooks
├── exercises/              # Hands-on exercises
│   ├── day1/
│   ├── day2/
│   └── day3/
├── presentations/          # Slide decks in PDF format
├── solutions/              # Exercise solutions
├── shiny-apps/             # Interactive Shiny applications
├── rmarkdown/              # R Markdown templates and reports
├── install-packages.R      # Script to install required packages
└── README.md               # Workshop information
```

## Datasets

This workshop uses the following datasets:

1. **Gapminder**: Global development indicators for countries over time
2. **NYC Flights**: Data on flights departing NYC in 2013
3. **Palmer Penguins**: Size measurements for three penguin species
4. **COVID-19 Time Series**: Global case counts for time series analysis

All datasets are included in the `/data` directory or will be loaded from R packages.

## Resources

### Recommended Reading

- Wickham, H., & Grolemund, G. (2017). R for Data Science. O'Reilly Media.
- Kuhn, M., & Johnson, K. (2019). Feature Engineering and Selection: A Practical Approach for Predictive Models. CRC Press.
- Xie, Y., Allaire, J.J., & Grolemund, G. (2018). R Markdown: The Definitive Guide. CRC Press.

### Online Resources

- [R for Data Science](https://r4ds.had.co.nz/)
- [Tidyverse Documentation](https://www.tidyverse.org/)
- [RStudio Cheatsheets](https://www.rstudio.com/resources/cheatsheets/)
- [Statistical Tools for High-Throughput Data Analysis](http://www.sthda.com/)

## Instructors

- **Dr. Emily Rodriguez** - Data Science Lead, Google Research
  - [GitHub](https://github.com/) | [LinkedIn](https://linkedin.com/)

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

We thank all contributors and the NUSC Summer School organizing committee for making this workshop possible.

---

For questions or additional information, don't hesitate to get in touch with us at info@nuscsummerschool.edu
