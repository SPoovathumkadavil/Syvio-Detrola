---
alias: "Variance"
subject: "Math"
subset: "Biology"
importance: 8
type: "Concept"
---

Variance is a measure of dispersion, meaning it is a measure of how far a set of numbers is spread out from their average value. It is the second central moment of a distribution, and the covariance of the random variable with itself, and it is often represented by $\large\sigma^2$, $\large s^2$ or $\large V(x)$.

## Calculation
$$\large \frac{\sum (x_i - \bar{x})^2}{n-1}$$
Note that this is [[Standard Deviation]] squared.
Variance is the average squared difference of all values to the mean.

## Why n-1?

Why divide by **n-1** rather than **n** in the third step above? In step 1, you compute the difference between each value and the mean of those values. **You don't know the true mean of the population;** **all you know is the mean of your sample**. Except for the rare cases where the sample mean happens to equal the population mean, the data will be closer to the sample mean than it will be to the true population mean. So the value you compute in step 2 will probably be a bit smaller (and can't be larger) than what it would be if you used the true population mean in step 1. To make up for this, divide by n-1 rather than n.v **This is called Bessel's correction.**

But why n-1? If you knew the sample mean, and all but one of the values, you could calculate what that last value must be. Statisticians say there are **n-1 degrees of freedom.**

The **n-1** equation is used in the common situation where you are **analyzing a sample of data and wish to make more general conclusions.** The SD computed this way (with n-1 in the denominator) is your best guess for the value of the SD in the overall population.

If you simply want to quantify the variation in a particular set of data, and don't plan to extrapolate to make wider conclusions, then you can compute the SD using n in the denominator. **The resulting SD is the SD of those particular values.** It makes no sense to compute the SD this way if you want to estimate the SD of the population from which those points were drawn. It only makes sense to use n in the denominator when there is no sampling from a population, there is no desire to make general conclusions. 