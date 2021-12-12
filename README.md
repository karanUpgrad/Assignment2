# Bike Sharing Liniar regression model
> A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 




## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

- We have used concents from Multiple Liniar Regressiion and made use of concepts such as RFE ( recursive feature elimination ) and OLS ( ordinary least sqaure ) to predict the values of bikes thats that can be taken up on hire based on various predictors 
-

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
 Using the concents from multiple regression we have created a training set of data and have found the parameters 'yr', 'holiday', 'temp', 'season_winter', 'mnth_mar',
       'mnth_may', 'mnth_sept', 'weathersit_bad', 'weathersit_good' after multiple iterations where we compared the VIF ( Variance Inflation Factor ) and P values. Since we wanted a very strong model we removed any sort of multicollinearity by checking the heat map and the removing any factor that had a VIF value that was above 3 or any p value that has a value above 0.05 eventually our model was built to perfection. 
      
-  we then performed the preiction on the training data using a regression model and found the y train pred value, subtracting the y train value to the y train pred value we found that the Errors are normally distribured here with mean 0. So everything seems to be fine
- We also founf the r_sqared value using this test analisys and noticed it was very close to the value from our final OLS model 
- We then created a y test pred and found that the r2_square value was almost similiar to the values from the training data which suggested a training set of 70-30 with random state set to 42 percent was an ideal fit 
-  we lastly checked for homoscedasticity and found that the model passed the requirement. 
- we have used the data provided from the company in the file Day.csv




## Technologies Used
- numpy
- pandas
- matplotlib
- seaborn
- sklearn
- statsmodels


<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Inferences
   The columns that we have taken into accoutn are - 'yr', 'holiday', 'temp', 'season_winter', 'mnth_mar',
       'mnth_may', 'mnth_sept', 'weathersit_bad', 'weathersit_good'
       
       The paramaters are as follows 
 -yr                 1963.721014
- holiday            -733.958256
- temp               5226.419951
- season_winter      1177.664827
- mnth_mar            476.054416
- mnth_may            631.773577
- mnth_sept           695.586595
- weathersit_bad    -1579.615781
- weathersit_good     661.110959

The  R-squared value is as follow -   0.799




