---
alias: "Inference for Quantitative Data, Means"
subject: "Math"
subset: "Statistics"
importance: 7
type: "AP Guide"
order: 7
---

## The _t_-distribution

- When the population standard deviation σ is unknown, we use the sample standard deviation _s_ as an estimate for σ.
    
- This **_Student’s t-distribution_** _-_ was introduced in 1908 by W. S. Gosset, a British mathematician employed by the Guinness Breweries.
    

For a sample from a _normally distributed population_, we work with the variable

![](https://knowt-user-attachments.s3.amazonaws.com/74d8b3a1721d426f8c15ff3abf141fef.jpeg)

with a resulting _t_-distribution that is bell-shaped and symmetric but lower at the mean, higher at the tails, and so more spread out than the normal distribution.

  

![](https://knowt-user-attachments.s3.amazonaws.com/dfbc99323bf04645a5d1fc9852960022.jpeg)

- The _t_-distribution is different for different values of _n_.
    
- In the tables, these distinct _t_-distributions are associated with the **values for degrees of freedom** (_df_).
    

> For this discussion, the _df_ value is equal to the sample size minus 1. The smaller the _df_ value, the larger the dispersion in the distribution. The larger the _df_ value, that is, the larger the sample size, the closer the distribution to the normal distribution.

- Thus, the _t_-distribution is the proper choice whenever the population standard deviation _σ_ is **unknown**.
    
- In the real world, _σ_ is almost always unknown, and so we should almost always use the _t_-distribution.
    

## Confidence Interval for a Mean

This sample mean is just one of a whole universe of sample means, and we remember that if _n_ is sufficiently large:

1. the set of all sample means is approximately normally distributed.
    
2. the mean of the set of sample means equals _µ_, the mean of the population.
    
3. the standard deviation
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/4d2c1ebb82a04f539f9517d97647dee5.jpeg)
    
    of the set of sample means is approximately equal to
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/b3f9b6da3ee9488c8bb4765fa4bcbcdb.jpeg)
    
    , that is, equal to the standard deviation of the whole population divided by the square root of the sample size.
    

- Typically we do not know _σ_, the population standard deviation. In such cases, we must use _s_, the _standard deviation of the sample_, as an estimate of _σ_.
    
- In this case
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/b0eb95fbe0274c3ca9c22417dc3e7436.jpeg)
    

is called the **_standard error_**

