# Hypothesis testing 
- So a hypothesis is a statement about a population parameter such as the mean of our poison distribution, and our estimate of the number of people that will come into the line for our grocery store example in the next hour.

**We create two hypotheses. We start off with a null hypothesis and an alternative hypothesis**
- we decide which one to call the null depending on how the problem is set up. So an example would be that, we get an average of five people coming in per hour, and the alternative maybe being greater than five. So any number greater than five would be the alternative, with just five being the null, or it could be a specific amounts of people such as five being the null and eight being the alternative. Now if one of those values is less specific, for example, such as greater than five or not equal to five, that will usually be the alternative, whereas the null will be the specific value.
- So given the data from the sample we use, we then use a hypothesis testing procedure to decide whether we're going to accept the null hypothesis or reject the null and accept the alternative.

# Fact
Now it's often said that you can reject the null but never accept the alternative. Here we're just saying for practical purposes, when moving forward with your projects, you'll be taking the path that the alternative is true depending on your test statistic. Now, in the Bayesian interpretation, we won't get a decision boundary, rather we'll get posterior probabilities of the null and the alternative hypothesis, and see which one is more likely

![Screenshot 2025-06-12 at 14 23 58](https://github.com/user-attachments/assets/16cc6756-febb-4d4d-bd42-392a42c40dd5)

- So, let's look at an example to make this clear. We're going to look at a coin tossing example. Imagine you have two coins. Coin 1 has 70 percent probability of coming up heads, and coin 2 has 50/50 chance of coming up heads.

- So we want to pick one without looking between these two.
- Toss that coin 10 times and see how many times heads comes up. Then given the number of heads that come up, you will say which one is more likely between the two coins? Which one will be more likely to be picked? Is it the 50/50 coin or the one that has 70 percent probability of coming up heads?
- So, given what we know about coins 1 and 2 and their probabilities, we can make a table of the probability of seeing a certain amount of heads out of our 10 tosses. So here we see coin 1 with a probability of heads being 0.5 and coin 2 with probability of heads being 0.7. We can see through the chart that as we get closer to, so lower numbers are going to be much more likely to be the 50/50 coin. As we get to higher values in terms of the number of heads that show up, it'll be much more likely that we have the 0.7 biased coin in terms of a higher probability of coming up as heads.

- Now we can calculate the likelihood ratio based on the number of heads we see when we toss this unidentified coin. We see the probability of coming up with three heads out of our 10 tosses, given our coin is either has a 50/50 chance of landing heads or 70/30 chance of landing heads.
- The probability of three heads given coin 1 is 0.117 versus the probability for three hexads given that we have coin 2 is much less likely as 0.009. Thus we have that coin 1 was 13 times more likely to give us the output of three heads than coin 2.
# likely hood ratio 
We call this ratio, the likelihood ratio, the ratio of which one of our null versus alternative hypothesis is more likely.

# Bayesian Hypothesis Testing with Coin Toss Example

## Prior Probabilities

As discussed in the **Bayesian interpretation**, we need **priors** for each hypothesis.

In this case, we randomly chose the coin that we're going to flip—whether it was **0.5 (fair coin)** or **0.7 (biased coin)**. So, we assume our **prior estimate** for each of these values—the chance of choosing either 0.5 or 0.7—is:

P(H₁) = 0.5
P(H₂) = 0.5


Since we have no way of knowing which coin was actually chosen **before seeing the data**, we assume a **50/50 chance** for each hypothesis.

---

## Real-World Consideration

If we were pulling a coin from the **general public**, our **prior distribution**—based on real-world knowledge—might heavily favor the idea of a fair coin. This would make it much **harder to accept** the hypothesis that the coin is unfair (i.e., biased).

---

## Using Bayes' Rule

In this example, we are assuming knowledge of **Bayes' Rule**. We'll use our priors, \( P(H_1) \) and \( P(H_2) \), both equal to **0.5**, to compute the **posterior distribution**.

### Posterior:
\[
P(H_1 \mid X) = \frac{P(X \mid H_1) \cdot P(H_1)}{P(X)}
\]

Where:
- \( X \): the observed data (e.g., getting 3 heads)
- \( H_1 \): hypothesis that the coin is fair (p = 0.5)
- \( P(X \mid H_1) \): likelihood of data under \( H_1 \)
- \( P(H_1) \): prior probability
- \( P(X) \): probability of the data over **all** hypotheses

**Note**: The denominator \( P(X) \) is the same for all hypotheses and **does not affect** the likelihood ratio.

---

## Likelihood Ratio

We focus on the ratio:

\[
\frac{P(X \mid H_1)}{P(X \mid H_2)}
\]

This tells us how much more likely the data is under \( H_1 \) than \( H_2 \).

But now we **include priors**:
\[
\frac{P(X \mid H_1) \cdot P(H_1)}{P(X \mid H_2) \cdot P(H_2)}
\]

If \( P(H_1) = 0.99 \) and \( P(H_2) = 0.01 \), you’d need a very large numerator (likelihood) to make \( H_2 \) more believable. This shows how **strong priors** can influence outcomes.

---

## Priors and Likelihood

Our priors are **multiplied** by the likelihoods to get posteriors:

\[
\text{Posterior} \propto \text{Likelihood} \times \text{Prior}
\]

The **likelihood ratio** is only based on the data and does **not depend on the priors**.

This ratio updates our priors to give the **posterior distribution**, which reflects our belief after seeing the data.

---

## Summary

- We reviewed **hypothesis testing** using Bayesian logic.
- We showed how **prior distributions** and the **likelihood ratio** shape the outcome.
- A **coin toss** example was used to demonstrate Bayesian reasoning.
- We will continue by discussing how this compares to **frequentist** approaches.

---


