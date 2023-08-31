## Two Categorical Variables

- Qualitative data often encompass two categorical variables that may or may not have a dependent relationship. These data can be displayed in a **_two-way table_** (also called a **_contingency table_**).
    

#### ➥ **Example 2.1**

_The Cuteness Factor_: A Japanese study had 250 volunteers look at pictures of cute baby animals, adult animals, or tasty-looking foods, before testing their level of focus in solving puzzles.

![](https://knowt-user-attachments.s3.amazonaws.com/ba624f50d97d436ab95e1ad058085469.jpeg)

> The grand total of all cell values, 250 in this example, is called the _table total_.
> 
> Pictures viewed is the _row variable_, whereas level of focus is the _column variable_.

- What percent of the people in the survey viewed tasty foods and had a medium level of focus?
    

![](https://knowt-user-attachments.s3.amazonaws.com/de7bfdd0719945949546dcfa17436f07.jpeg)

The standard method of analyzing the table data involves first calculating the totals for each row and each column.

![](https://knowt-user-attachments.s3.amazonaws.com/dd82edce5f224895ac170a7f1c0833a8.jpeg)

These totals are placed in the right and bottom margins of the table and thus are called **_marginal frequencies_** (or _marginal totals_). These marginal frequencies can then be put in the form of proportions or percentages. The _marginal distribution_ of the level of focus is:

![](https://knowt-user-attachments.s3.amazonaws.com/33252cdab80341d2b6cb3e85b58641db.jpeg)

This distribution can be displayed in a bar graph as follows:

![](https://knowt-user-attachments.s3.amazonaws.com/e97a531abef44f409b9de6ddbc0980a6.jpeg)

Similarly, we can determine the marginal distribution for the pictures viewed:

![](https://knowt-user-attachments.s3.amazonaws.com/075188d7e8884085adb3f0a0ef6ec883.jpeg)

The representative bar graph is:

![](https://knowt-user-attachments.s3.amazonaws.com/a374fa1fb1e340db94d97fe1293d6046.jpeg)

---

## Two Quantitative Variables

- Many important applications of statistics involve examining whether two or more quantitative (numerical) variables are related to one another.
    
- These are also called **bivariate quantitative data sets**.
    
- **Scatterplot** - gives an immediate visual impression of a possible relationship between two variables, while a numerical measurement, called the **correlation coefficien**t - often used as a quantitative value of the strength of a linear relationship. In either case, evidence of a relationship is not evidence of causation.
    

#### ➥ **Example 2.2**

Comic books heroes and villains can be compared with regard to various attributes. The scatterplot below looks at speed (measured on a 20-point scale) versus strength (measured on a 50-point scale) for 17 such characters. Does there appear to be a linear association?

![](https://knowt-user-attachments.s3.amazonaws.com/0ef41d5304f5468489e51b24910b1123.jpeg)

---

- _Positively associated-_ When larger values of one variable are associated with larger values of a second variable.
    
- _Negatively associated -_ When larger values of one are associated with smaller values of the other, the variables are called _negatively associated_.
    

> The strength of the association is gauged by how close the plotted points are to a straight line.

![](https://knowt-user-attachments.s3.amazonaws.com/1a590fca264942cebffdcb39a0b63bf4.jpeg)

![](https://knowt-user-attachments.s3.amazonaws.com/8d7a0382682845a5b27929deea22f8d6.jpeg)

---

> To describe a **scatterplot** you must consider **_form_** (linear or nonlinear), **_direction_** (positive or negative), **_strength_** (weak, moderate, or strong), and **_unusual features_** (such as outliers and clusters). As usual, all answers must also mention **_context_**.  

## Correlation

- Correlation measures the strength of only a _linear_ relationship.
    

Correlation, designated by _r_, has the formula in terms of the means and standard deviations of the two variables.

![](https://knowt-user-attachments.s3.amazonaws.com/c7ac0a2c6528426686aea7184a944f49.jpeg)

The correlation formula gives the following:

- The formula is based on standardized scores (**_z_****-scores**), and so changing units does not change the correlation _r_.
    
- Since the formula does not distinguish between which variable is called _x_ and which is called _y_, interchanging the variables (on the scatterplot) does not change the value of the correlation _r_.
    
- The division in the formula gives that the correlation _r_ is unit-free.
    

> The **value of** **_r_** always falls between −1 and +1, with −1 indicating perfect negative correlation and +1 indicating perfect positive correlation. It should be stressed that a correlation at or near zero does not mean there is not a relationship between the variables; there may still be a strong _nonlinear_ relationship. Additionally, a correlation close to −1 or +1 does not necessarily mean that a linear model is the _most_ appropriate model.

![](https://knowt-user-attachments.s3.amazonaws.com/4c436a363a154f7bb88ccd1148c7b15d.jpeg)

**_r_2** (called the **_coefficient of determination_**) - is the ratio of the variance of the predicted values ŷ to the variance of the observed values _y_.

- That is, there is a partition of the _y_-variance, and _r_2 is the proportion of this variance that is predictable from a knowledge of _x_.
    
- We can say that _r_2 gives the percentage of variation in the response variable, _y_, that is explained by the _variation_ in the explanatory variable, _x_. Or we can say that _r_2 gives the percentage of variation in _y_ that is explained by the linear regression model between _x_ and _y_. In any case, always interpret _r_2 in context of the problem. Remember when calculating _r_ from _r_2 that _r_ may be positive or negative, and that r will always take the same sign as the slope.
    

> Alternatively, _r_2 is 1 minus the proportion of unexplained variance:

![](https://knowt-user-attachments.s3.amazonaws.com/7d5bbbc981d64bc68f273b15b1b505c3.jpeg)

#### ➥ **Example 2.3**

The correlation between Total Points Scored and Total Yards Gained for the 2021 season among a set of college football teams is _r_ = 0.84. What information is given by the coefficient of determination?

**Solution:** _r_2 = (0.84)2 = 0.7056. Thus, 70.56% of the variation in Total Points Scored can be accounted for by (or predicted by or explained by) the linear relationship between Total Points Scored and Total Yards Gained. The other 29.44% of the variation in Total Points Scored remains unexplained.

## Least Squares Regression

What is the best-fitting straight line that can be drawn through a set of points?

![](https://knowt-user-attachments.s3.amazonaws.com/d28666339da24518b76654fcadf67b31.jpeg)

By **_best-fitting straight line_** we mean the straight line that minimizes the sum of the squares of the vertical differences between the observed values and the values predicted by the line.

![](https://knowt-user-attachments.s3.amazonaws.com/a3a9a0ffc5ce4bb2a57f391259135083.jpeg)

That is, in the above figure, we wish to minimize

![](https://knowt-user-attachments.s3.amazonaws.com/526e0d79a81945cea324f033b1f0d820.jpeg)

It is reasonable, intuitive, and correct that the best-fitting line will pass through ( x̄,ȳ), where x̄ and ȳare the means of the variables _X_ and _Y_. Then, from the basic expression for a line with a given slope through a given point, we have:

![](https://knowt-user-attachments.s3.amazonaws.com/437a90e281624186b71b77db4b3c775a.jpeg)

The slope _b_ can be determined from the formula

![](https://knowt-user-attachments.s3.amazonaws.com/8573bb6d0ef0484695fde065a75fd038.jpeg)

where _r_ is the correlation and _s_x and _s_y are the standard deviations of the two sets. That is, each standard deviation change in _x_ results in a change of _r_ standard deviations in ŷ. If you graph _z_-scores for the _y_-variable against _z_-scores for the _x_-variable, the slope of the regression line is precisely _r_, and in fact, the linear equation becomes,

![](https://knowt-user-attachments.s3.amazonaws.com/9750134997084cd6bb7990cf080d9e73.jpeg)

#### **Example 2.4**

A sociologist conducts a survey of 15 teens. The number of "close friends" and the number of times Facebook is checked every evening are noted for each student. Letting _X_ and _Y_ represent the number of close friends and the number of Facebook checks, respectively, gives:

|_X_:|25|23|30|25|20|33|18|21|22|30|26|26|27|29|20|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|_Y_:|10|11|14|12|8|18|9|10|10|15|11|15|12|14|11|

1. Identify the variables.
    
2. Draw a scatterplot.
    
3. Describe the scatterplot.
    
4. What is the equation of the regression line? Interpret the slope in context.
    
5. Interpret the coefficient of determination in context.
    
6. Predict the number of evening Facebook checks for a student with 24 close friends.
    

**Solution:**

1. The explanatory variable, _X_, is the number of close friends and the response variable, _Y_, is the number of evening Facebook checks.
    
2. Plotting the 15 points (25, 10), (23, 11), . . . , (20, 11) gives an intuitive visual impression of the relationship:  
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/4dbf13a495844f388cc716bffe16d8ef.jpeg)
    
3. The relationship between the number of close friends and the number of evening Facebook checks appears to be linear, positive, and strong.
    
4. Calculator software gives ŷ= -1.73 + 0.5492x , where _x_ is the number of close friends and _y_ is the number of evening Facebook checks. We can instead write the following:
    

![](https://knowt-user-attachments.s3.amazonaws.com/7d1e843d8d414e5b936be48c3cd22e6a.jpeg)

5. The slope is 0.5492. Each additional close friend leads to an average of 0.5492 more evening Facebook checks.
    
6. Calculator software gives r = 0.8836, so r2 = 0.78. Thus, 78% of the variation in the number of evening Facebook checks is accounted for by the variation in the number of close friends.
    
7. –1.73 + 0.5492(24) = 11.45 evening Facebook checks. Students with 24 close friends will average 11.45 evening Facebook checks.
    

## Residuals

- Residual - difference between an observed and a predicted value.
    
- When the regression line is graphed on the scatterplot, the residual of a point is the vertical distance the point is from the regression line.
    

![](https://knowt-user-attachments.s3.amazonaws.com/b90ec60401d343eb8ec93ebd89f32010.jpeg)

- A **positive residual** means the linear model _underestimated_ the actual response value.
    
- Negative residual means the linear model _overestimated_ the actual response value.
    

#### ➥ **Example 2.4**

We calculate the predicted values from the regression line in Example 2.13 and subtract from the observed values to obtain the residuals:

|x|30|90|90|75|60|50|
|---|---|---|---|---|---|---|
|y|185|630|585|500|430|400|
|ŷ|220.3|613.3|613.3|515.0|416.8|351.3|
|y-ŷ|–35.3|16.7|–28.3|–15.0|13.2|48.7|

Note that the sum of the residuals is

–35.3 + 16.7 – 28.3 – 15.0 + 13.2 + 48.7 = 0

The above equation is true in general; that is, _the sum and thus the mean of the residuals is always zero_.

## Outliers, Influential Points, and Leverage

- In a scatterplot, **_regression outliers_** are indicated by points falling far away from the overall pattern. That is, outliers are points with relatively large discrepancies between the value of the response variable and a predicted value for the response variable.
    
- In terms of residuals, a point is an outlier if its residual is an outlier in the set of residuals.
    

#### ➥ **Example 2.5**

A scatterplot of grade point average (GPA) versus weekly television time for a group of high school seniors is as follows:

![](https://knowt-user-attachments.s3.amazonaws.com/a557a32419c044038e3cd25376f89e87.jpeg)

> By direct observation of the scatterplot, we note that there are **two outliers**: one person who watches 5 hours of television weekly yet has only a 1.5 GPA, and another person who watches 25 hours weekly yet has a 3.0 GPA. Note also that while the value of 30 weekly hours of television may be considered an outlier for the television hours variable and the 0.5 GPA may be considered an outlier for the GPA variable, the point (30, 0.5) is _not_ an outlier in the regression context because it does not fall off the straight-line pattern.

---

- **Influential Scores** - Scores whose removal would sharply change the regression line. Sometimes this description is restricted to points with extreme _x_-values. An influential score may have a small residual but still have a greater effect on the regression line than scores with possibly larger residuals but average _x_-values.
    

#### ➥ **Example 2.**

Consider the following scatterplot of six points and the regression line:

![](https://knowt-user-attachments.s3.amazonaws.com/c33ecef023fb4c9da9fc5f5cd7fbd29f.jpeg)

> The heavy line in the scatterplot on the left below shows what happens when point _A_ is removed, and the heavy line in the scatterplot on the right below shows what happens when point _B_ is removed.

![](https://knowt-user-attachments.s3.amazonaws.com/642a4783efdd4c809ccda8921deab7c3.jpeg)

> Note that the regression line is greatly affected by the removal of point _A_ but not by the removal of point _B_. Thus, point _A_ is an _influential score_, while point _B_ is not. This is true in spite of the fact that point _A_ is closer to the original regression line than point _B_.

- A point is said to have **_high leverage_** if its _x_-value is far from the mean of the _x_-values. Such a point has the strong potential to change the regression line. If it happens to line up with the pattern of the other points, its inclusion might not influence the equation of the regression line, but it could well strengthen the correlation and _r_2, the coefficient of determination.
    

#### ➥ **Example 2.7**

Consider the four scatterplots below, each with a cluster of points and one additional point separated from the cluster.

![](https://knowt-user-attachments.s3.amazonaws.com/acf7c4409d5c471f95e373d5701f4ef1.jpeg)

- In _A_, the additional point has **high leverage** (its _x_-value is much greater than the mean _x_-value), has a small residual (it fits the overall pattern), and does not appear to be influential (its removal would have little effect on the regression equation).
    
- In _B_, the additional point has **high leverage** (its _x_-value is much greater than the mean _x_-value), probably has a small residual (the regression line would pass close to it), and is very influential (removing it would dramatically change the slope of the regression line to close to 0).
    
- In C, the additional point has **some leverage** (its x-value is greater than the mean x-value but not very much greater), has a large residual compared to other residuals (so it's a regression outlier), and is somewhat influential (its removal would change the slope to more negative).
    
- In D, the additional point has **no leverage** (its x-value appears to be close to the mean x-value), has a large residual compared to other residuals (so it's a regression outlier), and is not influential (its removal would increase the y-intercept very slightly and would have very little if any effect on the slope).
    

## More on Regression

The regression equation

![](https://knowt-user-attachments.s3.amazonaws.com/515b2c71cd714684a4377ddd18070a6f.jpeg)

has important implications.

1. If the correlation _r_ = +1, then
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/a76d20f626564e538fe4c26e37ccde45.jpeg)
    
    , and for each standard deviation _sx_ increase in _x_, the _predicted_ _y_-value increases by _Sy_.
    
2. If, for example, _r_ = +0.4, then
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/51a968fad9204f3986555bf73e919f95.jpeg)
    
    , and for each standard deviation _sx_ increase in _x_, the _predicted_ _y_-value increases by 0.4 _Sy_.
    
    #### ➥ **Example 2.8**
    
    Suppose _x_ = attendance at a movie theater, _y_ = number of boxes of popcorn sold, and we are given that there is a roughly linear relationship between _x_ and _y_. Suppose further we are given the summary statistics:
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/b3902cd5905a41f1bd331c2a26c80b2b.jpeg)
    
    1. When attendance is 250, what is the predicted number of boxes of popcorn sold?
        
    2. When attendance is 295, what is the predicted number of boxes of popcorn sold?
        

![](https://knowt-user-attachments.s3.amazonaws.com/fe1b2a76e8b14df0ad57076a237bc25a.jpeg)

---

3. The regression equation for predicting _x_ from _y_ has the slope:
    

![](https://knowt-user-attachments.s3.amazonaws.com/7b6a8f3751514952aa928e6a94342e95.jpeg)

#### ➥ **Example 2.9**

Use the same attendance and popcorn summary statistics from Example 2.24 above.

1. When 160 boxes of popcorn are sold, what is the predicted attendance?
    
2. When 184 boxes of popcorn are sold, what is the predicted attendance?
    

![](https://knowt-user-attachments.s3.amazonaws.com/74d9e37e55324106a691d0992c6b77ff.jpeg)

## Transformations to Achieve Linearity

- The nonlinear model can sometimes be revealed by transforming one or both of the variables and then noting a linear relationship. Useful transformations often result from using the _log_ or _ln_ buttons on your calculator to create new variables.
    

#### ➥ **Example 2.10**

Consider the following years and corresponding populations:

|Year, _x_:|1980|1990|2000|2010|2020|
|---|---|---|---|---|---|
|Population (1000s), _y_:|44|65|101|150|230|

![](https://knowt-user-attachments.s3.amazonaws.com/c798f7f9d11a46e4be7e738830e75216.jpeg)

> So, 94.3% of the variability in population is accounted for by the linear model. However, the scatterplot and residual plot indicate that a nonlinear relationship would be an even stronger model.

![](https://knowt-user-attachments.s3.amazonaws.com/4fcdbe9f174d45658d3c924eef57427a.jpeg)