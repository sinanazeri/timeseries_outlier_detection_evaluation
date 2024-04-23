# timeseries_outlier_detection_evaluation
find the best metric for detecting outliers in time series 

### Problem Definition
The primary goal is to evaluate the effectiveness of various anomaly detection algorithms in identifying outliers within synthetic time series data, and to determine which of several clustering metrics most accurately reflects the correct outlier detection as per the ground truth. The anomaly detection algorithms considered are DBSCAN, Isolation Forest, LOF (Local Outlier Factor), and OneClassSVM. The metrics used to assess these algorithms are F1-Score (for accuracy against ground truth), Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index, and Dunn Index.

### Solution Outline

#### Step 1: Data Generation
- **Generate Synthetic Time Series Data**: Simulate time series data with inherent trends, noise, and deliberately injected outliers. This dataset changes dynamically with each run to ensure the robustness of the findings.

#### Step 2: Anomaly Detection
- **Implement Anomaly Detection Algorithms**: Apply the selected algorithms (DBSCAN, Isolation Forest, LOF, and OneClassSVM) to the generated datasets to identify outliers.

#### Step 3: Evaluation Metrics Calculation
- **Calculate Detection Accuracy Metrics**: Compute the F1 Score, Precision, and Recall for each algorithm based on how well they identify outliers against the ground truth labels.
- **Calculate Clustering Quality Metrics**: Determine the Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index, and Dunn Index for each algorithm's output to assess the quality of clustering.

#### Step 4: Monte Carlo Simulation
- **Run Multiple Simulations**: Execute the above steps multiple times (Monte Carlo simulation) to ensure statistical reliability and robustness of the results. This helps in understanding the consistency of each algorithm across varied datasets.

#### Step 5: Correlation Analysis
- **Correlate F1 Scores with Clustering Metrics**: Analyze how each clustering metric correlates with the F1 Scores across all runs and algorithms to identify which metric aligns best with the ground truth recognition of outliers.

#### Step 6: Regression Analysis
- **Predict F1 Scores from Clustering Metrics**: Use regression analysis to determine how well the clustering metrics can predict the F1 Scores, thereby quantifying the predictive power of each metric regarding anomaly detection performance.

#### Step 7: Visual Analysis
- **Plot Metrics vs. F1 Scores**: Visually inspect the relationship between each clustering metric and the F1 Scores through scatter plots to observe trends, outliers, and anomalies in the relationship.

#### Step 8: Interpretation and Conclusion
- **Interpret Results**: Based on the correlation, regression, and visual analyses, conclude which clustering metric best represents the effectiveness of outlier detection algorithms in relation to the ground truth. This helps in selecting appropriate metrics for evaluating anomaly detection in similar datasets.

By following this structured approach, you can robustly assess the effectiveness of different anomaly detection algorithms and understand which clustering metrics provide the most accurate reflection of their performance against the actual occurrence of outliers. This comprehensive evaluation is critical for selecting the right tools and metrics for practical applications in anomaly detection.

----

## Results


![image](https://github.com/sinanazeri/timeseries_outlier_detection_evaluation/assets/121966646/8a35fd83-7cde-478c-af47-0b07f68cd36f)
![image](https://github.com/sinanazeri/timeseries_outlier_detection_evaluation/assets/121966646/17377b74-94aa-4dd9-9436-002920100bc8)
![image](https://github.com/sinanazeri/timeseries_outlier_detection_evaluation/assets/121966646/f118c5ac-9b26-4a1d-b2ac-5c366983e05a)
