# Student Stress Classification

A machine learning project focused on analyzing and classifying student stress levels using psychological, academic, and social indicators.

The project explores feature selection, dimensionality reduction, statistical analysis, and multiple classification algorithms to predict low, medium, and high stress levels.

Dataset

The project uses the Student Stress Monitoring Dataset.

* 1,100 samples
* 20 input features
* 3 target classes:
    * 0 — Low stress
    * 1 — Medium stress
    * 2 — High stress
* No missing values
* Approximately balanced class distribution

The dataset includes psychological, academic, and social factors such as anxiety level, depression, self-esteem, sleep quality, academic performance, and social support.

Project Workflow

1. Exploratory Data Analysis

* Dataset inspection and statistical analysis.
* Class distribution analysis.
* Missing value detection.
* Outlier detection using the IQR method.
* Feature distribution visualization.

2. Feature Selection

* Information Gain calculation.
* Ranking features according to their predictive relevance.
* Pearson correlation analysis.
* Selection of the most informative features.

3. Dimensionality Reduction

* Feature standardization.
* Linear Discriminant Analysis (LDA).
* Projection into a lower-dimensional feature space.
* Visualization of class separability.

4. Hypothesis Testing and Classification

* Stratified train-test split.
* Linear Discriminant Analysis classifier.
* Confusion matrix analysis.
* Precision, sensitivity, specificity, and accuracy evaluation.

5. K-Nearest Neighbors

* KNN classification.
* Hyperparameter selection using 5-fold cross-validation.
* Comparison between LDA-reduced and full feature spaces.
* Test set evaluation.

6. Neural Networks

* Training neural networks with different architectures.
* Comparison of small, optimal, and oversized networks.
* Training and validation analysis.
* Early stopping.
* Test set evaluation.

Reported Results

The following results are reported in the project documentation:

Classification Model	Test Accuracy
LDA Classifier	90.00%
KNN — LDA-reduced features	91.36%
KNN — 20 original features	87.27%
Neural Network (20, 10)	89.09%
Neural Network (3, 2)	85.45%

The best reported result was achieved by KNN using the LDA-reduced feature space, with a test accuracy of 91.36%.

Results are specific to this dataset and experimental setup.

Technologies and Libraries

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

Repository Structure

student-stress-classification/
│
├── 18_stress_dataset.csv
├── student_stress_classification.ipynb
├── requirements.txt
├── .gitignore
└── README.md

The notebook filename in this structure should match the actual uploaded filename.

How to Run

1. Clone the repository.
2. Install the required dependencies:

pip install -r requirements.txt

3. Open the Jupyter Notebook:

jupyter notebook

4. Open the project notebook.
5. Make sure the dataset CSV file is located in the same directory as the notebook.
6. Run all cells.

Key Takeaways

This project demonstrates an end-to-end machine learning workflow, from exploratory data analysis and feature selection to dimensionality reduction, classification, neural network training, and model evaluation.

It also highlights the importance of comparing models across different feature representations and evaluating their performance using multiple classification metrics.
