<h1>Student Grades Prediction</h1>

<p>This repository contains the code and analysis for predicting student final grades using various factors. The project involves data loading, preprocessing, exploratory data analysis (EDA), model training, and model evaluation.</p>

<h2>Table of Contents</h2>
<ul>
  <li><a href="#introduction">Introduction</a></li>
  <li><a href="#data-loading-and-preprocessing">Data Loading and Preprocessing</a></li>
  <li><a href="#exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</a></li>
  <li><a href="#model-training">Model Training</a></li>
  <li><a href="#model-evaluation">Model Evaluation</a></li>
  <li><a href="#conclusion">Conclusion</a></li>
</ul>

<h2 id="introduction">Introduction</h2>
<p>The goal of this project is to predict student final grades using a linear regression model. The dataset contains various demographic and behavioral features that could influence academic performance.</p>

<h2 id="data-loading-and-preprocessing">Data Loading and Preprocessing</h2>
<p>Start by loading the data and merging two datasets (math and Portuguese classes) based on common attributes. The data is then cleaned by removing unnecessary columns and handling missing values.</p>

<h2 id="exploratory-data-analysis-eda">Exploratory Data Analysis (EDA)</h2>
<p>During the EDA phase, analyze the data to understand relationships between different variables and the final grades. Some key analyses include:</p>
<ul>
  <li><strong>Gender Comparison:</strong> Comparing final grades between male and female students.</li>
  <li><strong>Study Time vs Final Grades:</strong> Analyzing the impact of study time on final grades.</li>
  <li><strong>Failures vs Final Grades:</strong> Exploring how the number of failures impacts students' final grades.</li>
  <li><strong>Alcohol Consumption vs Final Grades:</strong> Analyzing the effect of alcohol consumption on academic performance.</li>
  <li><strong>Absences vs Final Grades:</strong> Observing the impact of student absences on their final grades.</li>
</ul>

<h2 id="model-training">Model Training</h2>
<p>A linear regression model is trained using the preprocessed data. The dataset is split into training and testing sets, and the model is trained on the training set.</p>

<h2 id="model-evaluation">Model Evaluation</h2>
<p>The model's performance is evaluated using various metrics:</p>
<ul>
  <li><strong>Mean Absolute Error (MAE):</strong> Measures the average magnitude of the errors.</li>
  <li><strong>Mean Squared Error (MSE):</strong> Measures the average of the squares of the errors.</li>
  <li><strong>Root Mean Squared Error (RMSE):</strong> The square root of the average of squared differences.</li>
  <li><strong>R<sup>2</sup> Score:</strong> Represents the proportion of the variance for the dependent variable that's explained by the independent variables.</li>
</ul>

<h3>Performance Metrics</h3>
<ul>
  <li><strong>Mean Absolute Error (MAE):</strong> 3.5465264826446563</li>
  <li><strong>Mean Squared Error (MSE):</strong> 21.428702413016374</li>
  <li><strong>Root Mean Squared Error (RMSE):</strong> 4.629114467781905</li>
  <li><strong>R<sup>2</sup> Score:</strong> 0.006027261013986318</li>
</ul>

<h3>Evaluation and Commentary</h3>
<p>The model shows poor performance with an R<sup>2</sup> score of 0.006 and error metrics (MAE, MSE, RMSE) indicating significant discrepancies between predicted and actual values. These results can usually occur due to the following reasons:</p>
<ol>
    <li><strong>Model Underfitting:</strong> The model has not captured the underlying patterns in the training data and performs poorly on the test data. In this case, the model may not be complex enough.</li>
    <li><strong>Data Complexity:</strong> There might be a non-linear or complex relationship between the independent and dependent variables, which the linear model could not capture.</li>
    <li><strong>Insufficient Features:</strong> The features used in the model may not be sufficient to accurately predict the dependent variable.</li>
</ol>

<h4>R<sup>2</sup> Score and Error Metrics</h4>
<ul>
    <li><strong>Mean Absolute Error (MAE):</strong> Measures the average magnitude of the errors in a set of predictions, without considering their direction. A higher value indicates less accurate predictions.</li>
    <li><strong>Mean Squared Error (MSE):</strong> Measures the average of the squares of the errors—that is, the average squared difference between the estimated values and what is estimated. A higher value indicates the model is making larger errors.</li>
    <li><strong>Root Mean Squared Error (RMSE):</strong> The square root of the average of squared differences between prediction and actual observation. A higher value indicates larger errors and poor model performance.</li>
    <li><strong>R<sup>2</sup> Score:</strong> A statistical measure that represents the proportion of the variance for a dependent variable that's explained by an independent variable or variables in a regression model. An R<sup>2</sup> score close to 0 indicates the model does not explain much of the variance.</li>
</ul>

<h2 id="conclusion">Conclusion</h2>
<p>This project demonstrates the application of a linear regression model to predict student final grades. The model showed poor performance with the current data, indicating the need for further feature engineering and model improvement.</p>