![](https://knowt-user-attachments.s3.amazonaws.com/3f2e0fefc94848c4be71ab2e12944128.jpeg)

, and is used as an estimate for

![](https://knowt-user-attachments.s3.amazonaws.com/d0793ed5056c49e4953329d42f49235c.jpeg)

#### ➥ **Example 7.1**

When a random sample of 10 cars of a new model was tested for gas mileage, the results showed a mean of 27.2 miles per gallon with a standard deviation of 1.8 miles per gallon.

1. What is a 95% confidence interval estimate for the mean gas mileage achieved by this model? (Assume that the population of mpg results for all the new model cars is approximately normally distributed.)
    
2. Based on this confidence interval, do you think that the true mean mileage is significantly different from 25 mpg?
    
3. Determine a 99% confidence interval.
    
4. What would the 95% confidence interval be if the sample mean of 27.2 and standard deviation of 1.8 had come from a sample of 20 cars?
    
5. With the original data
    

![](https://knowt-user-attachments.s3.amazonaws.com/9b2c9bc0270848c5ad5e0e5b7528b99f.jpeg)

, with what confidence can we assert that the true mean gas mileage is 27.2 ± 1.04?

**Solution:**

1. _Parameter:_ Let μ represent the mean gas mileage (in miles per gallon) in the population of cars of a new model.
    

_Procedure:_ A one-sample _t_-interval for a population mean.

_Checks:_ The sample is given to be random, 10 cars are assumed to be less than 10% of all cars of the new model, and the population is stated to be approximately normal. So,

![](https://knowt-user-attachments.s3.amazonaws.com/7958cd6fe47c4908a1dff20ed6962525.jpeg)

follows a _t_-distribution.

_Mechanics:_ Calculator software (such as TInterval on the TI-84 or 1-Sample tInterval on the Casio Prizm) gives (25.912, 28.488).

_Conclusion in context:_ We are 95% confident that the true mean gas mileage of all cars of the new model is between 25.91 and 28.49 miles per gallon.

2. Yes, because 25 is not in the interval of plausible values from 25.9 to 28.5, there is convincing evidence that the true mean mileage is significantly different from 25 mpg.
    
3. Here, TInterval gives (25.35, 29.05). We are 99% confident that the true mean gas mileage of all cars of the new model is between 25.35 and 29.05 miles per gallon. Note that when we want a higher confidence (99% instead of 95%), we have to settle for a larger, less specific interval (±1.85) instead of (±1.29).
    
4. Here, TInterval gives (26.36, 28.04). We are 95% confident that the true mean gas mileage of all cars of the new model is between 26.36 and 28.04 miles per gallon. Note that when the sample size increased (from _n_ = 10 to _n_ = 20), the same sample mean and standard deviation resulted in a narrower, more specific interval (±0.84) instead of (±1.29).
    
5. Converting ±1.04 to _t_-scores yields
    

![](https://knowt-user-attachments.s3.amazonaws.com/0df05c71ceb94faf8b1b2fd7639041c3.jpeg)

and tcdf(-1.827, 1.827, 9) = 0.899 = 89.9%. We are 89.9% confident that the true mean gas mileage of all cars of the new model is between 26.16 and 28.24 miles per gallon.

## Significance Test for a Mean

- To conduct a **_significance test for a mean_**, we must check that we have a _simple random sample_, that the sample size is less than 10% of the population, and that either the sample size is large enough (_n_ ≥ 30) for the CLT to apply or the population has an approximately normal distribution (either stated or if we are given the sample data, a plot should be unimodal and reasonably symmetric, showing no outliers and no skewness).
    

#### ➥ **Example 7.2**

1. A manufacturer claims that a new brand of air-conditioning units uses only 6.5 kilowatts of electricity per day. A consumer agency believes the true figure is higher and runs a test on a random sample of size 50. If the sample mean is 7.0 kilowatts with a standard deviation of 1.4, should the manufacturer’s claim be rejected at a significance level of 5%? Of 1%?
    
2. Given the above conclusion, what type of error, Type-I or Type-II, might have been committed, and what would be a possible consequence?
    

**Solution:**

1. _Parameter:_ Let _μ_ represent the mean electricity usage (in kilowatts per day) of the population of a new brand of air-conditioning unit.
    

_Hypotheses:_ _H_0: _μ_ = 6.5 and _H_a: _μ_ > 6.5.

_Procedure:_ A one-sample _t_-test for a population mean (population SD is unknown).

_Checks:_ We are given a random sample, _n_ = 50 ≥ 30 is large enough for the CLT to apply, and we can assume that 50 is less than 10% of all of the new AC units.

_Mechanics:_ Calculator software (such as T-Test on the TI-84) gives _t_ = 2.525 and _P_ = 0.0074.

_Conclusion in context with linkage to the P-value:_ With this small of a _P_-value, 0.0074 < 0.05, there is convincing evidence to reject _H_0; that is, there is sufficient evidence for the consumer agency to reject the manufacturer’s claim that the new unit uses a mean of only 6.5 kilowatts of electricity per day.

![](https://knowt-user-attachments.s3.amazonaws.com/c40b52698d96446db705f6d5915a2d0a.jpeg)

2. There was sufficient evidence to reject the null hypothesis. If the null hypothesis were true, we would be committing a Type-I error, that is, mistakenly rejecting a true null hypothesis. A possible consequence here is that the consumer agency would discourage customers from purchasing a new brand of air-conditioning unit that really was saving on electricity consumption as advertised.
    

## Confidence Interval for the Difference of Two Means

We have the following information about the sampling distribution of

![](https://knowt-user-attachments.s3.amazonaws.com/2a0cfac310104497943e12440664fbb5.jpeg)

1. The set of all differences of sample means is approximately normally distributed.
    
2. The mean of the set of differences of sample means equals _µ_1 – _µ_2, the difference of population means.
    
3. The standard deviation
    

![](https://knowt-user-attachments.s3.amazonaws.com/b9f6026e5b7b488c990436e0b7561ea9.jpeg)

of the set of differences of sample means is approximately equal to

![](https://knowt-user-attachments.s3.amazonaws.com/424af7da29d34a8e8035964a11f1df22.jpeg)

> When the population standard deviations are unknown, use a _t_-distribution with
> 
> ![](https://knowt-user-attachments.s3.amazonaws.com/c79222597bec402a89e4224b98b18ce7.jpeg)
> 
> . There is the additional condition that either the original populations are roughly normal or the sample sizes are large enough (_n_1 ≥ 30 and _n_2 ≥ 30) for the CLT to apply.

#### ➥ **Example 7.3**

1. A 30-month study is conducted to determine the difference in the numbers of accidents per month occurring in two departments in an assembly plant. Suppose the first department averages 12.3 accidents per month with a standard deviation of 3.5, while the second averages 7.6 accidents with a standard deviation of 3.4. Determine a 95% confidence interval estimate for the mean difference in the numbers of accidents per month. (Assume that the two populations are independent and approximately normally distributed.)
    
2. Based on this confidence interval, do you think that there is a significant mean difference (first department minus second department) in accidents per month between the two departments?
    

**Solution:**

1. Parameters: Let _μ_1 represent the mean number of accidents in the population of the number of accidents in all months for the first department. Let _μ_2 represent the mean number of accidents in the population of the number of accidents in all months for the second department.
    

_Procedure:_ A two-sample _t_-interval for a difference between two population means (first department minus second department).

_Checks:_ We are not given that the sample is random, so we must assume that the 30 months are representative. We are given that the two populations are independent and approximately normal, so a _t_-interval may be found (population SDs are unknown).

_Mechanics:_ Calculator software (such as 2-SampTInt on the TI-84 or 2-Sample tInterval on the Casio Prizm) gives (2.9167, 6.4833).

_Conclusion in context:_ We are 95% confident that the first department has a true mean of between 2.92 and 6.48 more accidents per month than the second department.

2. Yes, because the entire interval from 2.92 to 6.48 is positive, there is convincing evidence that the mean difference in accidents per month between the two departments is significant.
    

## Significance Test for the Difference of Two Means

- A **Significance test for the difference of two means** requires us to check that we have _two independent simple random samples_ and that either the original two populations are roughly normal or the sample sizes are each large enough (_n_1 ≥ 30 and _n_2 ≥ 30) for the CLT to apply.
    

In this situation, the null hypothesis is usually that the means of the populations are the same or, equivalently, that their difference is 0:

![](https://knowt-user-attachments.s3.amazonaws.com/598414dbc65a468496a41459d13a6f48.jpeg)

The alternative hypothesis is then:

![](https://knowt-user-attachments.s3.amazonaws.com/2f1efeac97674b0e91e87185b07417b5.jpeg)

The first two possibilities lead to one-sided tests, and the third possibility leads to two-sided tests.

#### ➥ **Example 7.4**

1. A sales representative believes that the computer his company sells has more average non-operational time per week than a similar model of computer sold by a competitor. Before taking this concern to his director, the sales representative gathers data and runs a significance test. He determines that in a simple random sample of 40 week-long periods at different firms using his company’s product, the average downtime was 125 minutes per week with a standard deviation of 37 minutes. However, 35 week-long periods involving the competitor’s computer yield an average downtime of only 115 minutes per week with a standard deviation of 43 minutes. What conclusion should the sales representative draw?
    
2. Given the above conclusion, what type of error, Type-I or Type-II, might have been committed, and what would be a possible consequence?
    

**Solution:**

1. _Parameters: Let_ μ1 represent the mean of the population of non-operational times of the company's model computer. _Let_ μ2 represent the mean of the population of non-operational times of the competitor's model computer.
    

![](https://knowt-user-attachments.s3.amazonaws.com/fe1c41948c6541b7a0eb6748fd0ff8ae.jpeg)

_Procedure:_ A two-sample _t_-test for the difference of two population means.

_Checks:_ We are given independent SRSs, and the sample sizes are large enough (_n_1 = 40 ≥ 30 and _n_2 = 35 ≥ 30) for the CLT to apply. The population SDs are unknown, so a _t_-test is appropriate.

_Mechanics:_ Calculator software gives _t_ = 1.0718 and _P_ = 0.1438.

_Conclusion in context with linkage to the P-value:_ With this large of a _P_-value, 0.1438 > 0.05, there is not convincing evidence to reject _H_0; that is, the sales representative does not have convincing evidence that his company’s computers have greater mean non-operational time than that of the competitor’s computers.

2. There was not sufficient evidence to reject the null hypothesis. If the null hypothesis were false, we would be committing a Type-II error, that is, mistakenly failing to reject a false null hypothesis. A possible consequence here is that the company’s computers do have a greater mean non-operational time than those of the competitor’s, but because the test doesn’t show this, the company doesn’t make necessary fixes and future sales will suffer.
    

## Paired Data

- When we have a quantitative variable measured twice for the same individual or for two very similar individuals, inference on the true mean difference involves one-sample analysis on the single variable consisting of the differences from the paired data.
    

#### ➥ **Example 7.5**

An SAT preparation class of 30 randomly selected students produces the following total score summary:

![](https://knowt-user-attachments.s3.amazonaws.com/46a9c9fb79a44f0e9d30e9e3d16e1f7b.jpeg)

Find a 90% confidence interval of the mean improvement in test scores.

**Solution:** It would be wrong to calculate a confidence interval for a difference between two means using the means and standard deviations of the first and second scores. The independence condition between the two samples is violated! The proper procedure is a one-sample _t_-interval on the set of differences (improvement) between the scores for each of the 30 students.

_Parameter:_ Let  μ represent the mean improvement (2nd score minus 1st score) in the SAT scores of the population of students who take this SAT preparation class.

_Procedure:_ A one-sample _t_-interval for the mean of a population of differences in paired data.

_Checks:_ We are given a random sample, _n_ = 30 is less than 10% of all students, and _n_ = 30 is large enough so that the CLT applies.

_Mechanics:_ With an unknown population SD, it's necessary to find a _t_-interval.  Using  X̄ = 42.25 and _s_ = 27.92, calculator software (such as TInterval) gives (33.59, 50.91).

_Conclusion in context:_ We are 90% confident that the true mean improvement in test scores is between 33.59 and 50.91.

## Simulations and _P_-Values

- We can use a **simulation** to determine what values of a test statistic are likely to occur by random chance alone, assuming the null hypothesis is true.
    
- Then looking at where our test statistic falls, we can estimate a **_P_****-value**.
    

#### ➥ **Example 7.6**

One measure of variability is the median absolute deviation (MAD). It is defined as the median deviation from the median, that is, as the median of the absolute values of the deviations from the median. A particular industrial product has the following quality control check. Random samples of size 6 are gathered periodically, and measurements are taken of the dimension under observation. If the MAD calculation is significantly greater than what is expected during proper operation of the machinery, a recalibration is necessary. In a simulation of 100 such samples of size 6 from when the machinery is working properly, the resulting MAD calculations are summarized in the following dotplot:

![](https://knowt-user-attachments.s3.amazonaws.com/26a1392e0052406cb82812c4f86051f6.jpeg)

Suppose in a random sample of 6 products the measurements are {8.04, 8.06, 8.10, 8.14, 8.18, 8.19}. Is there sufficient evidence to necessitate a recalibration of the machinery?

**Solution:** The median is

![](https://knowt-user-attachments.s3.amazonaws.com/9a0e76ffaf074e7ebd56cd376a6accbb.jpeg)

. The absolute deviations from the median are {0.08, 0.06, 0.02, 0.02, 0.06, 0.07} with median

![](https://knowt-user-attachments.s3.amazonaws.com/4a0b64a6dc89465eb6a2ed44074ffa47.jpeg)

(the MAD calculation). In the simulation, there were 3 values out of 100 that were 0.06 or greater. This gives an estimated _P_-value of 0.03. With this small of a _P_-value, 0.03 < 0.05, there is sufficient evidence to necessitate a recalibration of the machinery.

## More on Power, Type I Errors, and Type II Errors

- **Type II error** - is a mistaken failure to reject the false null hypothesis, while the **_power_** is the probability of rejecting that false null hypothesis.
    

#### ➥ **Example 7.7**

A candidate claims to have the support of 70% of the people, but you believe that the true figure is lower. You plan to gather an SRS and will reject the 70% claim if your sample shows 65% or less support. What if, in reality, only 63% of the people support the candidate?

![](https://knowt-user-attachments.s3.amazonaws.com/c91d636dd311413b966dc8fc88f8ec36.jpeg)

The upper graph shows the null hypothesis model with the claim that _p_0 = 0.70 and the plan to reject _H_0 if

![](https://knowt-user-attachments.s3.amazonaws.com/dd8da6bb5150428dacda3049e97953bb.jpeg)

The lower graph shows the true model with _p_ = 0.63. When will we fail to recognize that the null hypothesis is incorrect? Answer: precisely when the sample proportion is greater than 0.65. This is a Type II error with probability _β_. When will we rightly conclude that the null hypothesis is incorrect? Answer: when the sample proportion is less than 0.65. This is the "power" of the test and has probability 1 − _β_.

## Confidence Intervals Versus Hypothesis Tests

- A claim about a population parameter indicates a hypothesis test, while an estimate of a population parameter asks for a confidence interval.
    

#### ➥ **Example 7.8**

Suppose it is reported that random samples of 3-point shots by basketball players Stephen Curry and Michael Jordan show a 43% rate for Curry and a 33% rate for Jordan.

(a) Are these numbers parameters or statistics?

(b) State appropriate hypotheses for testing whether the difference is statistically significant.

(c) Suppose the sample sizes were both 100. Find the _z_-statistic and the _P_-value, and give an appropriate conclusion at the 5% significance level.

(d) Calculate and interpret a 95% confidence interval for the difference in population proportions.

(e) Are the test decision and confidence interval consistent with each other?

(f) Repeat (c), (d), and (e) as if the sample size had been 200 for each.

**Solutions:**

(a) These two numbers are statistics because they describe  samples, not all 3-point shots ever taken by these two players.

(b) _H_0: _pCurry_ = _pJordan_ and _Ha_: _pCurry_ ≠ _pJordan_.

(c) Calculator software gives _z_ = 1.46 and _P_ = 0.145. With this large of a _P_-value, 0.145 > 0.05, there is not sufficient evidence to reject _H_0; that is, there is not convincing evidence of a difference in the true 3-point percentage rates of Curry and Jordan.

(d) Calculator software gives (−0.034, 0.234). We are 95% confident that the true difference in 3-point percentage rates (Curry minus Jordan) is between −3.4% and 23.4%.

(e) Yes, they are consistent. We did not conclude that the two percentages differ, and the confidence interval (for the difference in population proportions) includes the value zero.

(f) With a sample size of 200, calculator software gives _z_ = 2.06 and _P_ = 0.039. With this small a _P_-value, 0.039 < 0.05, there is sufficient evidence to reject  _H_0; that is, there is convincing evidence of a difference in the true 3-point percentage rates of Curry and Jordan. With a sample size of 200, calculator software gives a confidence interval of (0.005, 0.195). We are 95% confident that the true difference in 3-point percentage rates (Curry minus Jordan) is between 0.5% and 19.5%. This interval does not include zero, so it is convincing evidence of a difference in the true 3-point percentage rates of Curry and Jordan. This is again consistent with the hypothesis test.