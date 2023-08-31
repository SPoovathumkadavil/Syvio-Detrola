---
alias: "Probability, Random Variables, and Probability Distributions"
subject: "Math"
subset: "Statistics"
importance: 7
type: "AP Guide"
order: 4
---

## The Law of Large Numbers

- **_Law of large numbers -_** states that when an experiment is performed a large number of times, the relative frequency of an event tends to become closer to the true probability of the event; that is, _probability is long-run relative frequency__._ There is a sense of predictability about the long run.
    

**The law of large numbers has two conditions:**

- First, the chance event under consideration does not change from trial to trial.
    
- Second, any conclusion must be based on a large (a very large!) number of observations.
    

#### ➥ **Example 4.1**

There are two games involving flipping a fair coin. In the first game, you win a prize if you can throw between 45% and 55% heads. In the second game, you win if you can throw more than 60% heads. For each game, would you rather flip 20 times or 200 times?

**Solution:** The probability of throwing heads is 0.5. By the law of large numbers, the more times you throw the coin, the more the relative frequency tends to become closer to this probability. With fewer tosses, there is greater chance of wide swings in the relative frequency. Thus, in the first game, you would rather have 200 flips, whereas in the second game, you would rather have only 20 flips.

## Basic Probability Rules

#### ➥ **Example 4.2**

A standard literacy test consists of 100 multiple-choice questions, each with five possible answers. There is no penalty for guessing. A score of 60 is considered passing, and a score of 80 is considered superior. When an answer is completely unknown, test takers employ one of three strategies: guess, choose answer (c), or choose the longest answer. The table below summarizes the results of 1000 test takers.

