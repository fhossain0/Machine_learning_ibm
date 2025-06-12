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



