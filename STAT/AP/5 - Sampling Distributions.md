---
alias: "Sampling Distributions"
subject: "Math"
subset: "Statistics"
importance: 7
type: "AP Guide"
order: 5
---

## Normal Distribution Calculations

- The **normal distribution -** provides a valuable model for how many sample _statistics_ vary, under repeated random sampling from a population.
    
- Calculations involving normal distributions are often made through **_z_****-scores**, which measure **standard deviations** from the **mean**.
    
- On the TI-84, normalcdf(lowerbound, upperbound) gives the area (probability) between two _z_-scores, while invNorm(area) gives the _z_-score with the given area (probability) to the left. The TI-84 also has the capability of working directly with raw scores instead of _z_-scores. In this case, the mean and standard deviation must be given:
    

Normalcdf(lowerbound, upperbound, mean, standard deviation)invNorm(area, mean, standard deviation)

#### ➥ **Example 5.1**

The life expectancy of a particular brand of lightbulb is roughly normally distributed with a mean of 1500 hours and a standard deviation of 75 hours.

  

![](https://knowt-user-attachments.s3.amazonaws.com/74753cad020a4f0ea0757912a488dac5.jpeg)

1. What is the probability that a lightbulb will last less than 1410 hours?
    
2. What is the probability that a lightbulb will last between 1563 and 1648 hours?
    
3. What is the probability that a lightbulb will last between 1416 and 1677 hours?
    

**Solution:**

1. The _z_-score of 1410 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/57d416a0febb4725b2137f37903b0621.jpeg)
    
    On the TI-84, normalcdf(0, 1410, 1500, 75) = 0.1151 and normalcdf(−10, −1.2) = 0.1151.
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/904922853efb446790cf6c8892c79a57.jpeg)
    
2. The _z_-score of 1563 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/8eead107d07a42c5b47aa685df14d308.jpeg)
    
    and the _z_-score of 1648 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/c4eedd35403d44eb91ecc2ee78513d59.jpeg)
    
    Then we calculate the probability of between 1563 and 1648 hours by normalcdf(1563, 1648, 1500, 75) = 0.1762 or normalcdf(0.84, 1.97) = 0.1760.
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/6c752c9e1fe14a918e2f823b1b2148f3.jpeg)
    
    3. The _z_-score of 1416 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/38d2bd83a5744f4fba3e151ef6d1a925.jpeg)
    
    and the _z_-score of 1677 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/28b74d2a95d94f0a815ee00b8f7ff0b9.jpeg)
    
    Then we calculate the probability of between 1416 and 1677 hours by normalcdf(1416, 1677, 1500, 75) = 0.8595 or normalcdf(−1.12, 2.36) = 0.8595.
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/727ba3ea94904b4689342eda7d065242.jpeg)
    

---

To receive full credit for probability calculations using the probability distributions, you need to show:

1. Name of the distribution ("normal" in the example above)
    
2. Parameters ("µ = 1500, σ = 75" in the example above)
    
3. Boundary ("1410" in (a) of the example above)
    
4. Values of interest ("<" in (a) of the example above)
    
5. Correct probability (0.1151 in (a) of the example above)
    

## Central Limit Theorem

The following principle forms the basis of much of what we discuss in this unit and in those following. Statement 1 is called the **_central limit theorem_** **of statistics** (often simply abbreviated as CLT)

Start with a population with a given mean _µ_, a standard deviation _σ_, and any shape distribution whatsoever. Pick _n_ sufficiently large (at least 30), and take all samples of size _n_. Compute the mean of each of these samples:

1. the set of all sample means is approximately normally distributed (often stated: the distribution of sample means is approximately normal).
    
2. the mean of the set of sample means equals _µ_, the mean of the population.
    
3. the standard deviation of the set of sample means is approximately equal to, that is, to the standard deviation of the whole population divided by the square root of the sample size.
    

Alternatively, we say that for sufficiently large _n_, the sampling distribution of x̄ is approximately normal with mean _µ_ and standard deviation.

There are six key ideas to keep in mind:

- Averages vary less than individual values.
    
- Averages based on larger samples vary less than averages based on smaller samples.
    
- The central limit theorem (CLT) states that when the sample size is sufficiently large, the sampling distribution of the mean will be approximately normal.
    
- The larger the sample size _n_, the closer the _sample distribution_ is to the population distribution.
    
