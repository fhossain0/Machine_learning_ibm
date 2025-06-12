Estimation Vs inference
# Definition:
- Estimation is the process of calculating an approximate value of a population parameter (like mean, proportion, or standard deviation) based on sample data.
- Inference is the broader process of using sample data to draw conclusions or make decisions about a population, which includes estimation, hypothesis testing, and prediction. **statistical inference, we don’t just make an estimate, we also describe how accurate or reliable that estimate is. That’s where things like standard error and confidence intervals come in.**









# CI inside otf the barplots 
CI= confidence interval: Imagine you ask 10 people how much they like a product, and you get an average score (mean). But if you asked another 10 people, the average might be different.

The confidence interval shows a range around the average that says:

### when we plot bars for each category seaborn by default adds small lines (Error bards) on top of the bars 

parametric vs Non-parametric

If inferences is about trying to find out the data generating process (DGP)
then we can say that a statistical model of the data is a set of possible distributions or maybe even regressions

### parametric model is a particular type of statistical model : it is also a set of distribution or regressipon but they have a finite numbe rof parameters 

# None-parametric model 
- we make fewer assumptions
- in particular , we do not assume that the data belong to any particular distribution also called distribution free inference

An example of non-parametric is creating a distribution of the data (CDF or cumulative distribution function ) using a histogram

in this case , we are not specifying parameters 

# parametric models 
A parametric model is aparticular type of statistical model : it is a also a set of distribution or regression, but they have a finite number of parameters

An example of parametric model: the normal distribution 
![Screenshot 2025-06-12 at 13 09 14](https://github.com/user-attachments/assets/c53ef797-fbaa-4fd0-b3ec-2a49598931c8)

Example : customer lifetime value

Customer lifetime value is an extimate of the customer's value to the company 
Data releted to customer lifetime value migth include :
- The expected length of time aas a customer 
- the expected amount spent over time
- To estimate lifetime value, we make assumtions about the data
- these assumtions can be parametric (assuming a specific distribution) or non-parametric

The most common way of estimating parameters in a parametric model is through likelihood estimation(MLE)
- The likelihood function is related to probability and is a function of the aprameters of the model:
![Screenshot 2025-06-12 at 13 15 13](https://github.com/user-attachments/assets/168c0a33-4618-493d-8157-a394f8ff1f23)

Then we choose based estimation which gonna most likely to graw our conclustion 



# Most import part common distribution 

Commonly used distributions
![Screenshot 2025-06-12 at 13 17 35](https://github.com/user-attachments/assets/5d0d831d-88e1-484b-955c-513ceb8dcd10)
**Understandable: uniform distribution: because it is uniformly equal chances that you will get any value in out range, every single value is equally likely** 

![Screenshot 2025-06-12 at 13 26 08](https://github.com/user-attachments/assets/be606a57-f499-4fb5-92ea-438a1512f0dc)
**Gaussin / normal: Most likely value is going to be those values that are closest to the mean and those that are further out or either side are goinmg to be equally unlikely the further away we move from the mean**

- The central limit theoram makes normal distribution more popular. the idea is you take the average value from a bunch of samples, the average value of each one of those random samples. the distribution of those average is going to be a normal curve if you have enough values.

# log normal distribution
- the idea being that- if you took the loog of this variable, then you have the normal distribution
  ![Screenshot 2025-06-12 at 13 34 58](https://github.com/user-attachments/assets/c56fa367-e844-4ae1-a88f-34de259aefd8)

#  exponential curve 

What is going to be the amount of before the next event. 

![Screenshot 2025-06-12 at 13 38 22](https://github.com/user-attachments/assets/705076a8-d5ea-40e4-adea-f8389f114e45)

the time between you or some one else ends up watching this vedio. so the time will be, and then as soon as someone else watches, then you restart and mostly people are around one minute, whereas at some point there is  this long spread out, then you restart and mostly people are around one minute, where as at somepoint there is long spread out. some type of break that's likely to happen where it take 10 15 mints before the next person watches this vedio 

# poisson distribution

![Screenshot 2025-06-12 at 13 43 42](https://github.com/user-attachments/assets/99b54803-a016-495e-ad4f-25913bc80580)

think like number of events happend during the certain amount of time.
- We have the lambda, which is both the avrage value, and the variance value of the distribution. We can think here an exple is like how many people are ging to watch this vedio in next 10 minutes.
- if the lambda was one then we said most of the time is only one person that watches every 10 minutes. and it's tight around that one, but if something like 10 people watch it evry 10 minutes. then you will probably have. more of the spread of your standerd diviation becuase it cloud be closer to 5 or 15 when you have a larger value.
- and that's going to be your poisson distribution


# Frequesntist vs Bayesian Statistics 
A Frequentist is concerned with repeadted observation in the limit : We satrt with any idea for probabilities , we are trying to estimate so just to tie into a business example for both frequentist and bayesian how it works in regards to queuing theory 

**Queuing theory :** The study of working with queues or lines and how many servers we need to match the size of that queue or the size of that line.
So you can think about a grocery store how many cashiers we need to check out our customers in timely fashion this can be the web servers we will need in order to respond to all of the web pages requests and within an appropriate responsee sign or respond to all of the web page request . 


**Frequesntist vs Bayesian Statistics both to estimate the probabilities of certain number of customers coming over a fixed time period**

Processes may have true frequencies, but we are interested in modeling probabilities as many, many repeats of an experiment. 

So we assume no prior knowledge of the true frequencies, insted we rely on the fact that if our sample is learge enough, if we seen enough cues or line. we can have a strong estimates and probabilities of a certain number of people that will that will come in given a fixed time period and the parameters of our poisson distribution then we can refer estimates of our probability, given that sample, many repeats of experiment togather as much of as possible in our frequentist approach 


# Frequentist
1. Drive the probabilistic property of a procedure
2. Apply the probability directkly to the observed data

# Bayesian 
Now for Bayesian statistics, the parameters themselves can have a probability distribution. So rather than having a direct guess for the probability distribution and our uncertainty being around what their sample covered that population parameter, we provide probability distributions to the parameters themselves. In other words, the more data we have, the tighter that probability distribution will be around the parameter estimate that we have. Now, Bayesian also allows for experimenters to incorporate their prior beliefs of the distribution. For frequentists, it's going to be solely based on the data available. For the probability of seeing X amount of people in line during a certain time period, we can have actually an educated guess perhaps to start off with and Bayesian allows us to incorporate this into our prior distribution. 

- The prior distribution is then updated after seeing the data. So we had our initial guess and after seeing more and more data, we can change what the distribution of our parameter estimate is. Then after updating the distribution, we then have our posterior distribution, which has now incorporated the data to update our guess of what that estimate will be.

Now we use much of the same math and the same formulas for both frequentist and Bayesian statistics. The main element that's going to refer is essentially the interpretation as we discussed in terms of are we estimating how likely we are to cover the actual population mean? Or we coming up with a distribution for that population mean. We'll point out more along the way the difference in interpretation as appropriate. 


So in this section, we discussed about the difference between inference and estimation and how at times machine learning may only focus on the estimation, whereas statistical inference will look to the underlying data generating process. We discussed parametric and non-parametric approaches of modeling, where parametric modeling will rely on assumptions of distributions and number of parameters, where non-parametric models will not have as strong of an assumption. We went through common statistical distributions and examples of where they would be used in the real world. Then finally, we introduced the idea behind frequentist and Bayesian statistics. This next section we'll begin to discuss hypothesis testing in both frequentist and Bayesian framework.


