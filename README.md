# classifying-social-media-post-real-or-fake-
The dataset is from a shared task of Constraint@AAAI-2021. This task focuses on the detection of COVID19-related fake news in English. The sources of data are various social-media platforms such as Twitter, Facebook, Instagram, etc. Given a social media post, the objective of the shared task is to classify it into either fake or real news. It contains 10600 samples of which 5545 are labeled as real and 5055 are labeled as fake.
Task-1: Prepare dataset.
Use scikit-learn train_test_split with shuffle option to split the dataset into training, validation, and test split. The fraction should be 80/10/10 (train/val/test). Dump the train/val/test split into three csvs and include it with your submission.
Task-2: Preprocessing Social Media Post.
Social media posts contain a lot of crucial information which is not in text-format like emojis, urls, hashtags. You need to carefully preprocess such social media text because filtering out emojis or hashtags might flip the stance of the post. You must go through the following tutorial to understand how you can preprocess social media text.

Task-3: Obtaining vector representations.
In general, inputs to machine learning models are vectors (and not say words). In practice, we use tf-idf representation to encode the input sentences to vectors which are then fed into ML models.

Task-4: Training ML classification models.
You are supposed to build the following basic ML binary classification models, that takes a social media post and classifies into 0:fake and 1:real.
1.K-nearest Neighbor
2.Logistic Regression
3.Support Vector Machine - Linear Kernel
4.K-Means Clustering
5.Neural Networks
6.Ensemble Learning - Gradient Boosting

These ML models are very sensitive to the choice of hyperparameters that these ML models are initialized with. E.g., the K-Nearest Neighbor has two crucial hyperparameters: (i) K —the number of neighbors to consider, and (ii) The choice of metric to identify the K nearest neighbors.

You are expected to tune the hyperparameters involved in each of the Machine Learning Models. This might sound like a humongous task, but thankfully sci-kit learn provides you with a bunch of methods for hyperparameter optimization. 

Task-5: Evaluating Machine Learning Models.
Now that your machine learning models are tuned and ready for evaluation, prepare a report that includes confusion matrix, classification accuracy, f1-score, precision, and recall on the test split that you obtained in Task-1. You can use the classification_report routine of scikit-learn for this task, but for sake of understanding we would recommend writing a routine of your own. Also include the final best set of hyperparameters obtained specific to each model in the report.




















