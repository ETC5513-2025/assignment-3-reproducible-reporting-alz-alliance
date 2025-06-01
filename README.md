# ETC5513 Assignment 3

## Group 4 - ALZ Alliance
**Group Members:**
* Ayush Pandia - 35613424
* Thuy Ngo - 35776064
* Mohammad Zulkifli Falaqi - 35531916

## About The Project  
- **Topic:** Analysing failed startup business in US and examining the trend

- **Research Question:** Why and when do startups fail?

## Project Output
- `Assignment_3.pdf` - The final project report renderred in PDF
- `docs/index.html` - The reproducible project presentation, which can be accessed directly at [`https://tinyurl.com/ALZ-presentation`](https://tinyurl.com/ALZ-presentation) 

## Project Folder Structure

```
.
├── Assignment_3.qmd                                        # Quarto source file for the main report
├── Assignment_3.pdf                                        # Final Rendered PDF for main report
├── docs/                                                   # Folder for the project presentation slides
│   ├──index.qmd                                            # Quarto source file for presentation slides
│   ├──index.html                                           # Rendered HTML presentation slides
|   ├──styles.css                                           # CSS setting file for additional styling in preseentation slides
|   ├──images/                                              # Additional images folder used in presentation slides
|   └──index_files/                                         # Folder that contains resources and files that are required by the index.HTML file 
├── data/                                                   # Folder for dataset used in this project
│   ├── Finance_and_Insurance.csv                           # Raw data for Finance and Insurance sector
│   ├── Food_and_services.csv                               # Raw data for Food and Service sector
│   ├── Health_Care.csv                                     # Raw data for  Healthcare sector
│   ├── Information_Sector.csv                              # Raw data for Information sector
│   ├── Manufactures.csv                                    # Raw data for Manufactur sector
│   ├── Retail_Trade.csv                                    # Raw data for Retail Trade sector
│   ├── startup_combined.csv                                # Processed combined data for all sector
│   └── Startup_Failures_overall.csv                        # Processed data for failures overall
├── bibliography/                                           # Folder that contains the bibliographic references and citation files used
├── _extensions/                                            # Quarto-report-template extensions folder used in this project report
├── images/                                                 # Main images folder used in this project
├── renv/                                                   # renv environment files for reproducibility
├── renv.lock                                               # Exact R package versions for reproducibility
├── .Rprofile                                               # R session configuration
├── .gitignore                                              # Files and directories to exclude from version control
├── assignment-3-reproducible-reporting-alz-alliance.Rproj  # RStudio project file
├── AACSB.png                                               # AACSB accredited Logo, generated from monash-report-template
├── AMBA.png                                                # AMBA accredited Logo, generated from monash-report-template
├── EQUIS.png                                               # EQUIS accredited Logo, generated from monash-report-template
├── MBSportrait.jpg                                         # Monash Business School Logo, generated from monash-report-template
├── monash2.png                                             # Monash University Logo, generated from monash-report-template
└── README.md                                               # This README file
```

## Reproducibility Setup

This project uses the [`renv`](https://rstudio.github.io/renv/) package to manage dependencies and ensure a reproducible environment. 

To set up the project environment using `renv` in your Rstudio, follow these steps:

1. Install renv (if you haven't already):
```r
install.packages("renv")
```

2. Clone the repository to your local machine:
```r
git clone https://github.com/ETC5513-2025/assignment-3-reproducible-reporting-alz-alliance.git
```

3. Once you are in the project directory, you need to activate `renv`:
```r
library(renv)
renv::activate()
```

4. Restore the environment by installing the required packages specified in the renv.lock file, run:
```r
renv::restore()
```