# House-Price-Prediction
House Price Prediction using Linear Regression with multiple variables

In this project, we implement linear regression with multiple variables to predict the prices of houses.

Problem Statement: 
Suppose you are selling your house and you want to know what a good market price would be. One way to do this is to first collect information on recent houses sold and make a model of housing prices.
About Dataset: The file ex1data2.txt contains a training set of housing prices in Portland, Oregon. The first column is the size of the house (in square feet), the second column is the number of bedrooms, and the third column is the price of the house.

Packages used: pandas, matplotlib, numpy

Note: This problem statement and dataset is from Coursera, Andrew Ng’s machine learning Coursework

Important points to be noted:
1.	Load the dataset and display some values from the dataset. It is observed that house sizes are about 1000 times the number of bedrooms. Since features differs by orders of magnitude, first we need to perform feature scaling to make the gradient descent converge much more quickly. 
When normalizing the features, it is important to store the values used for normalization - the mean value and the standard deviation used for the computations, as we’ll need them later.
2.	Implement the cost function and gradient descent for linear regression with multiple variables. 
3.	Try out different learning rates for the dataset and find a learning rate that converges quickly. (It is advisable to choose 0.3, 0.1, 0.01, 0.03, …)
4.	Run gradient descent for about 50 iterations at the chosen learning rate and also calculate cost function J. Plots the J values against the number of the iterations. 
5.	If we picked a learning rate within a good range, the plot looks similar. If the graph looks very different, especially if the value of J increases or even blows up, then we need to adjust the learning rate and try again.

 ![image](https://user-images.githubusercontent.com/114208254/210999946-84708cdd-3628-4ff0-8c65-00c27b117ccc.png)

6.	With a small learning rate, we found that gradient descent takes a very long time to converge to the optimal value. Conversely, with a large learning rate, gradient descent might not converge or might even diverge!
7.	Predict the price of a house with 1650 square feet and 3 bedrooms. We need to normalize the features when making this prediction!
8.	Use the closed-form solution to linear regression to check the prediction. 
