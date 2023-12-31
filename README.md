# Forecast LA PM2.5 Levels

### Introduction
Climate change is a globally relevant, urgent, and multi-faceted issue heavily impacting many industries and aspects of public life. We choose to explore US Environmental Protection Agency (EPA) dataset: weather, air pollutant, and census data.

### Data

This dataset represents daily air quality measurements in the United States for 2019 and 2020 in EPA’s Air Quality System (AQS, https://www.epa.gov/aqs) database in which both PM2.5 and ozone are measured concurrently. These PM2.5 and ozone concentration data are joined with locational, meteorological, demographic information, and concentrations of other major air quality pollutants when available. All of the data were downloaded from AQS with the exception of four demographic parameters (people of color, low income, linguistically isolated, and less than high school education) which come from EPA’s EJSCREEN tool (https://www.epa.gov/ejscreen). These demographic parameters are at the Census "block group" level (area defined by the Census Bureau that usually has between 600 and 3,000 people) and listed in fractional units for the block group containing the monitor location.

1. **epa/Datathon_EPA_Air_Quality_Demographics_Meteorology_2019.xlsx**
    - Original dataset for Datathon. Has data for 2019 for 50 states.
2. **epa/Datathon_EPA_Air_Quality_Demographics_Meteorology_2020.xlsx**
    - Original dataset for Datathon. Has data for 2020 for 50 states.
3. **data/df_preprocessed.csv**
    - Output from 01_preprocessing. Merged 2019 and 2020 dataset. Filtered to just LA and Riverside. Dropped irrelevant columns such as demographics, geographical data, and data with too many sparse points.