# Dataset downloaded from kaggle website

                                Disease dataset as CSV file (training and test datasets)


This article seeks to develop a resilient machine learning model capable of accurately predicting human diseases by efficiently analyzing the symptoms exhibited by individuals.
<br>
<br>

In this project, we have established a well-structured pipeline to execute each step or phase separately, allowing us to concentrate more effectively on each individual stage. The pipeline attached below :


<img src=https://github.com/rezakharamani/DiseasePredictionClassification/blob/main/imagePipeline.png>

<br>
<br>
In the initial step, we work with two distinct datasets: one for training and another for testing. In this phase, we analyze the training data in the CSV files using Matplotlib libraries. Subsequently, we proceed with data modification to ensure cleanliness and readiness for processing, ultimately enabling accurate predictions. The number patients in training dataset is 4921, and for test is 43.


<br></br>
<mark> There are 133 columns in the training dataset that all of them have filled with 0 / 1 values except `target label` filled by string values like AIDS, Diabets, Cancer and so on.</mark>


<br>

`Data Collection:` The first step in tackling any machine learning problem involves preparing the data. In this project, we utilize a dataset sourced from Kaggle, comprising two CSV files for training and testing. The dataset comprises a total of 133 columns, where 132 columns represent symptoms and the last column denotes the prognosis.

`Data Cleansing:` Cleaning the data is a crucial aspect of any machine learning endeavor, as the quality of the data directly influences the model's efficacy. In our dataset, all columns are numerical, with the target column (prognosis) being in string format, and it is transformed into numerical form through label encoding.

`Model Development:` With the data gathered and cleaned, we move on to building machine learning models. The cleaned data is employed to train Support Vector Classifier, Naive Bayes Classifier, and Random Forest Classifier. The quality of these models is assessed using a confusion matrix.

`Inference:` Following the training of the three models, we predict diseases based on input symptoms by combining the predictions from all three models. This approach enhances the overall robustness and accuracy of our predictions.