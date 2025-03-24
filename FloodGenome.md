## FloodGenome: Interpretable Machine Learning for Decoding Features Shaping Property Flood Risk Predisposition in Cities

**Project description:** FloodGenome is an innovative interpretable machine learning model developed to assess the inherent susceptibility of urban areas to property flood damages, independent of specific flooding events. By analyzing hydrological, topographic, and built-environment features, FloodGenome classifies urban areas into distinct flood risk levels using random forest and k-means clustering methods. Leveraging extensive flood claims data from the National Flood Insurance Program (2003-2023), the model identifies critical flood risk factors such as elevation, surface imperviousness, and proximity to drainage systems. Its high accuracy and robust transferability across multiple metropolitan areas make FloodGenome a powerful tool for urban planners and policymakers, providing actionable insights to proactively manage urban flood risk and inform sustainable urban development strategies.

### 1. Flood risk level by k-means

First, K-means is applied to all hydrological, topographic, and built-environment features, the optimal number of clusters was identified using the elbow method, balancing cluster separation and interpretability. Then, each CBG was classified into four distinct risk categories according to similarities in these damage-related metrics. The four risk categories (low, medium, high, and extreme) is deternming by mean building damage ratio multiplied by total number of damaged buildings for each group. This clustering approach effectively reveals areas with comparable flood risk characteristics, enabling targeted and strategic flood risk management.

<img src="images/FG_figure1.png?raw=true"/>

### 2. Assess model transferability
Model transferability was assessed by evaluating how accurately a random forest model trained on data from one metropolitan statistical area (MSA) could predict flood risk levels in other MSAs. Specifically, the model trained on one city’s dataset was applied directly to other cities, and its predictive performance was quantified using the area under the receiver operating characteristic curve (ROC-AUC). High ROC-AUC scores across cities indicate consistent interactions among key flood-risk features, confirming the robustness and generalizability of the FloodGenome model to different urban contexts.

<img src="images/FG_figure2.png?raw=true"/>

### 3. Key Features Among Cities Shaping Property Flood Risk Disposition
Key features consistently shaping property flood risk predisposition across cities include Height Above Nearest Drainage (HAND), impervious surfaces, elevation, building area, and distance to coast. HAND and elevation directly influence flood susceptibility due to their effects on water accumulation and drainage dynamics, with lower values increasing flood risk. Impervious surfaces and building area, indicators of urban development, significantly amplify flood risks by intensifying runoff and reducing natural infiltration. Distance to coast further dictates flood vulnerability, particularly in coastal metropolitan areas. These features highlight critical areas for targeted flood risk mitigation and urban planning interventions.

<img src="images/FG_figure3.png?raw=true"/>

### 4. Specifying flood risk disposition at finer resolution
Flood risk disposition at finer spatial resolutions (e.g., 500m × 500m grid cells) was determined by applying the FloodGenome model trained initially at coarser scales. By recalculating hydrological, topographic, and built-environment features at this more detailed level, the model provides precise, localized flood risk assessments. The accuracy of these fine-resolution predictions was validated against real-world flood damage data, revealing strong alignment between model predictions and observed flood impacts. This fine-grained approach enables urban planners and policymakers to effectively target areas requiring flood mitigation strategies and proactively manage urban development to reduce flood vulnerability.

<img src="images/FG_figure4.png?raw=true"/>
