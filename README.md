# Redding-Water-Quality-Analysis

## Introduction
In the serene expanses of Redding, California, where nature's beauty intertwines with the ever-present specter of wildfires, the community finds itself at the intersection of environmental resilience and burgeoning challenges. The recent escalation in the frequency and intensity of wildfires has not merely been a distant occurrence but a palpable reality that hovers over the city. Although the average distance of these fires has exhibited an exponential retreat, the tendrils of their impact persist, raising crucial questions about the implications for Redding's environment and, notably, its water quality.

## Purpose
The purpose of this project is to explore the intricate relationships between wildfires, air quality, and water quality in Redding, California. By delving into the less-explored repercussions on water quality, the analysis seeks to unravel the complex dynamics of the aftermath of wildfires on the city's lifeblood—the water supplies. The urgency of this study is underscored by recent events, emphasizing the need for proactive measures to safeguard both the environment and public health.

## Methodology
4.	Water Quality Analysis
•	Overview: Utilizing the smoke estimate dataset and the wildfires dataset from the first step, this analysis aims to address the hypothesis regarding the correlation between wildfires and water quality in Redding, California.
•	Steps:
•	Downloaded the required water quality dataset from data.cnra.ca.gov to initiate the analysis.
•	Computed the smoke estimate for each fire as outlined in the third step of the methodology.
•	Generated maps illustrating the geographical distribution of wildfires and field results of water analysis to provide a visual overview.
•	Processed the water data, retaining essential information including sample_date, parameter, and fdr_result values.
•	Plotted the distance of fires from Redding across years and introduced a trend line to reveal any discernible patterns.
•	Constructed dual-axis plots for key water quality parameters (Water Temperature, pH, Turbidity, and Specific Conductance) against the calculated Smoke Estimate.
•	Findings:
•	Produced graphical representations showcasing correlation and trend lines to interpret the results.
•	Concluded the hypothesis regarding the potential impact of wildfires on water quality by analyzing trends in both wildfires and water parameters.
•	Importance: This step contributes to a holistic understanding of the interplay between wildfires, smoke estimates, and water quality. By visualizing trends and correlations, the analysis sheds light on potential connections between these factors in the Redding region.


## License
The dataset is made available under the [Creative Commons License](https://creativecommons.org/licenses/by/4.0/).

## Data Sources
The project relies on the [water quality dataset](https://data.ca.gov/dataset/water-quality-data/resource/b24d85ed-f88a-4d34-bdf1-812560c4b488) of California. This dataset contains field results that is surveys of water analysis done in the Shasta county.

## Data Description

| Name                  | Type      | Description                                               |
|-----------------------|-----------|-----------------------------------------------------------|
| station_id            | Integer   | Identification code for the station                        |
| station_name          | String    | Name of the station                                       |
| station_number        | String    | Unique number assigned to the station                      |
| full_station_name     | String    | Full name of the station                                   |
| station_type          | String    | Type of station (e.g., Surface Water)                      |
| latitude              | Float     | Latitude coordinates of the station                        |
| longitude             | Float     | Longitude coordinates of the station                       |
| status                | String    | Status of the station (e.g., Public, Review Status Unknown)|
| county_name           | String    | Name of the county where the station is located            |
| sample_code           | String    | Code assigned to the sample                                |
| sample_date           | String    | Date and time of the sample                                |
| sample_depth          | Integer   | Depth of the sample                                        |
| sample_depth_units    | String    | Units used to measure the sample depth (e.g., Feet)       |
| anl_data_type         | String    | Type of analytical data (e.g., EPA 360.2 (Field))          |
| parameter             | String    | The parameter measured in the sample (e.g., DissolvedOxygen, pH, WaterTemperature)|
| fdr_result            | Float     | Result of the FDR analysis                                 |
| fdr_text_result       | String    | Textual representation of the FDR result                   |
| fdr_date_result       | String    | Date of the FDR result                                     |
| fdr_reporting_limit   | Float     | Reporting limit for the FDR result                          |
| uns_name              | String    | UNS (Unknown Sample) name                                  |
| mth_name              | String    | Method name (e.g., Std Method 2510-B (Field))              |
| fdr_footnote          | String    | Footnote related to the FDR result                         |


