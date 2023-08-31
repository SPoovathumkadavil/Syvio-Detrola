---
alias: "Inference for Categorical Data, Proportions"
subject: "Math"
subset: "Statistics"
importance: 7
type: "AP Guide"
order: 6
---

## The Meaning of a Confidence Interval

- The **_percentage_** is the percentage of samples that would pinpoint the unknown **_p_** or **_µ_** within plus or minus respective margins of error.
    
- For a given sample proportion or mean, _p_ or _µ_ either is or isn’t within the specified interval, and so the probability is either 1 or 0.
    

**Two aspects to this concept:**

- First, there is the confidence interval, usually expressed in the form:
    

![](https://knowt-user-attachments.s3.amazonaws.com/8de8b315186144a9814fa395c4f380a9.jpeg)

- Second, there is the **_success rate for the method_**, called the **_confidence level_**, that is, the proportion of times repeated applications of this method would capture the true population parameter.
    

- The **_standard error_** is a measure of how far the sample statistic typically varies from the population parameter.
    
- The **_margin of error_** is a multiple of the standard error, with that multiple determined by how confident we wish to be of our procedure.
    

> All of the above assume that certain conditions are met. For inference on population proportions, means, and slopes, we must check for independence in data collection methods and for selection of the appropriate sampling distribution.

## Conditions for Inference

The following are the **_two standard assumptions_** for our inference procedures and the "ideal" way they are met:

1. **Independence assumption:**
    

- Individuals in a sample or an experiment an must be independent of each other, and this is obtained through **random sampling** or **random selection**.
    
- Independence across samples is obtained by selecting **two** (or more) **separate random samples**.
    
- Always examine how the data were collected to check if the assumption of independence is reasonable.
    
- Sample size can also affect independence. Because sampling is usually done without replacement, if the sample is too large, lack of independence becomes a concern.
    
- So, we typically require that the sample size _n_ be no larger than 10% of the population (the 10% Rule).
    

2. **Normality assumption:**
    

- **Inference for proportions** is based on a normal model for the sampling distribution of p̂, but actually we have a binomial distribution.
    
- Fortunately, the binomial is approximately normal if both _np_ and _nq_ ≥ 10.
    
- **Inference for means** is based on a normal model for the sampling distribution of x̄; this is true if the population is normal and is approximately true (thanks to the CLT) if the sample size is large enough (typically we accept _n_ ≥ 30).
    
- With regard to means, this is referred to as the **_Normal/Large Sample_** condition.
    

#### ➥ **Example 6.1**

If we pick a simple random sample of size 80 from a large population, which of the following values of the population proportion _p_ would allow use of the normal model for the sampling distribution of p̂?

1. 0.10
    
2. 0.15
    
3. 0.90
    
4. 0.95
    
5. 0.99
    

**Solution:** **(B)**

- The relevant condition is that both _np_ and _nq_ ≥ 10.
    
- In (A), _np_ = (80)(0.10) = 8; in (C), _nq_ = (80)(0.10) = 8; in (D), _nq_ = (80)(0.05) = 4; and in (E), _nq_ = (80)(0.01) = 0.8. However, in (B), _np_ = (80)(0.15) = 12 and _nq_ = (0.85)(80) = 68 are both ≥ 10.
    

## Confidence Interval for a Proportion

- Estimating a population proportion _p_ by considering a single sample proportion p̂.
    

This sample proportion is just one of a whole universe of sample proportions, and from Unit 5 we remember the following:

1. The set of all sample proportions is approximately normally distributed.
    
2. The mean _μ_p̂ of the set of sample proportions equals _p_, the population proportion.
    
3. The standard deviation σp̂ of the set of sample proportions is approximately equal to
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/d038bb28e33a479c9a434799f2bf5d4b.jpeg)
    

- In finding confidence interval estimates of the population proportion p, how do we find
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/2b0192ee103f40179b6fc756ba57efba.jpeg)
    

since _p_ is unknown? The reasonable procedure is to use the sample proportion p̂:

![](https://knowt-user-attachments.s3.amazonaws.com/af78aed1a7294fea974e4d85ec2e64a1.jpeg)

- When the standard deviation is estimated in this way (using the sample), we use the term _standard error_:
    

![](https://knowt-user-attachments.s3.amazonaws.com/a184028fe01a4ca8b6f387ac37e164d1.jpeg)

➥ **Example 6.2**

1. If 42% of a simple random sample of 550 young adults say that whoever asks for the date should pay for the first date, determine a 99% confidence interval estimate for the true proportion of all young adults who would say that whoever asks for the date should pay for the first date.
    
2. Does this confidence interval give convincing evidence in support of the claim that fewer than 50% of young adults would say that whoever asks for the date should pay for the first date?  
    

**Solution:**

1. The parameter is _p_, which represents the proportion of the population of young adults who would say that whoever asks for the date should pay for the first date. We check that
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/42ddf8aa46f545d5b073563694bb8701.jpeg)
    

![](https://knowt-user-attachments.s3.amazonaws.com/1495c8f5562e4db2bc646f84437fca71.jpeg)

- We are given that the sample is an SRS, and 550 is clearly less than 10% of all young adults. Since p̂ = 0.42, the standard error of the set of sample proportions is
    

![](https://knowt-user-attachments.s3.amazonaws.com/63547c65f3b646bbb0dca88a0af435f5.jpeg)

- 99% of the sample proportions should be within 2.576 standard deviations of the population proportion. Equivalently, we are 99% certain that the population proportion is within 2.576 standard deviations of any sample proportion.
    
- Thus, the 99% confidence interval estimate for the population proportion is 0.42 ± 2.576(0.021) = 0.42 ± 0.054. We say that the _margin of error_ is ±**0.054**. We are 99% confident that the true proportion of young adults who would say that whoever asks for the date should pay for the first date is between 0.366 and 0.474.
    

2. Yes, because all the values in the confidence interval (0.366 to 0.474) are less than 0.50, this confidence interval gives convincing evidence in support of the claim that fewer than 50% of young adults would say that whoever asks for the date should pay for the first date.
    

## Logic of Significance Testing

- Closely related to the problem of estimating a population proportion or mean is the problem of testing a hypothesis about a population proportion or mean.
    
- The **general testing procedure** is to choose a specific hypothesis to be tested, called the **_null hypothesis_**, pick an appropriate random sample, and then use measurements from the sample to determine the likelihood of the null hypothesis.
    
- If the sample statistic is far enough away from the claimed population parameter, we say that there is sufficient evidence to reject the null hypothesis. We attempt to show that the null hypothesis is unacceptable by showing that it is improbable.
    

The **_null hypothesis_** _H_0 is stated in the form of an equality statement about the _population_ proportion (for example, _H_0: _p_ = 0.37).

- There is an **_alternative hypothesis_**, stated in the form of a strict inequality (for example, _H_a: _p_ < 0.37 or _H_a: _p_ > 0.37 or _H_a: _p_ ≠ 0.37).
    
- The strength of the **sample statistic p̂** can be gauged through its associated P-value, which is the probability of obtaining a sample statistic as extreme (or more extreme) as the one obtained if the null hypothesis is assumed to be true. The smaller the P-value, the more significant the difference between the null hypothesis and the sample results.
    

  
There are two types of possible errors:

1. the error of mistakenly rejecting a true null hypothesis.
    
2. the error of mistakenly failing to reject a false null hypothesis.
    

- The **α-risk**, also called the **significance level of the test**, is the probability of committing a **_Type I error_** and mistakenly rejecting a true null hypothesis.
    
- **_Type II error_** - a mistaken failure to reject a false null hypothesis, has associated probability _β_.
    

There is a different value of β for each possible correct value for the population parameter p. For each β, 1 − β is called the **"power" of the test** against the associated correct value.

- **Power of a hypothesis test** - is the probability that a **Type II error** is not committed.
    

That is, given a true alternative, the power is the probability of rejecting the false null hypothesis. Increasing the sample size and increasing the significance level are both ways of increasing the power.  Also note that a true null that is further away from the hypothesized null is more likely to be detected, thus offering a more powerful test.

---

![](https://knowt-user-attachments.s3.amazonaws.com/0d46395def0d4cc98cbffc349cbb3e4e.jpeg)

> A simple illustration of the difference between a Type I and a Type II error is as follows.

- Suppose the null hypothesis is that all systems are operating satisfactorily with regard to a NASA launch. A Type I error would be to delay the launch mistakenly thinking that something was malfunctioning when everything was actually OK. A Type II error would be to fail to delay the launch mistakenly thinking everything was OK when something was actually malfunctioning. The power is the probability of recognizing a particular malfunction. (Note the complementary aspect of power, a “good” thing, with Type II error, a “bad” thing.)
    

It should be emphasized that with regard to calculations, questions like **“What is the** **_power_** **of this test?”** and **“What is the probability of a** **_Type II error_** **in this test?”** cannot be answered without reference to a specific alternative hypothesis.

## Significance Test for a Proportion

It is important to understand that because the _P_-value is a conditional probability, calculated based on the assumption that the null hypothesis, _H_0: _p_ = _p_0, is true, we use the claimed proportion _p_0 both in checking the _np_0 ≥ 10 and _n_(1 − _p_0) ≥ 10 conditions and in calculating the standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/9846e223af5f41bfbd54acbc4f661d30.jpeg)

#### ➥ **Example 6.3**

1. A union spokesperson claims that 75% of union members will support a strike if their basic demands are not met. A company negotiator believes the true percentage is lower and runs a hypothesis test. What is the conclusion if 87 out of a simple random sample of 125 union members say they will strike?
    
2. For each of the two possible answers above, what error might have been committed, Type I or Type II, and what would be a possible consequence?
    

**Solution:**

1. _Parameter:_ Let _p_ represent the proportion of all union members who will support a strike if their basic demands are not met.
    

_Hypotheses:_ _H_0: _p_ = 0.75 and _H_a: _p_ < 0.75.

_Procedure:_ One-sample _z_-test for a population proportion.

_Checks:_ _np_0 = (125)(0.75) = 93.75 and _n_(1 − _p_0) = (125)(0.25) = 31.25 are both ≥ 10, it is given that we have an SRS, and we must assume that 125 is less than 10% of the total union membership.

_Mechanics:_ Calculator software (such as 1-PropZTest on the TI-84 or Z-1-PROP on the Casio Prizm) gives _z_ = −1.394 and _P_ = 0.0816.

_Conclusion in context with linkage to the P-value:_ There are two possible answers:

a. With this large of a _P_-value, 0.0816 > 0.05, there is not sufficient evidence to reject _H_0; that is, there is not sufficient evidence at the 5% significance level that the true percentage of union members who support a strike is less than 75%.

b. With this small of a _P_-value, 0.0816 < 0.10, there is sufficient evidence to reject _H_0; that is, there is sufficient evidence at the 10% significance level that the true percentage of union members who support a strike is less than 75%.

![](https://knowt-user-attachments.s3.amazonaws.com/331d8a9636a444d3a6632321231a51c7.jpeg)

2. If the _P_-value is considered large, 0.0816 > 0.05, so that there is not sufficient evidence to reject the null hypothesis, there is the possibility that a false null hypothesis would mistakenly not be rejected and thus a Type II error would be committed. In this case, the union might call a strike thinking they have greater support than they actually do. If the _P_-value is considered small, 0.0816 < 0.10, so that there is sufficient evidence to reject the null hypothesis, there is the possibility that a true null hypothesis would mistakenly be rejected, and thus a Type I error would be committed. In this case, the union might not call for a strike thinking they don’t have sufficient support when they actually do have support.
    

## Confidence Interval for the Difference of Two Proportions

From Unit 5, we have the following information about the sampling distribution of

![](https://knowt-user-attachments.s3.amazonaws.com/8f0ff5cf03734620b8746ed8f7d74354.jpeg)

1. The set of all differences of sample proportions is approximately normally distributed.
    
2. The mean of the set of differences of sample proportions equals _p_1 − _p_2, the difference of the population proportions.
    
3. The standard deviation
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/5b39631ccc0541c38ae9e6349eafc8ac.jpeg)
    
    of the set of differences of sample proportions is approximately equal to:
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/dd9be6698b7e40879dfaa9b3bb739221.jpeg)
    

Remember that we are using the normal approximation to the binomial, so

![](https://knowt-user-attachments.s3.amazonaws.com/2aa100813f4b424c80138dbaee8ba662.jpeg)

should all be at least 10. In making calculations and drawing conclusions from specific samples, it is important both that the samples be _simple random samples_ and that they be taken _independently_of each other. Finally, the original populations should be large compared to the sample sizes, that is, check that  

![](https://knowt-user-attachments.s3.amazonaws.com/a71bc6a78b7a402a9e4a12d4d2d7b2b7.jpeg)

#### ➥ **Example 6.4**

1. Suppose that 84% of a simple random sample of 125 nurses working 7:00 a.m. to 3:00 p.m. shifts in city hospitals express positive job satisfaction, while only 72% of an SRS of 150 nurses on 11:00 p.m. to 7:00 a.m. shifts express similar fulfillment. Establish a 90% confidence interval estimate for the difference.
    
2. Based on the interval, is there convincing evidence that the nurses on the 7 AM to 3 PM shift express a higher job satisfaction than nurses on the 11 PM to 7 AM shift?
    

**Solution:**

1. _Parameters:_ Let _p_1 represent the proportion of the population of nurses working 7:00 a.m. to 3:00 p.m. shifts in city hospitals who have positive job satisfaction. Let _p_2 represent the proportion of the population of nurses working 11:00 p.m. to 7:00 a.m. shifts in city hospitals who have positive job satisfaction.
    

_Procedure:_ Two-sample _z_-interval for a difference between population proportions, _p_1 − _p_2.

_Checks_:

![](https://knowt-user-attachments.s3.amazonaws.com/e6afd677a3644a9e9096ccfe1f8cc1d8.jpeg)

![](https://knowt-user-attachments.s3.amazonaws.com/cb920e92e47343698135a9fd0959455f.jpeg)

we are given independent SRSs; and the sample sizes are assumed to be less than 10% of the populations of city hospital nurses on the two shifts, respectively.

_Mechanics:_ 2-PropZInt on the TI-84 or 2-Prop ZInterval on the Casio Prizm give (0.0391, 0.2009).

The observed difference is 0.84 − 0.72 = 0.12, and the critical _z_-scores are ±1.645. The confidence interval estimate is 0.12 ± 1.645(0.0492) = 0.12 ± 0.081.]

_Conclusion in context:_ We are 90% confident that the true proportion of satisfied nurses on 7:00 a.m. to 3:00 p.m. shifts is between 0.039 and 0.201 higher than the true proportion for nurses on 11:00 p.m. to 7:00 a.m. shifts.

2. Yes, because the entire interval from 0.039 to 0.201 is positive, there is convincing evidence that the nurses on the 7 AM to 3 PM shift express a higher job satisfaction than nurses on the 11 PM to 7 AM shift.
    

## Significance Test for the Difference of Two Proportions

The null hypothesis for a difference between two proportions is

![](https://knowt-user-attachments.s3.amazonaws.com/a0e02267e2864b68b895f202aa0ece35.jpeg)

and so the normality condition becomes that

![](https://knowt-user-attachments.s3.amazonaws.com/8ba21a7294024f938449e31938fd08ac.jpeg)

  

![](https://knowt-user-attachments.s3.amazonaws.com/fd77a257722142c7ac2e2290e6a6e7af.jpeg)

 should all be at least 10, where p̂ is the combined (or pooled) proportion,

![](https://knowt-user-attachments.s3.amazonaws.com/860c0ac90bf848b39fc732d893dde209.jpeg)

The other important conditions to be checked are both that the samples be random samples, ideally _simple random samples_, and that they be taken _independently_ of each other. The original populations should also be large compared to the sample sizes, that is, check that

![](https://knowt-user-attachments.s3.amazonaws.com/4305d774a9a545c994c4a3c9e9555379.jpeg)

Two points need to be stressed:

- First, sample proportions from the same population can vary from each other.
    
- Second, what we are really comparing are confidence interval estimates, not just single points.
    

For many problems, the null hypothesis states that the population proportions are equal or, equivalently, that their difference is 0:

![](https://knowt-user-attachments.s3.amazonaws.com/ca5614772df54296a0bc9ff47ac90da1.jpeg)

The alternative hypothesis is then:

![](https://knowt-user-attachments.s3.amazonaws.com/b1fcfb9dc096404a8ce3bd47ea8ffe45.jpeg)

where the first two possibilities lead to one-sided tests and the third possibility leads to a two-sided test.

Since the null hypothesis is that _p_1 = _p_2, we call this common value _pc_ and use this pooled value in calculating σ_d_:

![](https://knowt-user-attachments.s3.amazonaws.com/802f83a85cce40a38a74cf0427b66ccc.jpeg)

In practice, if

![](https://knowt-user-attachments.s3.amazonaws.com/041b0726bb6f4fe8b34ad2d52cb841f2.jpeg)

we use

![](https://knowt-user-attachments.s3.amazonaws.com/5fcb5e728c5a432cb7423d5d7002b6c2.jpeg)

as an estimate of _pc_ in calculating _σd_.

#### ➥ **Example 6.5**

1. In a random sample of 1500 First Nations children in Canada, 162 were in child welfare care, while in an independent random sample of 1600 non-Aboriginal children, 23 were in child welfare care. Many people believe that the large proportion of indigenous children in government care is a humanitarian crisis. Do the above data give significant evidence that a greater proportion of First Nations children in Canada are in child welfare care than the proportion of non-Aboriginal children in child welfare care?
    
2. Does a 95% _confidence interval_ for the difference in proportions give a result consistent with the above conclusion?
    

**Solution:**

1. _Parameters:_ Let  _p_1 represent the proportion of the population of First Nations children in Canada who are in child welfare care. Let _p2_ represent the proportion of the population of non-Aboriginal children in Canada who are in child welfare care.
    

_Hypotheses:_ _H_0: _p_1 − _p_2 = 0 or _H_0: _p_1 = _p_2 and _H_a: _p_1 – _p_2 > 0 or _H_a: _p_1 > _p_2.

_Procedure:_ Two-sample _z_-test for a difference of two population proportions.

_Checks:_

![](https://knowt-user-attachments.s3.amazonaws.com/9656c1f56aca42dcbb9028083550e71d.jpeg)

![](https://knowt-user-attachments.s3.amazonaws.com/0a806ee3025141e3b6e8aefa33826a87.jpeg)

are all at least 10; the samples are random and independent by design; and it is reasonable to assume the sample sizes are less than 10% of the populations.

_Mechanics:_ Calculator software (such as 2-PropZTest) gives _z_ = 11.0 and _P_ = 0.000.

_Conclusion in context with linkage to the P-value:_ With this small of a _P_-value, 0.000 < 0.05, there is sufficient evidence to reject _H_0; that is, there is convincing evidence that that the true proportion of all First Nations children in Canada in child welfare care is greater than the true proportion of all non-Aboriginal children in Canada in child welfare care.

2. Calculator software (such as 2-PropZInt) gives that we are 95% confident that the true difference in proportions (true proportion of all First Nations children in Canada in child welfare care minus the true proportion of all non-Aboriginal children in Canada in child welfare care) is between 0.077 and 0.110. Since this interval is entirely positive, it is consistent with the conclusion from the hypothesis test.