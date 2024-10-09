Binary classification to find undervalued property. 

Models used: random forest(with threshold probability), linear regression, KNN.
Dataset: https://www.kaggle.com/datasets/egorkainov/moscow-housing-price-dataset?resource=download

Classification models are trained with a modified dataset, where in random rows a certain value (delta) is subtracted from the price column and a positive label is placed in a new column (the target feature).

The regression model is trained on the original dataset to predict the price, the test data is modified in the same way as in the classification case, then the predicted values and the test data are compared and if the difference is large enough, the property is labeled undervalued. For a correct classification, the label in the modified test data must match the predicted label.
