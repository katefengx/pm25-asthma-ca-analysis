# Influence of PM2.5 Air Pollution on Asthma Rates in California Adults

---

## Abstract

Air pollutants such as particulate matter 2.5 (PM2.5) pose significant public health risks, exacerbated by climate change. This study investigates the correlation between PM2.5 pollution levels and the prevalence of adult asthma in California, aiming to identify regional patterns and explore potential confounding factors. Understanding these relationships is critical for informing policies to mitigate pollutant impact and reduce asthma prevalence.

By integrating data from the CDC’s PLACES dataset and the EPA’s PM2.5 pollution data, we performed exploratory data analysis and statistical assessments to explore spatial, temporal, and distributional trends. Our findings reveal regional disparities with Central California experiencing the highest PM2.5 levels, but Northern California showing higher asthma rates despite lower pollution, suggesting other factors like urbanization and healthcare access also influence asthma prevalence.

---

## Data Overview

### PLACES Dataset: Local Data for Better Health (County Level)

- **Source:** [CDC PLACES](https://data.cdc.gov/500-Cities-Places/PLACES-Local-Data-for-Better-Health-County-Data-20/swc5-untb/about_data)
- **Raw data:** 240,886 observations, 22 variables
- **Cleaned data:** 58 observations (California counties), 9 variables

This dataset provides county-level health statistics, including asthma prevalence among adults. Key variables include `totalpopulation` and `data_value` (percentage prevalence of asthma). We filtered for California counties and focused on adult asthma ("CASTHMA"), standardizing data for population where appropriate.

### EPA Dataset: 2022 PM2.5 Levels in California

- **Source:** [EPA Air Quality Data](https://www.epa.gov/outdoor-air-quality-data/download-daily-data)
- **Raw and cleaned data:** 59,756 observations, 22 raw variables reduced to 12 clean variables

Contains daily PM2.5 concentrations and Air Quality Index (AQI) values from monitoring sites across California. We aggregated data by county to obtain average pollution metrics, enabling spatial analysis of air quality.

---

## Methodology

### Data Preprocessing

- Filtered PLACES dataset to select relevant health measures for California counties.
- Cleaned EPA data by removing unnecessary columns and handling missing values.
- Aggregated EPA monitoring site data by county and averaged daily values to represent overall county pollution levels.
- Merged datasets on county names for combined analysis.

### Exploratory Data Analysis (EDA)

- Visualized top 10 counties with highest PM2.5 concentrations via bar charts.
- Created choropleth maps showing spatial distribution of asthma prevalence and AQI across California counties.
- Box plots analyzed regional asthma prevalence differences.
- Investigated correlations between asthma rates and pollution, noting regional disparities.

### Statistical Analysis

- Examined spatial and temporal trends of PM2.5 and asthma prevalence.
- Identified confounding factors such as urbanization and healthcare access influencing asthma prevalence beyond pollution levels.

---

## Key Findings

- **Regional Variations:** Central California had the highest PM2.5 concentrations, often exceeding health advisory limits. Northern California had elevated asthma prevalence despite lower PM2.5 levels, highlighting other influencing factors. Southern California showed the lowest levels for both metrics.
- **Correlation:** Some overlap between high PM2.5 and asthma prevalence counties, but no definitive causal link could be established due to confounding variables.
- **Complexity:** Asthma prevalence is influenced by multiple factors beyond air pollution, requiring multifaceted mitigation approaches.

---

## Limitations

- Aggregation at the county level may mask local pollution variability, especially between urban and rural areas.
- Data limited to 2022, restricting temporal trend analysis and seasonality insights.
- Other factors such as socio-economic status, healthcare access, and lifestyle behaviors were not included but likely affect asthma rates.
- The study is observational and cannot establish causation.

---

## Societal Impact

This analysis highlights environmental health disparities impacting low-income California communities disproportionately burdened by poor air quality and limited healthcare access. It underscores the importance of targeted public health policies, stricter pollution controls, and improved healthcare services to address environmental injustice and reduce asthma prevalence.

---

## Team Contributions

- **Kate** – Coordinated workflow, ensured cohesion, developed interactive choropleth maps for asthma and PM2.5, edited final video presentation.
- **Katelyn** – Retrieved and cleaned PLACES data, led exploratory data analysis, created box plots and bar charts linking asthma to regions.
- **Heidi** – Cleaned PM2.5 data, managed project timeline, created bar charts of top counties by PM2.5 levels.
- **Kyla** – Conducted literature research, summarized pollutant data, developed interactive PM2.5 visualizations by county.
- **Felix** – Explored ethical/privacy concerns, summarized asthma data insights, created AQI choropleth maps.

---

## How to Use This Repository

- The primary Jupyter notebook `final_analysis.ipynb` contains the complete analysis pipeline including data cleaning, EDA, visualization, and statistical testing.
- Data files are stored in the `data/` directory.
- Visualizations are saved in the `assets/` folder, including interactive charts and maps.
- Visit the [Project Page](https://katefengx.github.io/power-outage-prediction/) for an interactive experience.

---

## Contact

For questions or collaboration inquiries, please contact Kate Feng at \[your email].

---

Let me know if you want me to tailor it for a specific audience or add installation instructions, or a shorter version!
