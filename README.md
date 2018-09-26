# Quartic
## Questions

### Q: Briefly describe the conceptual approach you chose! What are the trade-offs? 
#### A: My approcah was to first analyze the data and see how much values are missing and what type of data it is. After that I checked if data has large deviation or notto decide how to fill the missing values. I tested cross validation predictions on approximately 10 classifiers and after checking their accuracy decided to use 5 Classifiers ensembled in voting classifier to predict the class. I used cross validation so that overfitting can be minimized. Selecting the 5 models above, I used RandomSearchCV to determine best parameters before prediciting the classes. I used RandomSearch because the size of data set is too large and it has too many features so RandomSearch will provide the approximated same result as that of GridSearchCv and it is fast too. For accuracy mean squared error (default) is used. Trade-offs are that It is not clear how derived feature depend on simple features so it will be difficult to do feature engineering. And in some features there were to many values missing approximately all the values were missing.

### Q: What's the model performance? What is the complexity? Where are the bottlenecks? 
#### A: Cross validation scores are very good in some classifiers ranging upto 96%.The biggest bottleneck is the too many missing vales in some features as it can alter the performance of the model.

### Q: If you had more time, what improvements would you make, and in what order of priority? 
#### A: If I had more time, I would have analyzed data more and tried to check if there's any relation between derived features and normal features and how they affect the target. Then after that I would have tried different preprocessing steps like Standardization, Normalization. I would have tried other accuracy meterics such as Recall and precision. After that I would have checked some more models and if they perform better than would have used them in the voting classifier.
