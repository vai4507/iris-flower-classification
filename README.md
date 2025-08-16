# iris-flower-classification
This project applies machine learning to classify Iris flowers into Setosa, Versicolor, and Virginica. It includes data cleaning, visualization, and model building using Logistic Regression, KNN, Naive Bayes, Decision Tree, and SVM, with most models achieving above 95% accuracy.

The Iris Flower Classification Project is a supervised machine learning project built on the well-known Iris dataset, originally introduced by the statistician Ronald Fisher. The goal of the project is to develop models that can accurately classify iris flowers into one of three species: Iris-setosa, Iris-versicolor, and Iris-virginica, based on four input features — Sepal Length, Sepal Width, Petal Length, and Petal Width.

1. Data Exploration and Preprocessing

The project begins with loading the dataset and basic data cleaning. An unnecessary column (Id) was removed, and checks for missing values confirmed that the dataset was complete. Using df.describe() and df.info(), statistical summaries and data type information were extracted to understand feature ranges and distributions. Additionally, the species distribution was examined using value_counts(), showing a balanced dataset with 50 samples per class.

2. Exploratory Data Analysis (EDA)

To understand feature behavior, histograms were plotted for all four numerical features. Scatter plots were generated for combinations such as Sepal Length vs. Sepal Width and Petal Length vs. Petal Width, with colors representing species. The plots revealed that petal measurements are the most discriminative features for class separation.
A correlation matrix and heatmap further confirmed that petal length and width strongly correlate with species type, making them key predictors.

3. Label Encoding and Train-Test Split

Since machine learning models require numerical inputs, the target variable (Species) was encoded using LabelEncoder. The dataset was then split into training (70%) and testing (30%) sets using train_test_split, ensuring unbiased model evaluation.

4. Model Training and Evaluation

Several machine learning algorithms were implemented and compared:

Logistic Regression – established as a simple linear baseline model.

K-Nearest Neighbors (KNN) – utilized distance-based classification.

Naive Bayes (GaussianNB) – applied probabilistic modeling.

Decision Tree Classifier – provided interpretable, rule-based predictions.

Support Vector Machine (SVM) – delivered robust classification with high accuracy.

Performance was evaluated using accuracy scores and classification reports (precision, recall, F1-score). Most models achieved 95–100% accuracy, with Decision Tree and SVM performing particularly well.

5. Prediction on New Data

The trained Decision Tree model was used to predict species for unseen flower measurements, demonstrating its ability to generalize beyond the training data.
