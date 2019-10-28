# DS5500-Assignment-2

## Problem 2

## Problem 3

## Problem 4
For seeing the relationship between income and life expectancy I plotted a scatter plot of Life expectancy against GDP to see how they are correlated. Looking at the plot we see that as we increase the income over certain range the life expectancy increases as well and after a certain point, it almost is constant as expected. 
The blue scatters represents the actual Y which is the life expectancy over income. The Yellow line represents the linear fit for the variable Life expectancy over GDP income. We can see that it fails to actually establish a correct representation between the variable. So does the 2nd degree and 3rd-degree polynomial regressor.

#### Plot for life expectancy over income gdp
![alt text](assets/q1_a.png)


The mean square error i got for all the regressors are as follows
    
    Mean square error for linear 1st-degree linear regression: 178.20974789819934
    Mean square error for linear 2nd-degree linear regression: 129.81171346584082
    Mean square error for linear 3rd-degree linear regression: 105.52296176335349

We can see that the mean square error decreases as we increase the degree of the polynomial but still the error is high


#### Residual plot for life expectancy over income gdp
![alt text](assets/q1_b.png)

For each residual wee can see that it is moving away from 0 and thereby increase the error


#### Further Analysis

Looking at the plot of life expectancy over income we see some form of log relation between them and both are variables that are directly proportional to each other as we see that if the income increases the life expectancy increases. 
So to see the logarithmic relation i fit the models with log-transformed Income GDP and observed the result.
 
Looking at the plot we can see that the lines for all the regressors are better fitting the relationship between life expectancy and income GDP. The 3rd-degree regressor over the log(income-GDP) fits the life expectancy best in comparison to all the models.

#### Plot for life expectancy fitter over log transformed income gdp
![alt text](assets/q1_c.png)

The mean square error for the new regressor got for all the regressors are as follows

    Mean square error for linear 1st-degree linear regression: 87.18455865550399
    Mean square error for linear 2nd-degree linear regression: 87.1171175681947
    Mean square error for linear 3rd-degree linear regression: 80.18137845255467

we can see that For all the regressor the mean square error has gone down for all the regressors.

#### Residual plot for life expectancy over income gdp
![alt text](assets/q1_d.png)

The residual for the third degree is close to 0 and better than all the resistors some of this may be because the model is overfitted a bit.

#### Relationship with respect to time.


If we introduce time in the above we see that the prediction becomes better. This is because time introduces a new dimension to the prediction by capturing the trends of how there has been an improvement in both income and life expectancy over time. This basically may show better medical equipment, quality of life etc over time.

We see each regressor better captures the relation than any of the above models.

#### Plot for life expectancy fitter over log transformed income gdp with respect to time
![alt text](assets/q1_e.png)

The mean square error for the are as follows

    Mean square error for linear 1st-degree linear regression: 55.79034619374027
    Mean square error for linear 2nd-degree linear regression: 36.18285625361796
    Mean square error for linear 3rd-degree linear regression: 32.491320843692016


we can see that for all the regressor the mean square error has gone down significantly less than the previous regressors.

![alt text](assets/q1_f.png)

Also looking at the residual the third-degree polynomial is closer toward 0 than any other regressor above.


## Problem 5

To see the relation here i plotted the child mortality over income similar to above with color blue as actual child mortality rate and yellow, green and red respectively for 1st, 2nd, and 3rd-degree regressor.

In the below plot we see that all the regressor lines are way off in representing the relation between both the variable. Also, we see that child mortality is inversely proportional to income. As income increase the child mortality rate decreases.

#### Plot for child mortality over income gdp
![alt text](assets/q2_1.png)

The mean square for the above regressor is as followed

    Mean square error for linear 1st-degree linear regression: 20077.780836437614
    Mean square error for linear 2nd-degree linear regression: 15595.930038339211
    Mean square error for linear 3rd-degree linear regression: 12728.78264364586

#### Residual plot for child mortality over income gdp
![alt text](assets/q2_2.png)

For each residual, we can see that the error is huge 

#### Further Analysis

As discussed above we saw that the relation between mortality rate and income as inversely proportional to each other. And also there is a logarithmic relation too. So I transformed income as a reciprocal of log income. 

    X = 1 / log(x)

Plotting the relationship shows that the models with the transformation fit the relationship. In particular, the 3rd-degree polynomial fits the best. One reason maybe it's just overestimating the relation.

#### Plot for child mortality over income GDP with reciprocal log transformation
![alt text](assets/q2_3.png)



The mean square error for the models are as followed

    Mean square error for linear 1st-degree linear regression: 10252.523752002628
    Mean square error for linear 2nd-degree linear regression: 9731.74603221738
    Mean square error for linear 3rd-degree linear regression: 9118.267658465405

The mean square errors significantly reduced and the models became better at understanding the relation between income GDP and child mortality rate.

The residual of the models can be seen in this plot

#### Residual plot for child mortality over income GDP with reciprocal log transformation

![alt text](assets/q2_4.png)


We see that the errors have reduced for all models and the predictions have improved.


#### Time Analysis

To see the involvement of time I build the same model with time as input too. Doing this I observed the estimation improved. This is expected as over time there has been an advancement in technology, medicine etc which was captured when including time as a variable. The below plot shows this relation.


#### Plot for child mortality over income GDP with reciprocal log transformation with respect to time

![alt text](assets/q2_5.png)

The mean square error of the plots is as followed.

    Mean square error for linear 1st-degree linear regression: 6156.205105344115
    Mean square error for linear 2nd-degree linear regression: 4325.340808813144
    Mean square error for linear 3rd-degree linear regression: 3731.6064446445944

The mean squared error, as usual, have reduced significantly as compared to the above build models.

#### Residual Plot for child mortality over income GDP with reciprocal log transformation with respect to time

![alt text](assets/q2_6.png)

Residual Plot shows decrease in error for all model hence improving the estimation
