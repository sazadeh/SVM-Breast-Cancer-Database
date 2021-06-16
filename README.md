# SVM-Breast-Cancer-Database
Classify Breast Cancer Database based on SVM Algorithm (Support Vector Machine)
We try to Implement SVM on 
Data set is downloaded from :
https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Original%29

In this dataset the attributes are:
Attribute Information:

1. Sample code number: id number
2. Clump Thickness: 1 - 10
3. Uniformity of Cell Size: 1 - 10
4. Uniformity of Cell Shape: 1 - 10
5. Marginal Adhesion: 1 - 10
6. Single Epithelial Cell Size: 1 - 10
7. Bare Nuclei: 1 - 10
8. Bland Chromatin: 1 - 10
9. Normal Nucleoli: 1 - 10
10. Mitoses: 1 - 10
11. Class: (2 for benign, 4 for malignant)

When we use SVM it is really important to tune the hyperparameters such as C,d and Kernerls. We used GridSearchCV() for this purpose.

**Note:** Based on the grid search the best Kerner is "Poly" and the best value for C will be 0.001 and degree will be 1.

After training the model,  we make the HeatMap for Test Accuracies and then we have an evaluation model..

The Heatmap figure shows that  the accuracy will decrease when degree of Polynomial kernel increased,also it seems when d is 1 we have better accuracy while increasing the C value and it can lead to overfitting. So based on the above figure the best C will be 0.001 and degree will be 1 and the gamma is 10. When we calculate the accuracy, it will be around 96%.
