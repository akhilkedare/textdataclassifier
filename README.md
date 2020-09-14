# textdataclassifier
This model was created to classify comments/reviews/feedback/queries into classes.

1. Exploratory data analysis

Dataset comprises of 128956 observations and 3 characteristics.
Data has only object and integer values.
No variable column has null/missing values.
Target variable/Dependent variable is discrete and categorical in nature.
“Class” ranges from A to D.
43946 review/ comments/ queries belongs to class A.
34576 review/ comments/ queries belongs to class B.
31589 review/ comments/ queries belongs to class C.
18845 review/ comments/ queries belongs to class D.

2. Data Cleaning

Removed punctuations from text data.
Converted all uppercase letters to lowercase in text data.
tokenised the text data.
Removed Stopwords, XXXX from text data.
Applied porter stemmer for stemming text data.
Joined tokens to convert sentences.

3. Model Creation

Splitted data into 70 percent training data and 30 percent testing data.
Converted cleaned data into vectors.
Using XGBClassifier as a classifier for model creation.
Gradient boosting is a method that goes through cycles to iteratively add models into an ensemble. Used model gives an accuracy of 89.18 on test data.

4. Hyper parameter tuning

n_estimators are set to 500 for better accuracy.
learning rate is set to 0.05 for better accuracy.
n_jobs is set to 4 for faster perormance.
early_stopping_round is set to 5 to stop detorriating accuracy.

5. Metrics Accuracy_score has been used from sklearn.metrics to check

Accuracy_score has been used from sklearn.metrics to check the accuracy of the model which gave a accuracy of 89.18 percentage.
the accuracy of the model which gave a accuracy of 89.18 percentage.
