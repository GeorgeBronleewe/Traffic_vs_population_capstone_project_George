## Methodology  
1. **Data Ingestion**  
   - Load Census ACS tables for 2013, 2018, and 2023.  
   - Load traffic datasets for Davidson County.  

2. **Cleaning & Standardization**  
   - Standardized column names across years (e.g., `population_total`, `owner_occupied`, `mode_total`).  
   - Dropped raw ACS margin/error columns.  
   - Aligned transportation categories (adjusting for “work from home” being introduced in 2020).  

3. **Exploratory Analysis**  
   - Compared population growth to changes in commute time distributions.  
   - Analyzed shifts in transport mode share (drive-alone vs. public transport vs. remote work).  
   - Calculated per-capita vehicle availability over time.  

4. **Traffic Integration**  
   - Merged demographic and commute data with Annual Average Daily Traffic counts.  
   - Explored correlation between traffic volume and population/household growth.  

## Key Questions  
- How much has Davidson County’s population grown from 2013 to 2023?  
- Are commute times worsening, improving, or stable?  
- Has the rise in remote work reduced pressure on roads?  
- How does vehicle availability compare to housing growth?  
- Do traffic counts reflect population growth trends?  

## Tools & Libraries  
- **Python** (pandas, numpy, matplotlib, seaborn)  
- **Geospatial Analysis** (GeoPandas, Folium, shapefiles/GeoJSON)  
- **Jupyter Notebooks** for reproducible analysis  
- **Git & GitHub** for version control  

## Repository Notes  
- Large geospatial files are excluded via `.gitignore`.  
- This repo highlights data wrangling, exploratory data analysis (EDA), and integration of multiple years of ACS census data with transportation records.  
- Notebooks are structured to allow reproducibility and incremental checking of cleaning steps.  

## Next Steps  
- Perform regression analysis between **population growth** and **traffic volumes**.  
- Visualize geographic distribution of traffic intensity vs. housing growth.  
- Develop policy recommendations around transportation infrastructure.  