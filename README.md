# Public Health & Opioid Study  

A research-driven analysis of how **socioeconomic disadvantage** and **opioid prescribing practices** influence mortality across U.S. counties. This project combines **statistical modeling**, **machine learning**, and **spatial data analysis** to explore structural drivers of the opioid epidemic.  

---

## 🎯 Research Motivation  
The opioid crisis in the United States has emerged as a leading public health challenge, with mortality disproportionately affecting economically disadvantaged regions. This project investigates:  

- **Are higher opioid prescribing rates associated with increased mortality?**  
- **Does socioeconomic disadvantage, particularly poverty, amplify these risks?**  
- **How do these relationships vary across geographic space?**  

By leveraging county-level data and geospatial methods, the project provides a data-informed perspective on structural health inequities.  

---

## 📊 Data Sources  
- **Mortality data:** CDC WONDER cause-of-death statistics  
- **Poverty data:** U.S. Census Bureau American Community Survey (ACS)  
- **Opioid prescribing rates:** National prescribing datasets  
- **Geospatial shapefiles:** U.S. Census Bureau TIGER/Line files  

Datasets were harmonized using **FIPS codes** to ensure accurate county-level merging.  

---

## 🧮 Methodology  
- **Data Preparation**  
  - Cleaning and harmonizing heterogeneous datasets  
  - Standardizing predictors using Z-scores  
  - Managing unreliable/missing mortality records  

- **Exploratory Analysis**  
  - Correlations and scatterplots  
  - Histograms and distributional checks  
  - Poverty-opioid interactions  

- **Modeling Approaches**  
  - **Multiple Linear Regression**: Baseline model and interaction model  
  - **Decision Tree Classification**: Identifying interpretable thresholds for county risk stratification  

- **Geospatial Analysis**  
  - County-level risk mapping  
  - Heatmaps of predicted mortality  
  - Residual analysis to highlight under/overperforming models  

---

## 📈 Key Insights  
- **Positive associations**: Both poverty and opioid prescribing independently predict higher mortality.  
- **Interaction effect**: Poverty moderates the impact of opioid access, with disadvantaged counties showing heightened vulnerability.  
- **Decision tree findings**: Counties with >31% poverty *and* high prescribing rates exhibit dramatically higher mortality (~55 deaths/100,000).  
- **Spatial clustering**: High-risk regions concentrated in the South, Midwest, and Appalachia.  

---

## 🛠️ Tools & Techniques  
- **Languages & Environment**: R, R Markdown  
- **Libraries**: tidyverse, dplyr, ggplot2, sf, rpart, rpart.plot  
- **Techniques**: Regression modeling, interaction terms, decision trees, z-score normalization, geospatial joins  
- **Outputs**: Publication-ready PDF report with embedded code, visualizations, and interpretations  

## 🚀 Reproducibility  
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/public-health-opioid-study.git
   cd public-health-opioid-study
