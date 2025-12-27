# Water Shutoffs, Race, and Income in Detroit

An analysis of racial and economic disparities in residential water service disconnections in Detroit (2010–2017).

## Overview

Detroit's water shutoff crisis has raised critical questions about environmental justice and equitable access to essential services. This project examines whether race or income is a stronger predictor of which neighborhoods experience the highest rates of water disconnection.

## Key Findings

- **Race matters more than income**: The correlation between Black population share and shutoffs (r = 0.41) is substantially stronger than the correlation with median income (r = 0.08)
- **Persistent disparities**: Tracts with ≥75% Black residents consistently experience ~2x the shutoff rate of other tracts throughout the study period
- **Income is not protective**: Above-median income tracts do not have meaningfully lower shutoff rates
- **Structural inequality**: Patterns suggest systemic factors beyond household ability to pay

## Visualizations

The analysis includes five figures:
1. Shutoffs vs. Black population share (cross-sectional)
2. Shutoffs vs. median income (cross-sectional)
3. Joint relationship: race, income, and shutoffs
4. Time series by income group
5. Time series by racial composition

## Data

The analysis combines:
- **Water shutoff records**: Administrative data on service disconnections (2010–2017)
- **American Community Survey**: Tract-level demographics

**Note**: Data files are not included in this repository. The analysis requires:
- `Data/MI_acs_tract_10_17.rds`
- `Data/si_1017_cleaned.dta`

## Files

```
├── detroit-water-shutoffs-analysis.Rmd   # Main R Markdown analysis
├── Data/                                  # Data directory (not tracked)
├── README.md                              # This file
├── .gitignore                             # Git ignore rules
└── LICENSE                                # MIT License
```

## Requirements

- R (≥ 4.0)
- R packages:
  - `tidyverse`
  - `lubridate`
  - `weights`
  - `foreign`
  - `readstata13`
  - `tidycensus`

Install required packages:

```r
install.packages(c("tidyverse", "lubridate", "weights", "foreign", "readstata13", "tidycensus"))
```

## Usage

1. Place data files in the `Data/` subdirectory
2. Open `detroit-water-shutoffs-analysis.Rmd` in RStudio
3. Knit to HTML or PDF

## Context

This analysis contributes to ongoing debates about water affordability and environmental justice in Detroit. For background, see:
- [We The People of Detroit](https://www.wethepeopleofdetroit.com/)
- [Food & Water Watch reports on Detroit water](https://www.foodandwaterwatch.org/)

## Acknowledgments

This analysis was completed as part of the *Data Analysis for Policy Research using R* course at Columbia University, taught by **Prof. Harold Stolper**.

## License

MIT License - see [LICENSE](LICENSE) for details.

## Author

Pranav Mehta
