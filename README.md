# Random-Forrest-and-GBDT-implementation
Apply both Random Forrest and GBDT on these feature sets Set 1: categorical(instead of one hot encoding, try response coding: use probability values), numerical features + project_title(BOW) + preprocessed_eassay (BOW) Set 2: categorical(instead of one hot encoding, try response coding: use probability values), numerical features + project_title(TFIDF)+ preprocessed_eassay (TFIDF) Set 3: categorical(instead of one hot encoding, try response coding: use probability values), numerical features + project_title(AVG W2V)+ preprocessed_eassay (AVG W2V). Here for this set take 20K datapoints only. Set 4: categorical(instead of one hot encoding, try response coding: use probability values), numerical features + project_title(TFIDF W2V)+ preprocessed_eassay (TFIDF W2V). Here for this set take 20K datapoints only.  The hyper paramter tuning (Consider any two hyper parameters preferably n_estimators, max_depth) Consider the following range for hyperparameters n_estimators = [10, 50, 100, 150, 200, 300, 500, 1000], max_depth = [2, 3, 4, 5, 6, 7, 8, 9, 10] Find the best hyper parameter which will give the maximum AUC value Find the best hyper paramter using simple cross validation data You can write your own for loops to do this task  Representation of results You need to plot the performance of model both on train data and cross validation data for each hyper parameter, like shown in the figure  with X-axis as n_estimators, Y-axis as max_depth, and Z-axis as AUC Score , we have given the notebook which explains how to plot this 3d plot, you can find it in the same drive 3d_scatter_plot.ipynb or   You need to plot the performance of model both on train data and cross validation data for each hyper parameter, like shown in the figure  seaborn heat maps with rows as n_estimators, columns as max_depth, and values inside the cell representing AUC Score You can choose either of the plotting techniques: 3d plot or heat map Once after you found the best hyper parameter, you need to train your model with it, and find the AUC on test data and plot the ROC curve on both train and test.  Along with plotting ROC curve, you need to print the confusion matrix with predicted and original labels of test data points   Conclusion You need to summarize the results at the end of the notebook, summarize it in the table format. To print out a table please refer to this prettytable library link 
