## Leveraging heterogeneous data and machine learning for mapping connectivity and infrastructure provision in Amazon

**Project description:** This study addresses the critical challenge of data scarcity in the Amazon region by developing a machine learning framework to map infrastructure provision and regional connectivity. By integrating heterogeneous datasets—including OpenStreetMap (OSM), human mobility data, and satellite imagery—the research provides a high-resolution assessment of how communities access essential services. The project utilizes H3 hexagonal hierarchical spatial indexing, K-Means, XGBoost, SHAP Analysis to identify "infrastructure-poor" areas and quantify the impact of seasonal connectivity disruptions, such as river level fluctuations.

### 1. Multi-Source Data Fusion & Spatial Indexing
The framework utilizes a multi-layered approach to overcome the limitations of traditional census data in remote regions:
* **H3 Spatial Indexing:** All data is standardized into a hexagonal grid system (H3) to ensure consistent spatial resolution across the vast Amazon basin.
* **Infrastructure Indicators:** Using OSM data, the study maps the density and distribution of healthcare, education, and energy facilities.
* **Connectivity Modeling:** The research models "Amazonian accessibility" by combining land-based road networks with riverine transport routes.

<img src="images/Amazon_figure1.png?raw=true"/>

### 2. Machine Learning for Infrastructure Gap Analysis
To identify underserved areas, the project employs advanced modeling techniques to predict infrastructure provision levels:
* **Feature Engineering:** Socio-economic and environmental variables are extracted to train models that can estimate infrastructure availability in areas where ground-truth data is missing.
* **K-means Clustering:** Used to categorize regions into distinct "Infrastructure Development Profiles," ranging from well-connected urban hubs to isolated remote communities.
* **Interpretability(SHAP):** The study uses SHAP (SHapley Additive exPlanations) values to identify the primary drivers of infrastructure provision, such as proximity to major rivers or historical road development.
<img src="images/Amazon_figure1.png?raw=true"/>

<img src="images/Amazon_ipi.png?raw=true"/>

### 3. Key Findings & Policy Impact

* **Connectivity Disparities:** Identified significant "connectivity deserts" where communities face extreme isolation.
* **Strategic Planning:** The findings offer actionable insights for the World Bank and local governments to prioritize infrastructure investments that minimize environmental impact while maximizing social benefit.

