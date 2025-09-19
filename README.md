# Advanced-Pattern-Recognition-

K-Nearest Neighbors (KNN) on the Glass Identification Dataset
This project implements the K-Nearest Neighbors algorithm from scratch in Python and evaluates it on the UCI Glass Identification dataset.
---
Dataset
- Source: UCI Machine Learning Repository (https://archive.ics.uci.edu/ml/datasets/glass+identification)
- Direct CSV: glass.data (https://archive.ics.uci.edu/ml/machine-learning-databases/glass/glass.data)
- Samples: 214
- Features: 9 continuous chemical measurements
- Classes: 6 glass types (building windows, vehicle windows, containers, tableware, headlamps, etc.)
---
Project Workflow
1. Data Loading & Cleaning
   - Read CSV from UCI.
   - Drop the ID column.

2. Preprocessing
   - Train/test split (80/20) with stratified sampling.
   - Standardize features using StandardScaler.

3. Custom KNN Implementation
   - Computes Euclidean distance manually.
   - Finds the k nearest neighbors.
   - Predicts the most common class among neighbors.


4. Model Evaluation
   - Loop through k = 1 15 to find the best accuracy.
   - Plot Accuracy vs. k.
   - Generate classification report and confusion matrix.
---
Results (Sample Run)
Metric
Value
Best k
Typically 5 7 (varies slightly per split)
Accuracy
~70 80 % on the test set
Confusion matrix and accuracy vs k plot are produced to visualize performance.

Visualizations
- Accuracy vs k line plot
- Confusion Matrix heatmap

These plots highlight the effect of different k values and class-wise performance.


Key Learnings
- Implementing KNN manually clarifies how distance-based classification works.
- Glass data is moderately difficult, showing how overlapping classes challenge KNN.
- Tuning k is crucial: small k can overfit; large k can underfit.
---
License
This project is released under the MIT License.
