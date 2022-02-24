# 66 Days of Data

## [Statistics Fundamentals](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw) 

### DAY 1: Histograms, The Main Ideas behind Probability Distributions, The Normal Distribution
 ![image](https://user-images.githubusercontent.com/25703485/154499858-39d05791-718a-492f-a21b-517138a105a5.png)
_Image from [The Normal Distribution, Clearly Explained!!!](https://www.youtube.com/watch?v=rzFX5NWojp0&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9&index=3)_
- To draw a normal distribution, we need to know:
  1. The avg measurement - tells where the centre of the curve goes
  2. SD of the measurements - tells how wide the curve should be 

### DAY 2: Population and Estimated Parameters

- Normal Distribution Exponential Distribution, Gamma Distribution
![Image](https://gregorygundersen.com/image/moments/total_mass.png)

 _Image from https://gregorygundersen.com/blog/2020/04/11/moments/_

- It's very rare to have population data. In statistics, we often estimate the population parameters using samples/some data points. 
- The more data we have, the more confidence we can have in accuracy of the estimates. 
- **p-values** and **confidence intervals** are often used to quantity the confidence in the estimated parameters 

### DAY 3: Mean, Variance and SD, Statistical Model 

 - Formula to calculate, not estimate, the population variance. Firt (Estimated mean x̄ - Population mean μ) for each measurement, square then add all the terms. Lastly we get the average of the square difference (by dividing nb of measurements, n) 
 - The population variance gives values in square. 
 - Population standard deviation = √population variance
 - We almost never have data to calculate the population variance/SD and always work with smaller samples to perform estimation
 - Estimated population variance: Since we don't know population mean (μ), we use sample mean (x̄). And dividing by n - 1 compensates the fact the we are calcualting difference from the sample mean instead of population mean, otherwise we will consistently underestimate the variance around the population mean, as the difference between data and sample mean are normally smaller than the difference between data and population mean. 
  ![Image](https://miro.medium.com/max/1186/0*Wsf4o0CCGLFGY27L.png)
  _Image from https://medium.com/statistical-guess/sample-variance-cbd0a848acfe_

- What is a model? A model is a way to explore the relationship.

### DAY 4: SAMPLING FROM A DISTRIBUTION, HYPOTHESIS TESTING AND THE NULL HYPOTHESIS 
- If there is no preliminary data, there are a lot of possibilities if we were to set hypotheses (e.g. 12h/13h/14h for time to recovers after taking drugs).
- Null hypothesis is useful when we do not have preliminary data.    
- The hypotehesis that there is no difference between things is called the **Null Hypothesis**

### DAY 5: ALTERNATIVE HYPOTHESES: MAIN IDEAS
- When we have only 2 groups of data, the **Alternative Hypothesis** is the oppositie of **Null Hypothesis**.
-![image](https://user-images.githubusercontent.com/25703485/154922065-1a61ad0c-7c33-4111-a195-c2d748517414.png)
_Image from [Alternative Hypotheses: Main Ideas!!!](https://www.youtube.com/watch?v=5koKb5B_YWo&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9&index=9)_
- When we have more than 2 groups of data, we have options for Alternative Hypothesis, we have options on how to set alternative hypothesis and decide which statistical test to use. 
_![image](https://user-images.githubusercontent.com/25703485/154922356-5d818dc6-f04a-4f12-a501-e51a4976cd40.png)_

### DAY 6: P-VALUES: WHAT THEY ARE AND HOW TO INTEPRET THEM, HOW TO CALCULATE P-VALUES 
- A p-value is a measure of probability that an observed difference could have occurted just by random chance. 
- The lower the p-value. the greater the statistical significance of the observed difference.
- Using a p-value treshold of 0.00001 means we would only get a False Positive once in every 100,000 experiments. 
- There are 2 types of p-values: one-sided & two-sided
- p-value is determined by adding up the probabilities. A p-value is composed of 3 parts:
i. The probability random chance would result in the observation
ii. The probability of observing something else that is equally rare
iii. The probability of observing something rarer or more extreme

### DAY 7: P-HACKING: WHAT IT IS AND HOW TO AVOID IT
- p-hacking refers to the misuse analysis techniques and results in being fooled by false positives.
- TO avoid p-hacking, calculate the p-value for each test and adjust all of the p-values with things like False Discovery Rate to reduce the probability of reporting a False Positive
- If you have p-values that is close to 0.05, don't just add more data to the observation, instead, use data you have for a Power Analysis to determine the correct sample size.

### DAY 8: STATISTICAL POWER & POWER ANALYSIS 
- Power is the probability that we will correctly reject the Null Hypothesis. 
- **Power Analysis** is a way to determine sample size for the next time we do this experiment.
- Power is affected 2 factors, i.e. (i) how much overlap there is between 2 distributions we want to identify, and (ii) the sample size, the number of measurements we collect from each group 
- The larger the overlap between 2 distributions, the larger the sample size needs to be in order to have higher power value.

### 2022-02-24 DAY 9: COVARIANCE & CORRELATION
- When the covariance is positive, it tells us the relationship of the 2 sets of observations is positive.
- Covariance is sensitive to the scale of the data, making it difficult to interpret
- Covariance is 
- The covariance formula is similar to the formula for correlation and deals with the calculation of data points from the **average/mean value** in a dataset. For example, the covariance between two random variables X and Y can be calculated using the following formula (for population):

![Image](https://miro.medium.com/max/1186/0*Wsf4o0CCGLFGY27L.png)

_Image from https://corporatefinanceinstitute.com/resources/knowledge/finance/covariance/_

- For a sample covariance, the formula is slightly adjusted:

![Image](https://cdn.corporatefinanceinstitute.com/assets/covariance2.png)

- Covariance is a stepping stone of many analyses.
- **Correlation** quantifies the strength of relationships. 
- Range from -1 to 1. -1 means the strongest linear relationship with a negative slope, and 1 is the strongest linear relationship with a positive slope. In both cases, if a straight line can not go through all of the data, then we will get correlation values closer to 0.
- Weak relationship = low correlation value, vice versa.
- Our confidence in the inference depends on how much data we have.
- p-value can be used to assess the confidence. The more the data we have, the smaller the p-value and the more confidence we have our inferences.

![image](https://user-images.githubusercontent.com/25703485/155543064-fa7ed00c-41c8-433a-9898-8760d57ec57f.png)

- 


