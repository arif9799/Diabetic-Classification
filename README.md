# Diabetic-Classification
Classifying a patient as Diabetic or Non-Diabetic based on Anthropometric Data.

In 2019, diabetes caused an estimated 1.5 million deaths in the world with diabetes being the 9th leading cause of death. If identified in early stages, Diabetes is treatable with medication which is expensive. We want to identify a non-invasive and faster diagnosis of diabetes. Hence, this project aims to find out if anthropometric data can be used to identify diabetes in its early stages. We used Multi-Layer Perceptron as our model and Grid Search Cross Validation to help with hyperparameter tuning to get the best precision and recall for the multi-layer perceptron. Our classifier was able to identify non-diabetic patients with 96% accuracy.

The Dataset used for the project comprises of details of clinical, Anthropometric & Bio- chemical Survey collected as an initiative for Annual Health Survey (AHS) conducted in India for 9 states. A bio-marker component was introduced in the AHS to gather data nutritional status and lifestyles of individuals. This Dataset consists of health factors for 48% of the population, 59% of the births in those 9 states, 70% of deaths of infants, 75% deaths of children under the age of 5 and 62% of Maternal deaths. These 9 states were the high focus of Medical sector of the country which led to collection of such vast amount of Data Aggregation.

From this data, the focus of the project, a patient being diabetic or non-diabetic was labelled based on the ‘Fasting blood glucose levels’, which for diabetic patients is 125 or more (hence labeled as ‘1’), ‘0’ otherwise. The overall dataset cumulatively has 1.89 million observations and 53 features. For the project, two subsets of major states, namely UTTAR-PRADESH (UP) and BIHAR (BH) were used which roughly comprised of 800,000 observations. The data contained an enormous number of missing values, which couldn’t be imputed, otherwise would have generated bias in the model prediction. Preprocessing the data, almost 250,000 observations were retained. The target variable is binary class ‘0’ or ‘1’, where 1 indicates a patient being diabetic and 0 indicates a patient being non-diabetic.

Data Preprocessing : 
 - Dropping out irrelevant features.
 - Standardizing ‘age’ feature.
 - Average-out variables.
 - Changing Labels of Gender feature.
 - Rounding Off.
 - Feature Engineering.

Certain Data Visualizations performed to analyze data:
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


