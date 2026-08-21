# Solar Flares and Earth Phenomena

## Overview

This project explores whether solar flare activity is associated with short-term changes in several Earth-based phenomena, including:

- Earthquakes
- Volcanic eruptions
- Global precipitation
- Global temperature anomalies

The goal was not to prove causation, but to test whether measurable statistical relationships appeared between solar activity and terrestrial events over short time lags.

## Data Sources

Data used in this project came from:

- NASA DONKI — Solar flare activity
- USGS — Global earthquake data
- Smithsonian Institution — Volcanic eruption data
- NASA GPM — Global precipitation data
- Berkeley Earth — Global temperature anomaly data

## Methods

The datasets were cleaned and converted into daily observations so they could be compared across a common timeline.

Solar activity was measured using:

- Total solar flare count
- M-class flare count
- X-class flare count
- Estimated solar flare energy output

Each Earth phenomenon was compared with solar activity at lags from 0 to 7 days.

Statistical methods included:

- Pearson correlation
- Spearman correlation
- False Discovery Rate (FDR) correction for multiple comparisons

Precipitation and temperature were analyzed using anomaly values to reduce the influence of normal seasonal variation.

## Key Findings

### Earthquakes
No statistically robust relationship was found between solar flare activity and global earthquake activity.

The strongest M6+ earthquake result occurred at a 3-day lag:

- Pearson r = -0.044
- FDR-adjusted p = 0.0618

### Volcanic Eruptions
No meaningful relationship was detected between solar flare activity and volcanic eruption activity.

The strongest observed correlation was approximately:

- |r| = 0.018

### Precipitation
Precipitation produced the strongest result in the project.

For total solar flare count at a 7-day lag:

- Pearson r = +0.0576
- FDR-adjusted p = 0.0048

For M-class flare count at a 7-day lag:

- Pearson r = +0.0637
- FDR-adjusted p = 0.0012

These relationships were statistically significant but very small and should not be interpreted as evidence of causation.

### Temperature
No statistically significant short-term relationship was detected between solar flare activity and global temperature anomalies.

## Overall Conclusion

Most Earth-system outcomes examined in this project showed no robust short-term relationship with solar flare activity.

Precipitation was the exception, showing a small statistically significant positive association several days after increased solar flare activity.

Because weather data are temporally autocorrelated and correlation does not establish causation, the precipitation result should be considered exploratory and a potential area for further research.

## Project Contents

- `Notebook/` — Python analysis and statistical testing
- `Data/` — Project datasets and processed data. Does Not include precipitation data due to size of the dataset. Code to gather the data is in the Jupyter Notebook
- `Dashboard/` — Interactive Power BI dashboard
- `Presentation/` — Project findings presentation

## Tools Used

- Python
- pandas
- NumPy
- SciPy
- statsmodels
- Matplotlib
- Power BI
- Jupyter Notebook

## Future Improvements

Possible extensions include:

- Time-series models that account for autocorrelation
- Regional precipitation analysis
- Confidence intervals for correlation estimates
- Longer analysis periods
- Other natural Phenomena to analyse