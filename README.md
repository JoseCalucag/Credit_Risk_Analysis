<h1 align = "center"> Credit_Risk_Analysis </h1>

<p align = "center">
<img src = "https://s3.amazonaws.com/blog.v-comply.com/wp-content/uploads/2017/12/25142550/Credit-Risk.jpg" width = "800" height = "360">
 </p>
 
 
<h2> Overview of the analysis </h2>
Using a credit card dataset from LendingClub, this project will take a look at the factors that can help predict whether someone is a low or high credit risk. We will use the imbalanced-learn and scikit-learn libraries to build models so to then train and evaluate them using various algorthims. Firstly, we applied oversampling algorithms in RandomOverSampler and SMOTE and then used an undersampling algorithm in ClusterCentroids. Next, we used SMOTEENN which combines oversampling and undersampling. Finally, we compared two machine mearning models in BalancedRandomForestClassifier and EasyEnsembleClassifier. Once finished creating a model from each algorthm, we can evaluate the data from a generated report and make a recommendation whether or not the any of these six algorthims should be used to predict credit risk.

<h2> Results </h2> 
# here is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt) <br>
Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. <br>
Use screenshots of your outputs to support your results.

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models

RandomOverSampler <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/ROS.png">
* Balanced accuracy score: 58.0%
* A high risk precision at 1%, a recall value of 45% connected to a f-score of 2%
* A low risk precision at 100%, a recall value of only 71% connected to a f-score of 83%

SMOTE <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/SMOTE.png">
* Balanced accuracy score: 63.9%
* A high risk precision at 1%, a recall value of 54% conneced to a f-score of 2%
* A low risk precision at 100%, a recall value of only 74% connected to a f-score of 85%

ClusterCentroids <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/CC.png">
* Balanced accuracy score: 63.9%
* A high risk precision at 1%, a recall value of 54% conneced to a f-score of 1%
* A low risk precision at 100%, a recall value of only 50% connected to a f-score of 66%

SMOTEENN <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/SMOTEENN.png">
* Balanced accuracy score: 64.8%
* A high risk precision at 1%, a recall value of 62% conneced to a f-score of 2%
* A low risk precision at 100%, a recall value of only 67% connected to a f-score of 80%

BalancedRandomForestClassifier <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/BRFC.png">
* Balanced accuracy score: 74.8%
* A high risk precision at 3%, a recall value of 62% conneced to a f-score of 6%
* A low risk precision at 100%, a recall value of only 88% connected to a f-score of 94%

EasyEnsembleClassifier <br>
<img src = "https://github.com/JoseCalucag/Credit_Risk_Analysis/blob/main/pics/EEC.png">
* Balanced accuracy score: 91.8%
* A high risk precision at 9%, a recall value of 92% conneced to a f-score of 16%
* A low risk precision at 100%, a recall value of only 94% connected to a f-score of 97%


<h2> Summary </h2>
With an overview of our results, we can see that the resapling algorithms are not as reliable; especially looking RandomOverSampling with the lowest accuracy at 58%. Even the oversampling of SMOTE (63.9%), the undersampling of ClusterCentroids (63.9%) and the combined sampling of SMOTEEN (64.8%) pale in campirison to our two other machine learning models. Albeit BalancedRandomForestClassifier has a better score (74.8%), EasyEnsembleClassifier has the best accuracy in 91.8%. Furthermore, EasyEnsembleClassifier also has the best high risk precision in 9%, a recall value of 92% and a f-score of 16%. Therefore, it is to my recommendation to use EasyEnsembleClassifier out of all the models for the highest predicitive accuracy, showing the higest recall value aned f-score in low risk precision for positive samples.
