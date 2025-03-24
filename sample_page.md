## FloodGenome: Interpretable Machine Learning for Decoding Features Shaping Property Flood Risk Predisposition in Cities

**Project description:** FloodGenome is an innovative interpretable machine learning model developed to assess the inherent susceptibility of urban areas to property flood damages, independent of specific flooding events. By analyzing hydrological, topographic, and built-environment features, FloodGenome classifies urban areas into distinct flood risk levels using random forest and k-means clustering methods. Leveraging extensive flood claims data from the National Flood Insurance Program (2003-2023), the model identifies critical flood risk factors such as elevation, surface imperviousness, and proximity to drainage systems. Its high accuracy and robust transferability across multiple metropolitan areas make FloodGenome a powerful tool for urban planners and policymakers, providing actionable insights to proactively manage urban flood risk and inform sustainable urban development strategies.

### 1. Flood risk level by k-means

First, K-means is applied to all hydrological, topographic, and built-environment features, the optimal number of clusters was identified using the elbow method, balancing cluster separation and interpretability. Then, each CBG was classified into four distinct risk categories according to similarities in these damage-related metrics. The four risk categories (low, medium, high, and extreme) is deternming by mean building damage ratio multiplied by total number of damaged buildings for each group. This clustering approach effectively reveals areas with comparable flood risk characteristics, enabling targeted and strategic flood risk management.

<img src="images/FG_figure1.png?raw=true"/>

### 2. Assess model transferability
Model transferability was assessed by evaluating how accurately a random forest model trained on data from one metropolitan statistical area (MSA) could predict flood risk levels in other MSAs. Specifically, the model trained on one city’s dataset was applied directly to other cities, and its predictive performance was quantified using the area under the receiver operating characteristic curve (ROC-AUC). High ROC-AUC scores across cities indicate consistent interactions among key flood-risk features, confirming the robustness and generalizability of the FloodGenome model to different urban contexts.

<img src="images/FG_figure2.png?raw=true"/>

### 3. Key Features Among Cities Shaping Property Flood Risk Disposition


<img src="images/FG_figure3.png?raw=true"/>

### 4. Specifying flood risk disposition at finer resolution


<img src="images/FG_figure4.png?raw=true"/>
