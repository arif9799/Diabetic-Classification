<p align="center">
  
  ___
</p>
<h3 align="center">
  
  [Diabetic Classification, _Supervised ML_](https://github.com/arif9799/Diabetic-Classification)
</h3>
<br>

<p align="center">
  <img src="https://github.com/arif9799/arif9799/blob/main/gifs/DiabeticClassification.gif" width="250" alt="Description">
</p>
<br>

_InsuLens: Focusing Clarity in Diabetic Classification_ 

Cleaned and preprocessed anthropometric datasets with a whopping 1.8 million observations collected from 9 different states in India. Analyzed and performed hyperparameter tuning with 'Grid Search Cross Validation' to derive optimal Parameters for training the MultiLayer Perceptron Classifier to classify the Diabetics. Upsampled the minority class from the imbalanced dataset using SMOTE technique that drastically increased the accuracy of predicting diabetic class from 13% to an impressive 71.4%.
<br>
<br>

In 2019, diabetes caused an estimated 1.5 million deaths in the world with diabetes being the 9th leading cause of death. If identified in early stages, Diabetes is treatable with medication which is expensive. We want to identify a non-invasive and faster diagnosis of diabetes. Hence, this project aims to find out if anthropometric data can be used to identify diabetes in its early stages. We used Multi-Layer Perceptron as our model and Grid Search Cross Validation to help with hyperparameter tuning to get the best precision and recall for the multi-layer perceptron. Our classifier was able to identify non-diabetic patients with 96% accuracy.

The Dataset used for the project comprises of details of clinical, Anthropometric & Bio- chemical Survey collected as an initiative for Annual Health Survey (AHS) conducted in India for 9 states. A bio-marker component was introduced in the AHS to gather data nutritional status and lifestyles of individuals. This Dataset consists of health factors for 48% of the population, 59% of the births in those 9 states, 70% of deaths of infants, 75% deaths of children under the age of 5 and 62% of Maternal deaths. These 9 states were the high focus of Medical sector of the country which led to collection of such vast amount of Data Aggregation.

From this data, the focus of the project, a patient being diabetic or non-diabetic was labelled based on the ‘Fasting blood glucose levels’, which for diabetic patients is 125 or more (hence labeled as ‘1’), ‘0’ otherwise. The overall dataset cumulatively has 1.89 million observations and 53 features. For the project, two subsets of major states, namely UTTAR-PRADESH (UP) and BIHAR (BH) were used which roughly comprised of 800,000 observations. The data contained an enormous number of missing values, which couldn’t be imputed, otherwise would have generated bias in the model prediction. Preprocessing the data, almost 250,000 observations were retained. The target variable is binary class ‘0’ or ‘1’, where 1 indicates a patient being diabetic and 0 indicates a patient being non-diabetic.

**Data Preprocessing:** <br/>
 - Dropping out irrelevant features.
 - Standardizing ‘age’ feature.
 - Average-out variables.
 - Changing Labels of Gender feature.
 - Rounding Off.
 - Feature Engineering.

**Certain Data Visualizations performed to analyze data:** <br/>
  - Correlation Heat Map.
  - Anthropometric Reading contrasted with Response Variable.
  - Gender Contrasted with Anthropometric Data.
  - Density Plots of Anthropometric Data contrasted with Response Variable.
  - Weight and Height w.r.t Response Variable.
  - Effect of Quality of Salt on Diabetes.
  - Distribution of Diabetics/Non-Diabetics (based on age).
  - Count-Plot of Diabetics/Non-Diabetics (based on Gender).
  - Distribution of Hemoglobin for Diabetics and non-diabetics.
  - State-wise Histogram of Diabetics and non-diabetics.

**Data Modeling:** <br/>
Since anthropometric data is being used for the classification of a patient as diabetic or non- diabetic, A Multilayered Perceptron Classifier was decided to be used as the machine learning model for this project.

An illustration of what a simple MLP Classifier instance with one hidden layer looks like is given below,

<p align="center"> 
<img width="360" alt="Picture1" src="https://user-images.githubusercontent.com/93501171/168000519-045e1d50-4bc9-4afc-b6a7-5032f0bda114.png">
</p> 

Each perceptron in it has a weighted sum represented by the equation below,

<p align="center"> 
<img width="360" alt="Picture1" src="https://user-images.githubusercontent.com/93501171/168002099-e62024d3-882b-4ec4-9565-97ef8499bc71.png">
</p> 

And an activation function that returns a probability that ranges from 0 to 1,

<p align="center"> 
<img width="360" alt="Picture1" src="https://user-images.githubusercontent.com/93501171/168000463-bd86716e-5aca-4f5c-b84e-1ad9d94d84a5.png">
</p> 


**Hyperparameter Tuning:**<br />

Hyperparameter tuning was done by Grid search cross validation in order to retrieve the most optimal values for the parameters shown in figure below,

<p align="center"> 
<img width="261" alt="Picture4" src="https://user-images.githubusercontent.com/93501171/168002324-4ed826db-cb8d-45d6-8782-4e0ba30f7f91.png">
</p> 

**Oversampling:** <br />

SMOTE oversampling technique was performed on the data, since the diabetic class was less compared to the non-diabetic ones. The below image shows the evaluation metrics before and after the SMOTE oversampling technique on the optimal hyperparameters.

<p align="center"> 
<img width="843" alt="Screen Shot 2022-05-12 at 2 09 23 AM" src="https://user-images.githubusercontent.com/93501171/168003592-492cd9b6-287a-4dfa-ae0c-2a22570297f7.png">
 </p> 
