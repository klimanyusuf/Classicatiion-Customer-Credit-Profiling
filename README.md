# Customer Segmentation and Credit Risk Prediction

This project utilizes machine learning techniques to address two key business problems: customer segmentation using clustering and credit risk prediction. It leverages two datasets: `users_data.csv` for customer segmentation and `classification_data.csv` for credit risk prediction.

## Project Structure

The project is divided into two main phases:

**Phase 1: Credit Risk Prediction (Classification) **

1.  **Exploratory Data Analysis (EDA):**
    *   Visualizing the distribution of labels.
    *   Analyzing the correlation between features using a heatmap.

2.  **Feature Engineering:**
    *   Encoding categorical variables using LabelEncoder.
    *   Removing irrelevant features (e.g., user\_id).
    *   Splitting data into training and testing sets.

3.  **Data Balancing:**
    *   Addressing class imbalance using SMOTE (Synthetic Minority Over-sampling Technique).

4.  **Feature Scaling:**
    *   Standardizing numerical features using StandardScaler.

5.  **Model Building:**
    *   Training various classification models:
        *   Logistic Regression
        *   Random Forest
        *   XGBoost

6.  **Model Evaluation:**
    *   Evaluating model performance using metrics such as accuracy, precision, recall, ROC-AUC, and confusion matrix.

**Phase 2: Customer Segmentation (Clustering)**

1.  **Exploratory Data Analysis (EDA):**
    *   Analyzing dataset information and identifying missing values.

2.  **Data Cleaning:**
    *   Handling missing values (e.g., filling with median).
    *   Addressing infinite values (replacing with NaN and then handling them).

3.  **Preprocessing:**
    *   Removing irrelevant columns (e.g., user\_id).
    *   Scaling numerical features using StandardScaler.

4.  **Clustering:**
    *   Performing customer segmentation using KMeans clustering algorithm.

5.  **Visualization:**
    *   Visualizing clusters using PCA (Principal Component Analysis) for dimensionality reduction.

6.  **Cluster Analysis:**
    *   Analyzing cluster characteristics by examining the mean values of features within each cluster.

## Libraries Used

*   pandas
*   scikit-learn (sklearn)
*   matplotlib
*   seaborn
*   imblearn
*   xgboost
*   numpy

## Conclusion

This project demonstrates the application of machine learning for customer segmentation and credit risk prediction. The generated insights can be used to improve business decision-making, target specific customer groups, and mitigate credit risk.


## Results

The project identifies distinct customer segments with varying characteristics (e.g., loan scores, device ratings, data quality). The insights gained from the cluster analysis can be used for:

- **Targeted Marketing:** Tailor marketing campaigns to specific customer groups.
- **Risk Assessment:** Identify high-risk and low-risk customer segments.
- **Product Development:** Develop products or features that cater to the needs of different customer clusters.
- **Customer Relationship Management:** Improve customer service and retention efforts.

## Further Exploration

- **Feature Engineering:** Explore creating new features to potentially improve cluster separation.
- **Hyperparameter Tuning:** Optimize the K-Means algorithm parameters (e.g., number of clusters, initialization method).
- **Different Clustering Algorithms:** Experiment with other clustering techniques (e.g., hierarchical clustering, DBSCAN).
- **Deployment:** Develop a system to automatically segment new users and update clusters as data changes.
