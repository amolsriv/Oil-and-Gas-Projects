# Oil-and-Gas-Projects
NOTE: Datasets are taken from kaggle.com and other public sources

**Oil and Gas Projects Repository**

This repository is a collection of data science and machine learning projects tailored to solving critical challenges in the oil and gas industry. The projects encompass various aspects of exploration, production, and optimization, using state-of-the-art analytical techniques to extract actionable insights from industry datasets.

**Drilling Optimization**

The Drilling optimisation.ipynb notebook focuses on improving the rate of penetration (ROP) in drilling operations by leveraging advanced machine learning models. Using the dataset Time Interval Data Drilling.csv, this project explores the relationship between operational parameters such as weight on bit, top drive RPM, torque, flow rate, and mud temperature with the ROP.

Key features include detailed data preprocessing, feature engineering (like deriving the Torque_Flow feature to capture non-linear effects), and the application of models such as Random Forest Regressor, XGBoost Regressor, and an ensemble Stacking Regressor. The notebook also integrates SHAP analysis to enhance the interpretability of the machine learning models, allowing users to understand the critical drivers of ROP. Evaluation metrics such as Mean Squared Error (MSE) and ￼ are used to assess model performance, with insights visualized through residual plots and dependence plots.

**Production Optimisation**

The Production Optimisation.ipynb implements a comprehensive workflow for optimizing and visualizing oil production trends using machine learning and interactive dashboards. It begins with training multiple models, including Linear Regression, Random Forest, and XGBoost, to predict oil production based on operational parameters, followed by evaluating and comparing their performance using metrics like R², MAE, and RMSE. Visualizations such as bar charts for model performance and scatter plots for actual vs. predicted values are included for insights. An interactive dashboard, built with Dash, allows users to explore time-series trends, model comparisons, and feature importance dynamically.

**ROP Optimisation**

In ROP optimisation, the goal was to optimize the drilling parameters (WOB and SURF_RPM) to maximize the rate of penetration (ROP) using a machine learning model (GradientBoostingRegressor) encapsulated in a pipeline. First, the range of WOB and SURF_RPM was determined from the dataset, and constant values for the remaining features were set to their mean values. A prediction space was then plotted over the defined ranges of WOB and SURF_RPM, using the trained model to predict ROP values. An objective function was created to maximize ROP, which was then optimized using Particle Swarm Optimization (PSO). The optimization process identified the feature values (xopt) that led to the maximum ROP and the corresponding ROP value (fopt). The solution was visualized through a contour plot of the prediction space, and the optimization results were printed for further analysis.

**Anomaly Detection**

The Anomaly Detection.ipynb notebook tackles the challenge of identifying unusual patterns in gas composition data collected during drilling operations. The dataset GAS Peaks-Drilling_Well.csv is used to analyze various gas components, such as Total Gas, methane (C1), ethane (C2), and propane (C3), across different depths.

This project applies multiple unsupervised learning methods, including Isolation Forest, Local Outlier Factor (LOF), Gaussian Mixture Models (GMM), and Autoencoders. These methods highlight potential anomalies in the data, which could indicate hydrocarbon-rich zones, operational inefficiencies, or safety concerns. Visualizations such as scatter plots and PCA projections help communicate these insights, while metrics like silhouette scores validate the clustering results. The notebook also provides a mechanism for comparing results across methods to ensure consistency in anomaly detection.

**Exploratory Data Analysis**

The Exploratory Data Analysis.ipynb notebook offers a deep dive into datasets related to oil production and petroleum operations. It provides insights into trends over time, regional production comparisons, and the identification of outliers in production data. By leveraging visualization tools and correlation analyses, this notebook helps uncover critical patterns that can guide strategic decisions in resource management and operational efficiency.

