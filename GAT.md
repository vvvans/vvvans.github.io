## Graph Attention Networks Unveil Determinants of Intra- and Inter-city Health Disparity

**Project description:** This study introduces an innovative graph attention network (GAT) approach to identify and analyze determinants of urban health disparities across five major U.S. cities. By integrating heterogeneous features such as socio-demographics, human mobility, population activity, and built-environment characteristics, the model predicts the prevalence of obesity, diabetes, cancer, and heart disease at a neighborhood scale. Leveraging large-scale mobility datasets and urban feature interactions, the research highlights key factors influencing health outcomes, demonstrating high model transferability and offering valuable insights for targeted public health interventions and urban planning policies aimed at reducing health disparities.

### 1. Model performance

This experiment evaluated the effectiveness of Graph Attention Networks (GAT) in predicting health outcomes (obesity, diabetes, cancer, and heart disease) at the neighborhood (census tract) level in five major U.S. cities.

<img src="images/FG_figure1.png?raw=true"/>

### 2. Feature Importance Analysis
To understand which urban factors most significantly contribute to neighborhood health disparities, the study applied the GraphLIME method, a local interpretable modeling technique. GraphLIME provided detailed insights into feature importance by ranking how each factor contributed to the GAT model predictions. Analysis revealed socio-demographic variables (e.g., income, age, minority percentage), built-environment features (density of facilities like grocery stores and restaurants), and population activity metrics as consistently influential across different cities and diseases. Notably, mobility and activity features emerged as particularly important predictors for diseases like diabetes and heart disease, highlighting critical areas for targeted urban planning and public health interventions.

<img src="images/FG_figure2.png?raw=true"/>

### 3. Cross-city Transferability Analysis
Models trained using data from one city were directly applied to predict health outcomes in other cities without additional tuning. The success of this approach was quantified through model accuracy (F1-score), revealing that significant similarities exist among the determinants of health disparities across cities, especially for conditions like obesity and diabetes. This indicates that urban health disparities, though context-specific in detail, share underlying universal patterns that can inform transferable urban design and public health strategies, enhancing efforts to reduce health inequalities on a broader scale.

<img src="images/FG_figure3.png?raw=true"/>

### 4. Specifying flood risk disposition at finer resolution
Flood risk disposition at finer spatial resolutions (e.g., 500m × 500m grid cells) was determined by applying the FloodGenome model trained initially at coarser scales. By recalculating hydrological, topographic, and built-environment features at this more detailed level, the model provides precise, localized flood risk assessments. The accuracy of these fine-resolution predictions was validated against real-world flood damage data, revealing strong alignment between model predictions and observed flood impacts. This fine-grained approach enables urban planners and policymakers to effectively target areas requiring flood mitigation strategies and proactively manage urban development to reduce flood vulnerability.

<img src="images/FG_figure4.png?raw=true"/>
