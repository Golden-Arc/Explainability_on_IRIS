# Explainability_on_IRIS
* This is the repository for Group 1 experiment on the explainability by using LIME and SHAP
* Group Member: YANG Xiaoran, LUAN Qifeng, DONG Yicheng, PENG Xiuya

## Experiment 1: Global Explainability by using SHAP
* The explnation of SHAP shows the Global Explainability
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/global.png)

* Analysis: Globally, sepal length contributes the most positive effect in the prediction as well as petal length and sepal width contributes some negative effects.

## Experiment 2: Comparison between Local Explainability on Different ML Model by using LIME
* Result on Random Forest (Correct Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/randomforest.png)

* Result on SVM (Correct Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/svm.png)

* Result on Logistic Regression (Correct Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/LR.png)

* Result on KNN (Wrong Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/KNN.png)

* Result on Naive Bayes (Wrong Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/NB.png)

* Result on MLP (Wrong Prediction)
![Image](https://github.com/Golden-Arc/Explainability_on_IRIS/blob/main/figure/MLP.png)

* Analysis: 
  1. According to the prediction results, Random Forest, SVM and Logistic Regression give the correct answer. But other models have provided false predictions.
  2. There are some patterns, such as petal length and petal width are always the main contributors to the prediction of versicolor class. However, due to the local instability of LIME itself, the contributions of each feature are not exactly the same.
  3. For the wrong prediction, petal width and sepal width are always the main disturbance of the model.