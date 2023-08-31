---
alias: "Inference for Quantitative Data, Slopes"
subject: "Math"
subset: "Statistics"
importance: 7
type: "AP Guide"
order: 9
---

## Sampling Distribution for the Slope

- When certain conditions are met, we can model the sampling distribution of the sample slope _b_ with _a_ normal distribution with mean _μb_ and standard deviation _σb_. Working with the standard error _sb_ as an estimate for _σb_ leads to a _t_-distribution with _df_ = _n_ – 2.
    
- If _μy_ is the mean value of the response variable _y_ for _a_ given value of the explanatory variable _x_, then the population regression model is given by _μy_= α + _βx_.
    

The theoretical conditions for inference on the slope are

1. The true relationship between the response and explanatory variables is linear.
    
2. The standard deviation of _y_, _σy_, does not vary with _x_.
    
3. The responses (_y_-values) for each _x_ are approximately normally distributed.
    

> While the above are the theoretical conditions that should be met, we will be working with data from a _single sample_; therefore, we will be approximating the sampling distribution and need to give conditions based on the sample slope _b_, a standard deviation of the sample residuals _s_, and a standard deviation of the sample _x_-values _sx_. Using _s_ and _sx_ as estimates for _σ_ and _σx_, respectively, leads us to estimating _σb_ with _sb_ and a resulting _t_-distribution with _df_ = _n_ – 2. That is, the statistic
> 
> ![](https://knowt-user-attachments.s3.amazonaws.com/643979e734824f26ad2f76190e76590e.jpeg)
> 
> has a _t_-distribution with _df_ = _n_ – 2.

Fortunately,

![](https://knowt-user-attachments.s3.amazonaws.com/297c93e0fd634aa7a99a1bd7bbb31ff9.jpeg)

= standard error of the sample slopes is typically given to you in generic computer output.

## Confidence Interval for the Slope of a Least Squares Regression Line

- The **slope** **_b_** of the regression line and the standard error
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/440148d46d56419cbcba4b316ef30d40.jpeg)
    

of the slope are listed explicitly in the computer output. A confidence interval for _β_ can be found using _t_-scores with _df_ = _n_ − 2.

- If given raw data, a confidence interval can readily be found using the statistical software on a calculator.
    

Conditions for finding a confidence interval for the slope include:

1. The sample must be randomly selected.
    
2. The scatterplot should be approximately linear.
    
3. There should be no apparent pattern in the residuals plot.
    
4. The distribution of the residuals should be approximately normal.
    
5. The sample size _n_ should be less than 10 percent of the population size _N_.
    

#### ➥ **Example 9.1**

Information concerning SAT verbal scores and SAT math scores was collected from 15 randomly selected students. A linear regression performed on the data using a statistical software package produced the following printout:

![](https://knowt-user-attachments.s3.amazonaws.com/956d2403638c45db82099e42f7eb2f90.jpeg)

![](https://knowt-user-attachments.s3.amazonaws.com/83c544c1e13645c991ca04089bcb64fd.jpeg)

1. Assume that all conditions for regression are met. What is the regression equation?
    
2. What is a 95% confidence interval estimate for the slope of the regression line?
    
3. Does the confidence interval (0.64 to 0.89) provide convincing evidence that SAT math scores are linearly related to SAT verbal scores?
    

**Solution:**

1. The _y_-intercept and slope of the equation are found in the **Coef**column of the above printout.  
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/880ab96437ea457a93b473cc7618ac4a.jpeg)
    
2. _Parameter:_ Let _β_ represent the slope of the true regression line for predicting SAT math scores from SAT verbal scores.
    
    _Procedure:_ One-sample _t_-interval for _β_
    
    _Conditions:_ Given that all conditions are met
    
    _Mechanics:_ The standard deviation of the residuals is S = 16.69 and the standard error of the slope is
    

![](https://knowt-user-attachments.s3.amazonaws.com/dcf5a5419fbd4b2c99f026cd31e94d69.jpeg)

With 15 data points, _df_ = 15 − 2 = 13, and the critical _t_-values are ±invT(0.975, 13) = ±2.160. The 95% confidence interval of the true slope is:

![](https://knowt-user-attachments.s3.amazonaws.com/055894de324b42b58050cfa39b8d28bf.jpeg)

_Conclusion in context:_ We are 95% confident that the interval from 0.64 to 0.89 captures the slope of the true regression line relating the SAT math score, _y,_ and SAT verbal score, _x_. (Or we are 95% confident that for every 1-point increase in verbal SAT score, the average increase in math SAT score is between 0.64 and 0.89.) provide convincing evidence that SAT math scores are linearly related to SAT verbal scores?

3. Note that β = 0 would indicate a line with slope 0 is the model for predicting SAT math scores from SAT verbal scores; that is, the model would predict the same SAT math score no matter what the SAT verbal score, and there would not be convincing evidence of a linear relationship.
    

In this example, because the confidence interval (0.64 to 0.89) does not contain 0 as a plausible value of the slope of the population regression line, there is convincing evidence that SAT math and verbal scores are linearly related.

## Hypothesis Test for Slope of Least Squares Regression Line

In addition to finding a confidence interval for the true slope, we can also perform a hypothesis test for the value of the slope. Often we use the null hypothesis _H_0: _β_ = 0, that is, that there is no linear relationship between the two variables.

Assumptions for **inference for the slope** of the least squares line include the following:

1. The sample must be randomly selected.
    
2. The scatterplot should be approximately linear.
    
3. There should be no apparent pattern in the residuals plot.
    
4. The distribution of the residuals should be approximately normal.
    
5. The sample size _n_ should be less than 10 percent of the population size _N_.
    

> Note that a low _P_-value tells us that if the two variables did not have some linear relationship, it would be highly unlikely to find such a random sample. However, **strong evidence that there is some linear association does not mean the association is strong**.

#### ➥ **Example 9.3**

The following table gives serving speeds in mph (using a flat or “cannonball” serve) of ten randomly selected professional tennis players before and after using a newly developed tennis racket.

1. Is there evidence of a _straight-line_ relationship with positive slope between serving speeds of professionals using their old and the new rackets?
    
2. Interpret in context the least squares line.
    

**Solution:**

1. _Parameter_: Let β represent the slope of the true regression line for predicting serving speed in mph after using a newly developed tennis racket from serving speed before using a newly developed tennis racket.
    

_Hypotheses: H_0: _β_ = 0, _H_a: _β_ > 0.

_Procedure:_ _t_-test for the slope of a regression line.

_Checks:_ We are told that the data come from a _random_ sample of professional players, the scatterplot appears to be approximately linear, there is no apparent pattern in the residuals plot, the histogram of residuals appears to be approximately normal, and the sample of size 10 is less than 10% of all professional players.

![](https://knowt-user-attachments.s3.amazonaws.com/74cf350e98e74103913561c2d0ee5358.jpeg)

_Mechanics:_ Using the statistics software on a calculator (for example, LinRegTTest on the TI-84 or LinearReg tTest on the Casio Prizm) gives:

![](https://knowt-user-attachments.s3.amazonaws.com/816cbf36f055458986d73b6e5981bb5b.jpeg)

_Conclusion in context with linkage to the P-value:_

With such a small _P_-value, 0.00019 < 0.05, there is very strong evidence to reject _H_0; that is, there is convincing evidence of a straight-line relationship with positive slope between serving speeds of professionals using their old and the new rackets.

2. With a slope of approximately 1 and a _y_-intercept of 8.76, the regression line indicates that use of the new racket increases serving speed on the average by 8.76 mph regardless of the old racket speed. That is, players with lower and higher old racket speeds experience on the average the same numerical (rather than percentage) increase when using the new racket.