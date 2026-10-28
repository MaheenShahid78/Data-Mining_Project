# 🚀 Space Mission Dataset Analysis Using MapReduce and Machine Learning

## 📌 Project Overview

The **Space Mission Dataset Analysis** project demonstrates how distributed data processing and machine learning techniques can be used to analyze space exploration missions. The project uses a synthetic space mission dataset containing information about mission objectives, target celestial bodies, launch vehicles, mission costs, scientific yield, fuel consumption, and mission success rates.

**MapReduce** is used for data preprocessing and aggregation, while machine learning algorithms are applied to identify patterns, predict mission success, and group missions according to their characteristics.

This project combines big data processing concepts with predictive analytics and clustering to explore how data-driven insights can support space mission planning and resource allocation.

## 🎯 Project Objectives

- Apply the MapReduce programming model to preprocess and aggregate space mission data.
- Explore relationships between mission characteristics and mission success.
- Use Linear Regression to predict average mission success.
- Apply Decision Tree Regression to analyze and predict mission success.
- Use K-Means Clustering to identify groups of missions with similar characteristics.
- Analyze mission costs and scientific yields to identify potentially cost-effective mission targets.
- Demonstrate the integration of distributed data processing and machine learning techniques.

## 📂 Dataset Description

The project uses a **synthetic space mission dataset** designed to represent different aspects of space exploration. It contains categorical and numerical attributes that support data preprocessing, statistical analysis, prediction, and clustering.

### Dataset Features

| Feature | Description |
|---|---|
| Mission ID | Unique identifier assigned to each mission. |
| Mission Name | Name of the space mission. |
| Launch Date | Date on which the mission was launched. |
| Target Type | Category of the celestial body being explored. |
| Target Name | Name of the mission's target. |
| Mission Type | Primary purpose or objective of the mission. |
| Distance from Earth (light-years) | Recorded distance to the target. |
| Mission Duration (years) | Duration of the mission. |
| Mission Cost (billion USD) | Estimated financial cost of the mission. |
| Scientific Yield (points) | Measure of the scientific output of the mission. |
| Crew Size | Number of crew members involved. |
| Mission Success (%) | Recorded mission success rate. |
| Fuel Consumption (tons) | Amount of fuel consumed. |
| Payload Weight (tons) | Weight of the mission payload. |
| Launch Vehicle | Vehicle used to launch the mission. |

The dataset supports the investigation of mission performance, resource consumption, cost-effectiveness, and scientific outcomes.

## 🛠️ Technologies and Concepts

- **Python** — Core programming language for data analysis.
- **Apache Spark / PySpark** — Distributed data processing and MapReduce-related operations.
- **Jupyter Notebook** — Interactive environment for implementing and documenting the analysis.
- **MapReduce** — Data transformation, filtering, and aggregation.
- **Linear Regression** — Predictive modeling of average mission success.
- **Decision Tree Regression** — Interpretable, tree-based prediction.
- **K-Means Clustering** — Unsupervised grouping of missions.
- **Elbow Method** — Technique used to help determine a suitable number of clusters.
- **Silhouette Score** — Metric used to assess the quality of clustering.

## 📁 Project Structure

```text
Space-Mission-Dataset-Analysis/
│
├── Code.ipynb
├── space_missions_dataset.csv
├── Project Report.pdf
└── README.md
```

- `Code.ipynb` — Jupyter Notebook containing the project implementation and analysis.
- `space_missions_dataset.csv` — Dataset used for the analysis.
- `Project Report.pdf` — Academic report documenting the objectives, methodology, results, and conclusions.
- `README.md` — Project overview and documentation.

## ⚙️ Methodology

### 1. Data Preprocessing Using MapReduce

MapReduce concepts are applied to process the dataset through operations such as filtering, transformation, and aggregation. This helps organize the mission data into a form suitable for further analysis.

The approach demonstrates how data-processing tasks can be divided into smaller operations and combined to produce meaningful summaries.

### 2. Linear Regression

Linear Regression is used to model the relationship between selected input features and **average mission success**.

The model helps examine how changes in the selected features relate to the predicted mission success rate. Its performance is evaluated using regression metrics, including R², MAE, MSE, and RMSE.

### 3. Decision Tree Regression

A Decision Tree Regressor is used to predict mission success based on patterns in the processed data.

Decision trees are useful because their branching structure can be interpreted to understand how input features contribute to predictions. However, perfect performance on training data may indicate overfitting.

### 4. K-Means Clustering

K-Means Clustering is used to group missions with similar characteristics.

