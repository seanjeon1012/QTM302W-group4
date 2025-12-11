# QTM302W: Exploratory Data Analysis on Quarterly Macroeconomic Indicators
### Names and Affiliations
Laura Wang, Sean Jeon, Yuting Chen, Kari Zhou
* Emory University Department of Quantitative Theory & Methods (QTM)

### Project Intro/Objective
This project performs an exploratory analysis of the FRED-QD (Federal Reserve Economic Data – Quarterly Data) dataset to understand how key U.S. macroeconomic indicators evolved from 2000 to 2025.
   
### Methods Used
* Descriptive Statistics
* Trend visualization
* Correlation Analysis
* Linear regressions
* Time-Series Visualization

### List of Platforms/Languages
* R 
* libraries: ggplot

## Project Description

### Our goals are to:
1. Investigate the evolution of GDP and its major components (consumption, investment, government spending, trade) and how they contribute to long-run economic performance.
2. Identify housing indicators as potential leading signals of broader economic shifts.
3. Examine policy impacts, particularly interest rates and government spending, on investment and economic cycles.

### Models and Visualization Techniques: 
Our analysis begins by establishing a statistical snapshot of the economy, summarizing central tendencies and volatility for variables such as real GDP, disposable income, federal funds rate, consumer sentiment, and the house price index. We then visualize temporal dynamics using line charts that highlight structural breaks and crisis periods, and decompose GDP into its major components to understand how their relative shares have shifted over time. Stacked area plots and proportion calculations allow us to track changes in economic composition, while time-filtered comparisons help contextualize behavior before, during, and after key economic disruptions.

### Challenges:
A key limitation of the analysis is the relatively small sample size that results from relying on quarterly data, which restricts statistical power and the ability to capture short-term fluctuations. Additionally, because the event time is used as a sharp cutoff, the regression discontinuity approach can detect differences in housing activity before and after major shocks but cannot capture behavioral shifts occurring during the shock itself. Finally, the analysis focuses primarily on the purchasing power of households able to buy homes, which means it does not account for changes experienced by the homeless population or renters, groups that may be significantly affected by major economic disruptions in the United States.

### Future Directions:
Future work could incorporate additional income-related metrics, such as changes in employment, unemployment rates, and wages, to better understand how financial conditions shape patterns in housing activity. Another promising direction is to examine how major economic shocks alter the consumption behavior of individuals with home loans, offering insight into mortgage-related financial stress. Expanding the dataset to include homelessness statistics and renter behavior would also help capture the experiences of populations who do not own homes but are nonetheless deeply affected by economic downturns. These extensions would provide a more comprehensive understanding of how housing markets and vulnerable groups respond to large-scale economic shocks.

## Getting Started

1. Clone this repo
```bash
git clone https://github.com/Lauraleyao/QTM302W-group4.git
cd QTM302W-group4
```
3. Raw Data is being kept [here](data/2025-09-QD.csv) within this repo.
    
4. Data processing/transformation scripts are being kept [here](data/EDA_notebook.Rmd)

## Directory Structure
```bash
QTM302W-group4/
│
├── data/
│ └── 2025-09-QD.csv # Raw FRED-QD dataset
│
├── EDA_final.Rproj # RStudio project file
├── EDA_notebook.Rmd # Main analysis notebook (RMarkdown)
├── activate.R # renv environment activation script
├── renv.lock # Package version lockfile for reproducibility
├── settings.json # R project / environment settings
│
└── README.md # Project documentation
```

## Contact Info
For questions, please contact:

* Laura Wang - laura.wang@emory.edu
* Sean Jeon - sean.jeon@emory.edu
* Yuting Chen - yuting.chen@emory.edu
* Kari Zhou - kari.zhou@emory.edu
