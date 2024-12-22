# Regional Analysis: Nitrogen Dioxide (NO2)

## Overview
This project investigates the levels of nitrogen dioxide (NO2), a key air pollutant, across various regions, countries, and years. Using the World Health Organization (WHO) Air Quality Database, the study analyzes the temporal trends and spatial disparities in NO2 emissions. Statistical tests, including Welch's t-test, bootstrapping, and chi-square tests, are used to examine differences in emissions across regions and timeframes. 

The project focuses on:
1. Regional NO2 emissions comparison between the South East Asia and European regions.
2. Temporal NO2 emission changes in France and India.
3. Global NO2 compliance trends based on WHO guidelines.

## Data Sources
1. **WHO Air Quality Database (2022)**: Includes annual mean concentrations of PM2.5, PM10, and NO2 across cities worldwide.
2. **World Bank Population Data (2022)**: Provides population data for demographic analysis.

## Methodology
### Data Preparation
- Columns irrelevant to the analysis were dropped (e.g., PM2.5, PM10).
- Missing values were removed.
- NO2 temporal coverage > 90% was retained to ensure data quality.
- Population data was merged with NO2 data to explore demographic correlations.

### Statistical Tests
1. **Welch's t-test**:
   - Compared NO2 levels between South East Asia and European regions in 2019.
   - Tested whether France reduced NO2 emissions in 2016 compared to 2010.
   - Evaluated whether India had greater NO2 emissions in 2018 compared to 2014.

2. **Bootstrapping**:
   - Applied for France's NO2 comparison between 2010 and 2016 to validate results.

3. **Chi-square test**:
   - Assessed whether global compliance with WHO NO2 guidelines is dependent on year.

## Key Findings
- **Regional Comparison**: South East Asia had significantly higher NO2 levels than the European region in 2019.
- **Temporal Trends**:
  - France reduced NO2 emissions significantly from 2010 to 2016.
  - India showed no significant change in NO2 emissions from 2014 to 2018.
- **Global Compliance**: NO2 compliance with WHO guidelines varies significantly by year.

## Results Visualization
- Pair plots, scatter plots, box plots, and heatmaps were created using Python's Plotly library for interactive data visualization.

## Tools and Libraries
- **Data Analysis**: R, dplyr, tidyr
- **Visualization**: Python, Plotly
- **Statistical Testing**: Welch's t-test, Bootstrapping, Chi-square test

## Limitations
- Limited data coverage across rural areas and certain regions.
- Missing data for specific years and cities.
- Unequal sample sizes between regions, necessitating the use of Welch's t-test.

## Conclusion
The analysis highlights the regional disparities and temporal trends in NO2 emissions. While France has successfully reduced its NO2 levels, South East Asia continues to face challenges due to industrialization and urbanization. The findings emphasize the importance of policy interventions and enhanced monitoring for global air quality improvement.

## References
- World Health Organization (2022). WHO Air Quality Database.
- World Bank (2022). Population Data.
- Jion, Most. M. M. F., et al. (2023). A critical review and prospect of NO2 pollution over Asia.
- Kolcava, D., et al. (2019). Does trade liberalization lead to environmental burden shifting?

## How to Run the Analysis
1. Clone the repository and navigate to the project directory.
2. Load the datasets (`who_dataset_v1.csv` and `who_population.csv`).
3. Execute the R scripts for data cleaning and statistical analysis.
4. Use Python scripts for visualizations.
5. Review the generated plots and results.

---

## License

This project is licensed under an **All Rights Reserved** license. Unauthorized use, distribution, or modification of the code is strictly prohibited. For inquiries or permission requests, please contact [sm3924@georgetown.edu or msheeba00@gmail.com].
