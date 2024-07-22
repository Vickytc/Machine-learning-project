Submit_Luxi_Bai.ipynb is my python project file
A2-Data_files is training data set
Kaggle_Supervised_*.csv is my Kaggle test files 
==========================

Submit_Luxi_Bai.ipynb: 
Assignment 2: Predict the Rating of Movies Extracted from the TMDB Database.
==========================
Name：Luxi Bai
Number: 1527822
==========================


1. Read Data and Prepare for next Steps
----------------------------------------------
This part import some necessary packages for this project, which include pandas, numpy, sklearn, scipy, datatime, matplotlib and warnings. Just clicking 'run' can finish this part.

Then, I pre-process some features in these datasets for following training. For example, change feature "original_language" from text feature to numeric feature.


2. Train and Evaluate Supervised Methods of RF, MLP and KNN
----------------------------------------------
This part is eary to test, you could just click each part in order for examination. Results will appear under every single line code from 2.2 to 2.5.

2.1 Define a function to train and evaluate three supervised models: RF, MLP, KNN. Here I use the best parameters I found during the whole process.

2.2 Result of non-text features to train these three models

2.3 Result of textual features use BOW

2.4 Result of textual features use TFIDF

2.5 The Training Result of All Features (Text and Non-text)

Here I can compare if text features will influence the training  result for each model.


3. Baseline models of Zero-R and Random
----------------------------------------------
Just clicking 'run' in order can finish this part.
3.1 Training result of Zero-R baseline model

3.2 Training result of Random baseline model

Baseline models are the lowest performance for effective models. Every model will compare with them.


4. Feature Selection
----------------------------------------------
Select best top N non-text features, and result shows that more features make better model. Therefore, all features are necessary. Just click 'run', results will appear under codes.


5. Self Training with RF, MLP and KNN on All featues, BoW and TFIDF
----------------------------------------------
This part is a compositive part to training semi-supervised models. You need to choose suitable parts for specific model by yourself. Note: every model will cost a lot of times (over 30 mins) to run because of its complexity. 
5.1 Pre-process unlabelled data because of some abnormal values: this part is necessary for all features training. If you want to test BoW or TFIDF, please skip this part and go on section 5.2.

5.2 Prepare training datasets of TFIDF/BoW/All features: you can choose to annotate other parts if you want to test one of them. For example, if you want to test TFIDF part, please annotate BoW and All features part in this section, and click 'run' in order.

5.3 Define a self-learning function for three models: RF/MLP/KNN: this part is core codes for self-training models, please run it before 5.4 every time.

5.4 Train models: choose suitable code and annotate another line. It will cost a lot of times

Here I can get the results of if unlabelled datas will improve model performance.


6. Get Kaggle submission file test_predictions*.csv
----------------------------------------------
According to the experiments above, I finally choose RF as the best model to submit on Kaggle. Here I package it as a CSV file for submission. I have prepared my Kaggle csv files in zip file.


7. RF Model tuning for RF
----------------------------------------------
For better performance of RF, I try to find best parameters of this model in this part. It also need me to adjust some parameters. (include: n_estimators, max_feature, max_depth, min_sample_leaf)

8. Ploting
----------------------------------------------
To polt some necessay pictures for report. Just click 'run' is ok.




