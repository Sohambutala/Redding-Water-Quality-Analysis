# Redding-Water-Quality-Analysis

## Introduction
In the serene expanses of Redding, California, where nature's beauty intertwines with the ever-present specter of wildfires, the community finds itself at the intersection of environmental resilience and burgeoning challenges. The recent escalation in the frequency and intensity of wildfires has not merely been a distant occurrence but a palpable reality that hovers over the city. Although the average distance of these fires has exhibited an exponential retreat, the tendrils of their impact persist, raising crucial questions about the implications for Redding's environment and, notably, its water quality.

## Purpose
The purpose of this project is to explore the intricate relationships between wildfires, air quality, and water quality in Redding, California. By delving into the less-explored repercussions on water quality, the analysis seeks to unravel the complex dynamics of the aftermath of wildfires on the city's lifeblood—the water supplies. The urgency of this study is underscored by recent events, emphasizing the need for proactive measures to safeguard both the environment and public health.

## Methodology

### Water Quality Analysis

- **Overview:** Utilizing the smoke estimate dataset and the wildfires dataset from the first step [1](./README.md#methodology), this analysis aims to address the hypothesis regarding the correlation between wildfires and water quality in Redding, California.

- **Steps:**
  1. Downloaded the required water quality dataset from data.cnra.ca.gov to initiate the analysis.
  2. Computed the smoke estimate for each fire as outlined in the third step of the methodology [1](./README.md#methodology).
  3. Generated maps illustrating the geographical distribution of wildfires and field results of water analysis to provide a visual overview.
  4. Processed the water data, retaining essential information including sample_date, parameter, and fdr_result values.
  5. Plotted the distance of fires from Redding across years and introduced a trend line to reveal any discernible patterns.
  6. Constructed dual-axis plots for key water quality parameters (Water Temperature, pH, Turbidity, and Specific Conductance) against the calculated Smoke Estimate.
  7. **Note**: We are not creating any intermediate datasets but processing the one mentioned below to extract insights.

- **Findings:**
  - Produced graphical representations showcasing correlation and trend lines to interpret the results.
  - Concluded the hypothesis regarding the potential impact of wildfires on water quality by analyzing trends in both wildfires and water parameters.

- **Importance:**
  - This step contributes to a holistic understanding of the interplay between wildfires, smoke estimates, and water quality. By visualizing trends and correlations, the analysis sheds light on potential connections between these factors in the Redding region.

- **References**
    - This analysis builds upon the work conducted in another [repository](https://github.com/Sohambutala/Redding-Water-Quality-Analysis)


## Special Considerations

When interpreting the results of the water quality analysis, it is crucial to consider several special considerations that impact the robustness and generalizability of the findings. These considerations encompass both human-centered aspects and technical intricacies:

### Human-Centered Considerations

1. **Community Relevance:**
   - Acknowledge the importance of the study's findings to the local community in Redding. Ensure that the results are communicated in a manner accessible to a diverse audience, including residents and policymakers.

2. **Public Health Implications:**
   - Recognize the potential public health implications of water quality trends influenced by wildfires. Consider the relevance of the findings to community well-being and address any potential health concerns that may arise.

3. **Community Engagement:**
   - Foster ongoing community engagement and participation. Encourage collaboration with local stakeholders to gather insights, validate findings, and ensure that the study aligns with community needs.

### Technical Considerations

1. **Data Quality and Completeness:**
   - Evaluate the quality and completeness of the water quality dataset obtained from data.cnra.ca.gov. Acknowledge any limitations or gaps in the data that may impact the accuracy and reliability of the analysis.

2. **Smoke Estimate Accuracy:**
   - Understand the limitations associated with estimating smoke impact for each fire. Acknowledge that the accuracy of smoke estimates depends on various factors, including the distance from Redding and the hectares burnt, and may serve as a proxy measure rather than a precise quantification.

3. **Visualization Interpretation:**
   - Exercise caution when interpreting graphical representations, correlation plots, and trend lines. Recognize that visualizations provide insights but may not establish causation, and correlations observed in the data do not imply direct relationships without further analysis.

4. **Temporal Misalignment:**
   - Be mindful of any temporal misalignment between the water quality data and the wildfire/smoke estimate data. Addressing this misalignment ensures that the analysis accurately captures the interplay between wildfires and water quality over time.

5. **Ethical Data Use:**
   - Adhere to ethical considerations in handling and using data. Prioritize privacy, confidentiality, and responsible data practices throughout the analysis, respecting the rights and interests of individuals represented in the datasets.

6. **Communication of Uncertainty:**
   - Clearly communicate the uncertainties associated with the study findings. Acknowledge the complexity of the relationships between wildfires and water quality, and avoid overgeneralization or making definitive claims beyond the scope of the data.

These special considerations contribute to a comprehensive and nuanced understanding of the water quality analysis, fostering transparency, accountability, and responsible research practices.

## Project Outcome:

This comprehensive project aimed to explore the intricate relationships between wildfires, air quality, and water quality in the Redding, California region. For detailed insights refer the [report](./Documentation/DATA512-Project%20Report.pdf) Key findings include:

### Air Quality Insights:

Correlation between recorded wildfires and Air Quality Index (AQI) data, showcasing how wildfire events significantly impact air quality.
Successful application of machine learning models to estimate smoke impact, providing a predictive tool for assessing future air quality trends.
### Water Quality Analysis:

Identification of potential correlations between wildfire events, calculated smoke estimates, and key water quality parameters (e.g., Water Temperature, pH, Turbidity).
Visualization of temporal trends in water quality parameters, shedding light on the dynamic interplay between wildfires and water quality over the years.
These outcomes contribute to a holistic understanding of the environmental dynamics in the Redding region, offering valuable insights for stakeholders, policymakers, and researchers interested in the intersection of wildfires and ecological elements.

## License
- [Water Quality Dataset License](https://data.ca.gov/dataset/water-quality-data)
- [USGS Wildland Fire Combined Dataset License](https://www.usgs.gov/information-policies-and-instructions/copyrights-and-credits)
- The dataset is made available under the [Creative Commons License](https://creativecommons.org/licenses/by/4.0/).
- [Sample notebook for Geodetic Distance Computation](https://drive.google.com/file/d/1qNI6hji8CvDeBsnLDAhJXvaqf2gcg8UV/view?usp=sharing)
- [Sample code for accessing the US EPA Air Quality System API](https://drive.google.com/file/d/1bxl9qrb_52RocKNGfbZ5znHVqFDMkUzf/view?usp=sharing)
- [Sample code for GeoJSON reader](https://drive.google.com/file/d/1TwCkvdaw0MxJzW7NSDg6XxYQ0dvaS44I/view?usp=sharing)

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