The Elbow Method is applied to help select the number of clusters, while silhouette scores are used to assess cluster separation and consistency.

The resulting clusters are analyzed in terms of target types, mission costs, and scientific yields.

## 📊 Results and Findings

The results below summarize the findings documented in the project report.

### Linear Regression

- The model achieved an **R² score of 1.0 on the evaluated training data**, with extremely small reported prediction errors.
- The model was used to predict average mission success.
- The report identifies potential overfitting as a concern, particularly because the data was aggregated before modeling.

An R² score of 1.0 on training data does not, by itself, establish that a model will perform equally well on unseen data.

### Decision Tree Regression

- The Decision Tree Regressor produced perfect predictions for the evaluated mission target categories in the report.
- Its interpretability makes it useful for examining relationships between features and predicted outcomes.
- The report highlights potential overfitting and recommends further validation on unseen data.

### K-Means Clustering

The clustering analysis identified two groups with different characteristics:

| Cluster | Characteristics described in the report |
|---|---|
| Cluster 0 | Missions targeting Stars and Planets, associated with higher mission costs and lower scientific yields. |
| Cluster 1 | Missions targeting Exoplanets, Asteroids, and Moons, associated with lower costs and higher scientific yields. |

The report also describes the use of silhouette scores to evaluate the clustering results.

## 💡 Key Insights

- **Cost-effectiveness:** The report identifies Cluster 1 as a potentially cost-effective group because its missions are associated with lower costs and higher scientific yields.
- **Mission diversity:** Different target categories exhibit different cost and scientific-yield characteristics in the clustering analysis.
- **Predictive modeling:** Regression techniques provide a way to investigate relationships between mission features and mission success.
- **Interpretability:** Decision trees offer an understandable structure for examining model predictions.
- **Distributed processing:** MapReduce provides a framework for organizing data preprocessing and aggregation.
- **Model reliability:** Very high training performance should be validated before drawing conclusions about predictions for new missions.

These findings describe patterns in the synthetic dataset and should not be interpreted as established facts about real-world space missions.

## ⚠️ Limitations

- The dataset is synthetic and may not fully represent the complexity of actual space exploration missions.
- Perfect training performance may indicate overfitting rather than reliable generalization.
- Aggregation can simplify the data and may hide variation between individual missions.
- Clustering results depend on the selected features, preprocessing decisions, and number of clusters.
- The findings are limited to the variables and patterns represented in the available dataset.

## 🔮 Future Improvements

- Evaluate models on separate training and testing datasets.
- Apply cross-validation to obtain a more reliable estimate of predictive performance.
- Compare additional regression algorithms and tune model parameters.
- Investigate feature scaling and feature selection for clustering.
- Explore more detailed visualizations of mission costs, scientific yield, and mission success.
- Extend the analysis using larger or real-world space mission datasets.
- Improve the robustness and generalizability of the models before using them for decision-making.

## 🎓 Academic Context

This project was completed as part of the **Bachelor of Data Science** program at the **School of Computing Sciences**.

**Instructor:** Mr. Usama Ahmed  
**Lab Engineer:** Mr. Fahad Qureshi

The project demonstrates the application of distributed data processing and machine learning concepts to a structured data analysis problem.

## 📚 References

1. Saha, D. (2023, April 25). *PySpark Made Easy: Day 2 – Execute PySpark on Google Colabs.* Medium.  
   https://medium.com/@dipan.saha/pyspark-made-easy-day-2-execute-pyspark-on-google-colabs-f3e57da946a

2. Codersarts. (2022, July 2). *EDA Analysis with PySpark Using Zomato Dataset - 08 | Map-Reduce | PySpark Tutorial for Beginners.* YouTube.  
   https://www.youtube.com/watch?v=-LTTG249jMw

3. Data Science for Everyone. (2021, November 5). *K Means Clustering with PySpark Hack Data.* YouTube.  
   https://www.youtube.com/watch?v=mbYNKM3hdPI

4. Demir, N. (2023, July 10). *Data Processing with PySpark: Exploring Filtering, Mapping, and Reducing.* Medium.  
   https://blog.demir.io/data-processing-with-pyspark-exploring-filtering-mapping-and-reducing-537fb1eda5f3

5. rshah204. (2019, October 20). *MapReduce Implementation in PySpark.* GitHub.  
   https://github.com/rshah204/MapReduce-Implementation-in-PySpark/blob/master/MapReduce_PySpark.ipynb

## 👥 Contributors

| Maheen Shahid maheenshahid0302@gmail.com
| Hoor-ul-ain Wajid hoorwajid3@gmail.com


