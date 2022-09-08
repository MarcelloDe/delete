---
layout: post
title: "IBM Data Science Certification: Data Analysis Project"
subtitle: "Project Spotlight"
date: 2022-09-22 12:42
---

<h1> Data Analysis Assignment: House Sales in King County, USA </h1>

<p>In this assignment, you will analyse and predict housing prices using attributes or features such as square footage, number of bedrooms, number of floors and so on.</p>

<p>We will be analyzing this dataset: <a href="https://s3-api.us-geo.objectstorage.softlayer.net/cf-courses-data/CognitiveClass/DA0101EN/coursera/project/kc_house_data_NaN.csv">House Sales in King County, USA</a></p>


<p>This report provides details of our attempt to predict house prices using various regression methods. We will make use of data of house prices in King County, Washington State, USA for sales in 2014 and 2015.</p>

<p>
Our main, predictive question is:&ldquo;Is it possible to predict the sale price of a house from information about that house such as the size, number of bedrooms, condition etc?&rdquo;</p>

<h2>The Dataset </h2>
<p> The dataset contains house sale prices for King County, which includes Seattle. It includes home sold between May 2014 and May 2015</p>

<p><b>id </b>:a notation for a house</p>

<p> <b>date</b>: Date house was sold</p>

<p>
<b>price</b>: Price is prediction target</p>

<p>
<b>bedrooms</b>: Number of Bedrooms/House</p>

<p>
<b>bathrooms</b>: Number of bathrooms/bedrooms</p>

<p><b>sqft_living</b>: square footage of the home</p>

<p><b>sqft_lot</b>: square footage of the lot</p>

<p>
<b>floors </b>:Total floors (levels) in house</p>

<p>
<b>waterfront</b>: House which has a view to a waterfront</p>

<p>
<b>view</b>: Has been viewed</p>

<p>
<b>condition</b>: :How good the condition is Overall</p>

<p><b>grade</b>: overall grade given to the housing unit, based on King County grading system</p>

<p>
<b>sqft_above </b>:square footage of house apart from basement</p>

<p>
<b>sqft_basement</b>: square footage of the basement</p>

<p><b>yr_built</b>: Built Year</p>

<p>
<b>yr_renovated </b>:Year when house was renovated</p>

<p><b>zipcode</b>:zip code</p>

<p>
<b>lat: Latitude coordinate</p>

<p><b>long</b>: Longitude coordinate</p>

<p><b>sqft_living15</b>: Living room area in 2015(implies-- some renovations) This might or might not have affected the lotsize area</p>

<p>
sqft_lot15</b>: lotSize area in 2015(implies-- some renovations)</p>

<h2> The Questions </h2>

<p>
Question 1) Display the data types of each column using the attribute dtype, then take a screenshot and submit it, include your code in the image.</p>

 <img src="/assets/images/Ibm6/1.jpg">

<p>Question 2) Drop the columns &quot;id&quot; and &quot;Unnamed: 0&quot; from axis 1 using the method drop(), then use the method describe() to obtain a statistical summary of the data.</p>

 <img src="/assets/images/Ibm6/2.jpg">

<p>Question 3 use the method value_counts to count the number of houses with unique floor values, use the method .to_frame() to convert it to a dataframe.</p>

 <img src="/assets/images/Ibm6/3.jpg">

<p>Question 4 use the function boxplot in the seaborn library to produce a plot that can be used to determine whether houses with a waterfront view or without a waterfront view have more price outliers.</p>

 <img src="/assets/images/Ibm6/4.jpg">

<p>Question 5 Use the function regplot in the seaborn library to determine if the feature sqft_above is negatively or positively correlated with price</p>

 <img src="/assets/images/Ibm6/5.jpg">

<p>Question 6 Fit a linear regression model to predict the price using the feature 'sqft_living' then calculate the R^2. Take a screenshot of your code and the value of the R^2.</p>

 <img src="/assets/images/Ibm6/6.jpg">

<p> Question 7 Fit a linear regression model to predict the 'price' using the list of features:<br>
&bull; &quot;floors&quot;<br>
&bull; &quot;waterfront&quot;<br>
&bull; &quot;lat&quot;<br>
&bull; &quot;bedrooms&quot;<br>
&bull; &quot;sqft_basement&quot;<br>
&bull; &quot;view&quot;<br>
&bull; &quot;bathrooms&quot;<br>
&bull; &quot;sqft_living15&quot;<br>
&bull; &quot;sqft_above&quot;<br>
&bull; &quot;grade&quot;<br>
&bull; &quot;sqft_living&quot;</p>

 <img src="/assets/images/Ibm6/7.jpg">

<p>Question 8 Create a pipeline object that scales the data performs a polynomial transform and fits a linear regression model. Fit the object using the features in the question above, then fit the model and calculate the R^2. Take a screenshot of your code and the R^2.</p>

 <img src="/assets/images/Ibm6/8.jpg">

<p>Question 9 Create and fit a Ridge regression object using the training data, setting the regularization parameter to 0.1 and calculate the R^2 using the test data. Take a screenshot for your code and the R^2</p>

 <img src="/assets/images/Ibm6/9.jpg">

<p>Question 10 Perform a second order polynomial transform on both the training data and testing data. Create and fit a Ridge regression object using the training data, setting the regularisation parameter to 0.1. Calculate the R^2 utilising the test data provided. Take a screenshot of your code and the R^2.</p>

 <img src="/assets/images/Ibm6/10.jpg">