![](https://knowt-user-attachments.s3.amazonaws.com/ab6324d0c3c243a3a311f17099de223b.jpeg)

1. What is the probability that someone in this group uses the “guess” strategy?
    
2. What is the probability that someone in this group scores 60–79?
    
3. What is the probability that someone in this group does not score 60–79?
    
4. What is the probability that someone in this group chooses strategy “answer (c)” _and_ scores 80–100 (sometimes called the _joint probability_ of the two events)?
    
5. What is the probability that someone in this group chooses strategy “longest answer” _or_ scores 0–59?
    
6. What is the probability that someone in this group chooses the strategy “guess” _given that_ his or her score was 0–59?
    
7. What is the probability that someone in this group scored 80–100 _given that_ the person chose strategy “longest answer”?
    
8. Are the strategy “guess” and scoring 0–59 _independent events_? That is, is whether a test taker used the strategy “guess” unaffected by whether the test taker scored 0–59?
    
9. Are the strategy “longest answer” and scoring 80–100 _mutually exclusive events_? That is, are these two events disjoint and cannot simultaneously occur?
    

**Solution:**

![](https://knowt-user-attachments.s3.amazonaws.com/b37c043a2a9248d48ccb69c7c9181bbd.jpeg)

2. ![](https://knowt-user-attachments.s3.amazonaws.com/404a9306b4eb4b74ad938df0fcca1a19.jpeg)
    
3. _P_(_does not score_ 60–79) = 1 − _P_(_score_ 60–79) = 1 − 0.53 = 0.47
    
4. ![](https://knowt-user-attachments.s3.amazonaws.com/c2824ab7555b4545bcc7a30ba0e53d64.jpeg)
    
5. ![](https://knowt-user-attachments.s3.amazonaws.com/4b2c421ffbfd4416ba03b7c42aca23a7.jpeg)
    
6. ![](https://knowt-user-attachments.s3.amazonaws.com/150b48ceb0e3491d98b5f3edc696f212.jpeg)
    
7. ![](https://knowt-user-attachments.s3.amazonaws.com/21929a9dbf39434aa0db76ee00b7c231.jpeg)
    
8. We must check if _P_ (_guess_|score 0–59) = _P_(_guess_). From (f) and (a), we see that these probabilities are not equal (0.333 ≠ 0.3), so the strategy “guess” and scoring 0–59 are _not_ independent events.
    
9. _longest answer_ ∩ _score_ 80–100 ≠ Ø and _P_(_longest answer_ ∩ _score_ 80–100)  = 135/1000 ≠ 0, so the strategy “longest answer” and scoring 80–100 are _not_ mutually exclusive events.
    

## Multistage Probability Calculations

#### ➥ **Example 4.3**

On a university campus, 60%, 30%, and 10% of the computers use Windows, Apple, and Linux operating systems, respectively. A new virus affects 3% of the Windows, 2% of the Apple, and 1% of the Linux operating systems. What is the probability a computer on this campus has the virus?

**Solution:** In such problems, it is helpful to start with a tree diagram.

![](https://knowt-user-attachments.s3.amazonaws.com/4f830667c5b54aadac40bc74531386a8.jpeg)

We then have:

![](https://knowt-user-attachments.s3.amazonaws.com/97c01a4b82ae4e80b03dca79f2f7b91c.jpeg)

## Random Variables, Means (Expected Values), and Standard Deviations

- Often each outcome of an experiment has not only an associated probability but also an associated **_real number_**.
    
- If _X_ represents the different numbers associated with the potential outcomes of some chance situation, we call **_X_** a **random variable**.
    

#### ➥ **Example 4.4**

A charity holds a lottery in which 10,000 tickets are sold at $1 each and with a prize of $7500 for one winner. What is the average result for each ticket holder?

**Solution:** The actual winning payoff is $7499 because the winner paid $1 for a ticket. Letting X be the payoff random variable, we have:

|Outcome|Random Variable _X_|Probability _P_(_x_)|
|---|---|---|
|Win|7499|1/10,000|
|Lose|–1|9,999/10,000|

![](https://knowt-user-attachments.s3.amazonaws.com/b60a400eac174d2088bd0736bc25637d.jpeg)

> Thus, the _average_ result for each ticket holder is a $0.25 loss. [Alternatively, we can say that the expected payoff to the charity is $0.25 for each ticket sold.]

---

The mean of this new discrete random variable is ∑(_xi_ − _µx_)2_pi_, which is precisely how we define the variance, _σ_2, of a discrete random variable:

![](https://knowt-user-attachments.s3.amazonaws.com/bb96daf19dde465a95afe74d5b551d50.jpeg)

#### ➥ **Example 4.5**

A highway engineer knows that the workers can lay 5 miles of highway on a clear day, 2 miles on a rainy day, and only 1 mile on a snowy day. Suppose the probabilities are as follows:

|Outcome|Random variable _X_ (Miles of highway)|Probability _P_(_x_)|
|---|---|---|
|Clear|5|0.6|
|Rain|2|0.3|
|Snow|1|0.1|

1. What are the mean (expected value), standard deviation, and variance?
    
2. Would it be surprising if the workers laid 10 miles of highway one day?
    

**Solution:**

1. ![](https://knowt-user-attachments.s3.amazonaws.com/90cf3f764c98458295c80065a37e229d.jpeg)
    

In the long run, the workers will lay an average of 3.7 miles of highway per day. The number of miles the workers lay on a randomly selected day will generally vary about 1.62 from the mean of 3.7 miles.

2. 10 is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/b4bbb87b6fe042ce8f33d8f40b482ba3.jpeg)
    
    standard deviations above the mean, so this would be very surprising!
    

## Means and Variances for Sums and Differences of Sets

- When the random variables are independent, there is an easy calculation for finding both the mean and standard deviation of the sum (and difference) of the two random variables.
    

#### ➥ **Example 4.6**

A casino offers couples at the hotel free chips by allowing each person to reach into a bag and pull out a card stating the number of free chips. One person’s bag has a set of four cards with _X_ = {1, 9, 20, 74}; the other person’s bag has a set of three cards with _Y_ = {5, 15, 55}. Note that the mean of set _X_ is

![](https://knowt-user-attachments.s3.amazonaws.com/c3ae4e7e4df946069d1dd6097531c927.jpeg)

1. What is the average amount a couple should be able to pool together?

**Solution:** Form the set _W_ of sums: _W_ = {1 + 5, 1 + 15, 1 + 55, 9 + 5, 9 + 15, 9 + 55, 20 + 5, 20 + 15, 20 + 55, 74 + 5, 74 + 15, 74 + 55} = {6, 16, 56, 14, 24, 64, 25, 35, 75, 79, 89, 129} and

![](https://knowt-user-attachments.s3.amazonaws.com/581024c33b7340408cce336fbfce1984.jpeg)

Finally, _µW_ = _µX_ + _Y_ = _µX_ + _µY_ = 26 + 25 = 51. On average, a couple should be able to pool together 51 free chips.

2. How is the variance of _W_ related to the variances of the original sets?
    

![](https://knowt-user-attachments.s3.amazonaws.com/1cb2c99b5fd14c25967fedd154d88d38.jpeg)

We can also calculate the standard deviation

![](https://knowt-user-attachments.s3.amazonaws.com/7bd114267e1043c1b3f42705ef406d01.jpeg)

and conclude that the average pooled number of chips received by a couple is 51 with a standard deviation of 35.78.

## Means and Variances for Sums and Differences of Random Variables

- The mean of the sum (or difference) of two random variables is equal to the sum (or difference) of the individual means.
    
- _If two random variables are independent_, the variance of the sum (or difference) of the two random variables is equal to the **_sum_** of the two individual variances.
    

#### ➥ **Example 4.7**

An insurance salesperson estimates the numbers of new auto and home insurance policies she sells per day as follows:

![](https://knowt-user-attachments.s3.amazonaws.com/b632a9ea9d344a4184399660ed2bdf49.jpeg)

1. What is the expected value or mean for the overall number of policies sold per day?
    
2. Assuming the selling of new auto policies is independent of the selling of new home policies (which may not be true if some new customers buy both), what would be the standard deviation in the number of new policies sold per day?
    

**Solution:**

1. _µauto_= (0)(0.2) + (1)(0.4) + (2)(0.3) + (3)(0.1) = 1.3,  
    _µhome_= (0)(0.5) + (1)(0.3) + (2)(0.2) = 0.7, and so  
    _µtotal_ = _µauto_ + _µhome_ = 1.3 + 0.7 = 2.0.
    
2. _σ_2_auto_= (0 − 1.3)2(0.2) + (1 − 1.3)2(0.4) + (2 − 1.3)2(0.3) + (3 − 1.3)2(0.1) = 0.81,  
    _σ_2_home_ = (0 − 0.7)2(0.5) + (1 − 0.7)2(0.3) + (2 − 0.7)2(0.2) = 0.61, and so, **assuming independence**, _σ_2_total_ = _σ_2_auto_ + _σ_2_home_ = 0.81 + 0.61 = 1.42 and
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/569e18f80c9845abbfb4135244f90a0f.jpeg)
    

## Transforming Random Variables

- **Adding a constant** **to every value** of a random variable will increase the mean by that constant.
    
- **Differences between values** remain the same, so measures of variability like the standard deviation will remain unchanged.
    
- **Multiplying every value** of a random variable by a constant will increase the mean by the same multiple. In this case, differences are also increased and the standard deviation will increase by the same multiple.
    

#### ➥ **Example 4.8**

A carnival game of chance has payoffs of $2 with probability 0.5, of $5 with probability 0.4, and of $10 with probability 0.1. What should you be willing to pay to play the game? Calculate the mean and standard deviation for the winnings if you play this game.

**Solution:**

![](https://knowt-user-attachments.s3.amazonaws.com/f62ec030ba704820a2aa4845b49d5ebb.jpeg)

You should be willing to pay any amount less than or equal to $4.

![](https://knowt-user-attachments.s3.amazonaws.com/50bb5d5dd8ca4567a10b9ff1a4fe544b.jpeg)

What if $4 is added to each payoff?

![](https://knowt-user-attachments.s3.amazonaws.com/ec30b57d846843b3ab132ae7f42999e1.jpeg)

Note that _µX_+4 = _µX_ + 4 and _σX_+4 = _σX_.

What if instead each payoff is tripled?

![](https://knowt-user-attachments.s3.amazonaws.com/60e32edff9924f33af72ef951ac6ed0b.jpeg)

Note that _µ_3_X_ = 3_µX_ and _σ_3_X_ = 3_σX_

## Binomial Distribution

**Probability distributio**n - is a list or formula that gives the probability of each outcome.

- For applications in which a two-outcome situation is repeated a certain number of times, where each repetition is independent of the other repetitions, and in which the probability of each of the two outcomes remains the same for each repetition, the resulting calculations involve what are known as **_binomial probabilities_**.
    

#### ➥ **Example 4.9**

Suppose the probability that a lightbulb is defective is 0.1 (so probability of being good is 0.9).

1. What is the probability that four lightbulbs are all defective?
    
2. What is the probability that exactly two out of three lightbulbs are defective?
    
3. What is the probability that exactly three out of eight lightbulbs are defective?
    

**Solution:**

1. Because of independence (i.e., whether one lightbulb is defective is not influenced by whether any other lightbulb is defective), we can multiply individual probabilities of being defective to find the probability that all the bulbs are defective:
    
    (0.1)(0.1)(0.1)(0.1) = (0.1)4 = 0.0001
    
2. The probability that the first two bulbs are defective and the third is good is (0.1)(0.1)(0.9) = 0.009. The probability that the first bulb is good and the other two are defective is (0.9)(0.1)(0.1) = 0.009. Finally, the probability that the second bulb is good and the other two are defective is (0.1)(0.9)(0.1) = 0.009. Summing, we find that the probability that exactly two out of three bulbs are defective is 0.009 + 0.009 + 0.009 = 3(0.009) = 0.027.
    
3. The probability of any particular arrangement of three defective and five good bulbs is (0.1)3(0.9)5 = 0.00059049. We need to know the number of such arrangements.
    
    The answer is given by combinations:
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/886babeb6521455c888d9be048c4fd5d.jpeg)
    
    Thus, the probability that exactly three out of eight light bulbs are defective is 56 × 0.00059049 = 0.03306744. [On the TI-84, binompdf(8,0.1,3)= 0.03306744.]
    

## Geometric Distribution

- Suppose an experiment has two possible outcomes, called _success_ and _failure_, with the probability of success equal to _p_ and the probability of failure equal to _q_ = 1 − _p_ and the trials are independent. Then the probability that the first success is on trial number _X_ = _k_ is
    
    ![](https://knowt-user-attachments.s3.amazonaws.com/395cf6f1fa98481abb80c523655507c8.jpeg)
    

#### ➥ **Example 4.10**

Suppose only 12% of men in ancient Greece were honest. What is the probability that the first honest man Diogenes encounters will be the third man he meets? What is the probability that the first honest man he encounters will be no later than the fourth man he meets?

**Solution:**

This is a geometric distribution with p = 0.12. Then P(X=3) = (0.88)2(0.12) = 0.092928, where X is the number of men needed to be met in order to encounter an honest man. [Or we can calculate geometpdf (0.12, 3) = 0.092928.] This is a geometric distribution with p = 0.12. Then = geometcdf (0.12, 4) = 0.40030464. [Or we could calculate (0.12) + (0.88)(0.12) + (0.88)2(0.12) + (0.88)3(0.12) = 0.40030464.]

---

To receive full credit for geometric distribution probability calculations, students need to state:

1. Name of the distribution ("geometric" in the example above)
    
2. Parameter ("p = 0.12" in the example above)
    
3. The trial on which the first success occurs ("X = 3" in the first question above)
    
4. Correct probability (“0.092928” in the first question above)
    

## Cumulative Probability Distribution

- **Probability distribution** - is a function, table, or graph that links outcomes of a statistical experiment with its probability of occurrence.
    
- **_Cumulative_** **probability distribution** - is a function, table, or graph that links outcomes with the probability of less than or equal to that outcome occurring.
    

#### ➥ **Example 4.11**

The scores received on the 2019 AP Statistics exam are illustrated in the following tables:

![](https://knowt-user-attachments.s3.amazonaws.com/cd195be8536142999e7046b8bd96df8e.jpeg)

![](https://knowt-user-attachments.s3.amazonaws.com/aa1bb217a937406bae4e09677b6f3e94.jpeg)

What is the probability that a student did not receive college credit (assuming you need a 3 or higher to receive college credit)?

**Solution:** the probability was 0.211 + 0.197 = 0.408 that a student received a 1 or 2 and thus did not receive college credit.

---