- The larger the sample size n, the closer the sampling distribution of x̄ is to a normal distribution.
    
- If the original population has a normal distribution, then the sampling distribution of x̄ has a normal distribution, no matter what the sample size n.
    

#### ➥ **Example 5.2**

1. The naked mole rat, a hairless East African rodent that lives underground, has a life expectancy of 21 years with a standard deviation of 3 years. In a random sample of 40 such rats, what is the probability that the mean life expectancy is between 20 and 22 years?
    
2. The mean life expectancy is at least how many years with a corresponding probability of 0.90?
    

Solution:

We have a random sample that is less than 10% of the naked mole rat population. With a sample size of _n_ = 40 ≥ 30, the central limit theorem applies, and the sampling distribution of x̄ is approximately normal with mean

![](https://knowt-user-attachments.s3.amazonaws.com/12fd0d8defa940a891a441501534e008.jpeg)

and standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/ae912029432446a799cb07bf3a33d89a.jpeg)

The _z_-scores of 20 and 22 are

![](https://knowt-user-attachments.s3.amazonaws.com/579dc64c24e047df9d980ed89c519082.jpeg)

The probability of sample mean between 20 and 22 is normalcdf(–2.110,2.110)= 0.965. [Or normalcdf(20,22,21,0.474)= 0.965.]

![](https://knowt-user-attachments.s3.amazonaws.com/e8117fa5c7944a4db5045ce913b1ecb7.jpeg)

2. The critical _z_-score is invNorm(0.10) = –1.282 with a corresponding raw score of 21 – 1.282(3) = 17.15 years.
    

![](https://knowt-user-attachments.s3.amazonaws.com/28a504ec404c4c3f9de9368d8c15390e.jpeg)

## Biased and Unbiased Estimators

- **_Bias_** means that the sampling distribution is **not** **_centered_** on the population parameter.
    

The sampling distributions of proportions, means, and slopes are **_unbiased_***.* That is, for a given sample size, the set of all **_sample proportions_** is centered on the **_population proportion_**, the set of all **_sample means_** is centered on the **_population mean_**, and the set of all sample slopes is centered on the **_population slope_**.

Here are some illustrative simulations:

![](https://knowt-user-attachments.s3.amazonaws.com/ea9420e6f49049f4981049c14b13a747.jpeg)

the sampling distribution for the maximum is clearly _biased._ That is, for a given sample size, the set of all sample maxima ṽ is not centered on the population maximum, _V_. For example, here is one simulation of sample maxima. Note that _V_ falls far right of the center of the distribution of ṽ.

![](https://knowt-user-attachments.s3.amazonaws.com/31a0d6343fe14810969445c9acf4539d.jpeg)

#### ➥ **Example 5.3**

Five new estimators are being evaluated with regard to quality control in manufacturing professional baseballs of a given weight. Each estimator is tested every day for a month on samples of sizes _n_ = 10, _n_ = 20, and _n_ = 40. The baseballs actually produced that month had a consistent mean weight of 146 grams. The distributions given by each estimator are as follows:

![](https://knowt-user-attachments.s3.amazonaws.com/acd4f47f168b4bdbb4156df9f3a036b3.jpeg)

1. Which of the above appear to be unbiased estimators of the population parameter?
    
2. Which of the above exhibits the lowest variability for _n_ = 40?
    
3. Which of the above is the best estimator if the selected estimator will eventually be used with a sample of size _n_ = 100?
    

Solution:

1. Estimators B, C, and D are unbiased estimators because they appear to have means equal to the population mean of 146. A statistic used to estimate a population parameter is unbiased if the mean of the sampling distribution of the statistic is equal to the true value of the parameter being estimated.
    
2. For _n_ = 40, estimator A exhibits the lowest variability, with a range of only 2 grams compared to the other ranges of 6 grams, 4 grams, 4 grams, and 4 grams, respectively.
    
3. Estimator D because we should choose an unbiased estimator with low variability. From part (a), we have Estimator B, C, and D as unbiased estimators. Now we look at the variability of these three statistics. As _n_ increases, D shows tighter clustering around 146 than does B. Finally, while C looks better than D for _n_ = 40, the estimator will be used with _n_ = 100, and the D distribution is clearly converging as the sample size increases while the C distribution remains the same. Choose Estimator D.
    

## Sampling Distribution for Sample Proportions

- The proportion essentially represents a **_qualitative calculation_**.
    
- The interest is simply in the **_presence or absence_** of some attribute.
    

---

- Suppose the sample size is _n_ and the actual population proportion is _p_. From our work on binomial distributions, we remember that the mean and standard deviation for the number of successes in a given sample are _np_ and √np(1-p), respectively, and for large values of _n_ the complete distribution begins to look “normal.”
    
- Here, however, we are interested in the proportion rather than in the number of successes. From Unit 1, remember that when we multiply or divide every element by a constant, we multiply or divide both the mean and the standard deviation by the same constant. In this case, to change number of successes to proportion of successes, we divide by _n_:
    

![](https://knowt-user-attachments.s3.amazonaws.com/f61359b3d0a14329943f23dc3e1b861a.jpeg)

#### ➥ **Example 5.4**

It is estimated that 80% of people with high math anxiety experience brain activity similar to that experienced under physical pain when anticipating doing a math problem. In a simple random sample of 110 people with high math anxiety, what is the probability that less than 75% experience the physical pain brain activity?

Solution:

The sample is given to be random, both _np_ = (110)(0.80) = 88 ≥ 10 and _n_(1 − _p_) = (110)(0.20) = 22 ≥ 10, and our sample is clearly less than 10% of all people with math anxiety. So, the sampling distribution of p̂ is approximately normal with mean 0.80 and standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/a4a1e63381d74d899db735df1f58ba39.jpeg)

With a z-score of

![](https://knowt-user-attachments.s3.amazonaws.com/0b48370f04ad45f498df327d2f3c8ebb.jpeg)

the probability that the sample proportion is less than 0.75 is normalcdf(–1000,–1.312) = 0.0948.

[Or normalcdf(–1000, 0.75, .80, .0381) = 0.0947.]

![](https://knowt-user-attachments.s3.amazonaws.com/42c37cabf1e24f2e89a91ec30589880a.jpeg)

## Sampling Distribution for Differences in Sample Proportions

- Dealing with one difference from the set of all **possible differences** obtained by subtracting sample proportions of one population from sample proportions of a second population.
    
- To judge the significance of one particular difference, we must first determine how the differences vary among themselves. Remember that the mean of a set of differences is the difference of the means, and the variance of a set of differences is the sum of the variances of the individual sets.
    

![](https://knowt-user-attachments.s3.amazonaws.com/8346dfccc86e48629b7a2787106e2753.jpeg)

With our proportions we have  

![](https://knowt-user-attachments.s3.amazonaws.com/0f328e6d7e054620924a9128268ebc38.jpeg)

 and can calculate:

![](https://knowt-user-attachments.s3.amazonaws.com/b454017883f042878e63805b8b787a7c.jpeg)

#### ➥ **Example 5.5**

In a study of how environment affects our eating habits, scientists revamped one of two nearby fast-food restaurants with table cloths, candlelight, and soft music. They then noted that at the revamped restaurant, customers ate more slowly and 25% left at least 100 calories of food on their plates. At the unrevamped restaurant, customers tended to quickly eat their food and only 19% left at least 100 calories of food on their plates. In a random sample of 110 customers at the revamped restaurant and an independent random sample of 120 customers at the unrevamped restaurant, what is the probability that the difference in the percentages of customers in the revamped setting and the unrevamped setting is more than 10% (where the difference is the revamped restaurant percent minus the unrevamped restaurant percent)?

Solution: We have independent random samples, each less than 10% of all fast-food customers, and we note that _n_1_p_1 = 110(0.25) = 27.5, _n_1(1 − _p_1) = 110(0.75) = 82.5, _n_2_p_2 = 120(0.19) = 22.8, and _n_2(1 − _p_2) = 120(0.81) = 97.2 are all ≥10. Thus, the sampling distribution of p̂1- p̂2 is roughly normal with mean

![](https://knowt-user-attachments.s3.amazonaws.com/016f7bbdcb7246fa9db8e164421837ed.jpeg)

and standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/81c90fedf273437b8bbab0ece6f0159c.jpeg)

The _z_-score of 0.10 is

![](https://knowt-user-attachments.s3.amazonaws.com/55b0cf7619df431e86309e43a090429b.jpeg)

, and normalcdf(0.731,1000)= 0.232. [Or normalcdf(0.10,1.0,0.06,0.0547)= 0.232.]

![](https://knowt-user-attachments.s3.amazonaws.com/cea398acb336436fa4790067da7133a5.jpeg)

## Sampling Distribution for Sample Means

- Suppose the variance of the population is _σ_2 and we are interested in samples of size _n_. Sample means are obtained by first summing together _n_ elements and then dividing by _n_.
    

A set of sums has a variance equal to the sum of the variances associated with the original sets. In our case,

![](https://knowt-user-attachments.s3.amazonaws.com/64ac0f6f7c634d999a30a54cc1d2bc7b.jpeg)

When each element of a set is divided by some constant, the new variance is the old one divided by the square of the constant. Since the sample means are obtained by dividing the sums by _n_, the variance of the sample means is obtained by dividing the variance of the sums by _n_2. Thus, if _σ_x̄ symbolizes the standard deviation of the sample means, we find that:

![](https://knowt-user-attachments.s3.amazonaws.com/8d1cf481b0c64dfcb5912f4de7405e9f.jpeg)

#### ➥ **Example 5.6**

The number of emergency room visits after drinking energy drinks is skyrocketing. One particular energy drink has an average of 200 mg of caffeine with a standard deviation of 10 mg. A store sells boxes of six bottles each. What is the mean and standard deviation of the average milligrams of caffeine consumers should expect from the six bottles in each box?

Solution: We have samples of size 6, and 6 is assumed to be less than 10% of all such bottles. The mean of these sample means will equal the population mean of 200 mg. The standard deviation of these sample means will equal

![](https://knowt-user-attachments.s3.amazonaws.com/872f961c5ef346e99a4ea75cf861f458.jpeg)

 For all random samples of size _n_ = 6 from this population, the sample mean milligrams of caffeine will have a mean of 200 mg and will typically vary by about 4.08 mg from the population mean of 200 mg.

## Sampling Distribution for Differences in Sample Means

- To judge the significance of one particular difference, we must first determine how the differences vary among themselves.
    
- The necessary key is the fact that the variance of a set of differences is equal to the sum of the variances of the individual sets. Thus:
    

![](https://knowt-user-attachments.s3.amazonaws.com/8c04de5b3a2541c0aa2c4fbf014115b3.jpeg)

#### ➥ **Example 5.7**

It is estimated that 40-year-old men contribute an average of 65 genetic mutations to their new children, whereas 20-year-old men contribute an average of only 25. Assuming standard deviations of 15 and 5 mutations, respectively, for the 40- and 20-year-olds, what is the probability that the mean number of mutations in a random sample of thirty-five 40-year-old new fathers is between 35 and 45 more than the mean number in a random sample of forty 20-year-old new fathers?

Solution: We have independent random samples, each less than 10% of their age groups, and both sample sizes are over 30, so the sampling distribution of x̄1-x̄2 is roughly normal with mean

![](https://knowt-user-attachments.s3.amazonaws.com/3b2baaa4aa19422aaa40d1ed17a468f4.jpeg)

and standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/9a07951ea9234a3e95544dbc80a021d2.jpeg)

The _z_-scores of 35 and 45 are

![](https://knowt-user-attachments.s3.amazonaws.com/0ed222aa13ad4e19b35665eb58335e6f.jpeg)

, respectively, and normalcdf(-1.883,1.883)= 0.940. [Or normalcdf(35,45,40,2.656)= 0.940.]

![](https://knowt-user-attachments.s3.amazonaws.com/5cc2469f338846ceb18d1d3e2232b77c.jpeg)

## Simulation of a Sampling Distribution

- The normal distribution can handle sampling distributions of the statistics we are most interested in, namely the sample proportion and sample mean.
    
- If other statistics arise, we can use simulation to obtain a rough idea of the corresponding sampling distributions.
    

For example, a study is made of the number of dreams high school students remember having every night. The median number is 3.41 with a variance of 1.46 and a minimum of 0. Now taking a large number of random samples of 15 students, we calculate the median, variance, and minimum for each sample and graph the resulting simulated sampling distributions.

![](https://knowt-user-attachments.s3.amazonaws.com/9b48771b7c5f49bba6506bd82eb326c7.jpeg)

> The simulated sampling distribution of these medians is roughly bell-shaped, the simulated sampling distribution of the variances is skewed right, and the simulated sampling distribution of the minimums is very roughly bell-shaped.