# How to complete data science projects for submission

The current batch of projects included in this course are all data science/machine learning projects ask you to use a specific type of model to make predictions based on a dataset. These projects all follow the same format and steps, mirroring the workflow of a data scientist. The only real difference between them are the model type employed and the dataset (though a few even share the same dataset). The projects I am referring to are as follows:

1. [Logistic Regression](https://4geeks.com/syllabus/data-science-7/project/logistic-regression-project-tutorial)
2. [Linear Regression](https://4geeks.com/syllabus/data-science-7/project/linear-regression-project-tutorial)
3. [Regularized Linear Regression](https://4geeks.com/syllabus/data-science-7/project/regularized-linear-regression-project-tutorial)
4. [Decision Trees](https://4geeks.com/syllabus/data-science-7/project/decision-tree-project-tutorial)
5. [Random Forests](https://4geeks.com/syllabus/data-science-7/project/random-forest-project-tutorial)
6. [Boosting Algorithms](https://4geeks.com/syllabus/data-science-7/project/boosting-algorithms-project-tutorial)
7. [Naive Bayes](https://4geeks.com/syllabus/data-science-7/project/naive-bayes-project-tutorial)
8. [K-nearest Neighbors](https://4geeks.com/syllabus/data-science-7/project/k-nearest-neighbors-project-tutorial)

The instructions given in each case are:

- **Step 1**: Loading the dataset
- **Step 2**: Perform a full EDA
- **Step 3**: Build a decision tree
- **Step 4**: Optimize the previous model

There are some slight variations and tips given for each individual project, but they are essentially the same. This is good for us - it means if we can finish one of these project, the others will be much easier. Let's expand on these instructions and generalize them so that you know what to include in you project submission.

## 1. Data loading

1. Load the data into a Pandas dataframe.
2. Look at the features and label names, types and overall amounts of data.
3. Split the data into training and testing features and labels.
4. Encode string features if necessary.

## 2. EDA

### 2.1. Baseline model performance

1. Use cross-validation to determine the model's performance on raw data with default settings.

### 2.2. Missing, and/or extreme values

1. Look at the summary descriptive statistics for each feature.
2. Look at the features distributions using a histogram.
3. Based on the information gained from 1 and 2, note and discuss extreme values or missing data if present.
4. Implement a strategy to deal with missing or extreme values if any.
5. Test the results of your data cleaning with cross-validation.

### 2.3. Feature selection

1. Plot the pairwise correlation between all sets of features.
2. Plot the relationship between each feature and the target variable.
3. Based on your observations in 1 and 2, discuss any pathologies or irrelevant features.
4. Implement a feature selection strategy.
5. Test the results of your feature selection with cross validation.

### 3. Model training

1. Implement the model with defaults and cross-validate it on the fully explored/cleaned data.

### 4. Model optimization

1. Use grid or random search to tune the model's hyperparameters.
2. Cross-validate the model with the optimized hyperparameters to estimate out-of-sample performance.
3. Re-train the optimized model on the complete fully explored/cleaned training data.
4. Evaluate the model's performance on the test set.

### Other tips for good, professional looking notebooks

1. Comment your code - use the '#' symbol to add comments to code blocks. Comments should be short and succinct, telling the reader what each call does.
2. Add explanations using Markdown text. As you move through the project, explain what you are doing at each step and why as well as any observations and conclusions.
3. Take advantage of the outline using Markdown formatting. Jupyter will extract an outline from a notebook that has headings defined. You can then display the outline in the activities panel. This is a great tool to stay organized and guide your reader.
