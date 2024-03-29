# 66 Days of Data

## Starting #66daysofdata 2023 [here](https://yshinyong.github.io/66daysofdata/hello-world2)

## [Statistics Fundamentals](https://www.youtube.com/channel/UCtYLUTtgS3k1Fg4y5tAhLbw) 

### 2022-02-16 DAY 1: Histograms, The Main Ideas behind Probability Distributions, The Normal Distribution
<center><img src="https://user-images.githubusercontent.com/25703485/154499858-39d05791-718a-492f-a21b-517138a105a5.png" width="600" height="450" ></center>
_Image from [The Normal Distribution, Clearly Explained!!!](https://www.youtube.com/watch?v=rzFX5NWojp0&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9&index=3)_
- To draw a normal distribution, we need to know:
  1. The avg measurement - tells where the centre of the curve goes
  2. SD of the measurements - tells how wide the curve should be 

### 2022-02-17 DAY 2: Population and Estimated Parameters 

- Normal Distribution Exponential Distribution, Gamma Distribution
![Image](https://gregorygundersen.com/image/moments/total_mass.png)

 _Image from https://gregorygundersen.com/blog/2020/04/11/moments/_

- It's very rare to have population data. In statistics, we often estimate the population parameters using samples/some data points. 
- The more data we have, the more confidence we can have in accuracy of the estimates. 
- **p-values** and **confidence intervals** are often used to quantity the confidence in the estimated parameters 

### 2022-02-18 DAY 3: Mean, Variance and SD, Statistical Model 

 - Formula to calculate, not estimate, the population variance. Firt (Estimated mean x̄ - Population mean μ) for each measurement, square then add all the terms. Lastly we get the average of the square difference (by dividing nb of measurements, n) 
 - The population variance gives values in square. 
 - Population standard deviation = √population variance
 - We almost never have data to calculate the population variance/SD and always work with smaller samples to perform estimation
 - Estimated population variance: Since we don't know population mean (μ), we use sample mean (x̄). And dividing by n - 1 compensates the fact the we are calcualting difference from the sample mean instead of population mean, otherwise we will consistently underestimate the variance around the population mean, as the difference between data and sample mean are normally smaller than the difference between data and population mean. 
  <center><img src="https://miro.medium.com/max/1186/0*Wsf4o0CCGLFGY27L.png" width="500" height="350" ></center>
  _Image from https://medium.com/statistical-guess/sample-variance-cbd0a848acfe_

- What is a model? A model is a way to explore the relationship.

### 2022-02-19 DAY 4: SAMPLING FROM A DISTRIBUTION, HYPOTHESIS TESTING AND THE NULL HYPOTHESIS 
- If there is no preliminary data, there are a lot of possibilities if we were to set hypotheses (e.g. 12h/13h/14h for time to recovers after taking drugs).
- Null hypothesis is useful when we do not have preliminary data.    
- The hypotehesis that there is no difference between things is called the **Null Hypothesis**

### 2022-02-20 DAY 5: ALTERNATIVE HYPOTHESES: MAIN IDEAS
- When we have only 2 groups of data, the **Alternative Hypothesis** is the oppositie of **Null Hypothesis**.
-![image](https://user-images.githubusercontent.com/25703485/154922065-1a61ad0c-7c33-4111-a195-c2d748517414.png)
_Image from [Alternative Hypotheses: Main Ideas!!!](https://www.youtube.com/watch?v=5koKb5B_YWo&list=PLblh5JKOoLUK0FLuzwntyYI10UQFUhsY9&index=9)_
- When we have more than 2 groups of data, we have options for Alternative Hypothesis, we have options on how to set alternative hypothesis and decide which statistical test to use. 
_![image](https://user-images.githubusercontent.com/25703485/154922356-5d818dc6-f04a-4f12-a501-e51a4976cd40.png)_

### 2022-02-21 DAY 6: P-VALUES: WHAT THEY ARE AND HOW TO INTEPRET THEM, HOW TO CALCULATE P-VALUES 
- A p-value is a measure of probability that an observed difference could have occurted just by random chance. 
- The lower the p-value. the greater the statistical significance of the observed difference.
- Using a p-value treshold of 0.00001 means we would only get a False Positive once in every 100,000 experiments. 
- There are 2 types of p-values: one-sided & two-sided
- p-value is determined by adding up the probabilities. A p-value is composed of 3 parts:
i. The probability random chance would result in the observation
ii. The probability of observing something else that is equally rare
iii. The probability of observing something rarer or more extreme

### 2022-02-22 DAY 7: P-HACKING: WHAT IT IS AND HOW TO AVOID IT
- p-hacking refers to the misuse analysis techniques and results in being fooled by false positives.
- TO avoid p-hacking, calculate the p-value for each test and adjust all of the p-values with things like False Discovery Rate to reduce the probability of reporting a False Positive
- If you have p-values that is close to 0.05, don't just add more data to the observation, instead, use data you have for a Power Analysis to determine the correct sample size.

### 2022-02-23 DAY 8: STATISTICAL POWER & POWER ANALYSIS 
- Power is the probability that we will correctly reject the Null Hypothesis. 
- **Power Analysis** is a way to determine sample size for the next time we do this experiment.
- Power is affected 2 factors, i.e. (i) how much overlap there is between 2 distributions we want to identify, and (ii) the sample size, the number of measurements we collect from each group 
- The larger the overlap between 2 distributions, the larger the sample size needs to be in order to have higher power value.

### 2022-02-24 DAY 9: COVARIANCE & CORRELATION
- When the covariance is positive, it tells us the relationship of the 2 sets of observations is positive.
- Covariance is sensitive to the scale of the data, making it difficult to interpret
- The covariance formula is similar to the formula for correlation and deals with the calculation of data points from the **average/mean value** in a dataset. For example, the covariance between two random variables X and Y can be calculated using the following formula (for population):
<center><img src="https://miro.medium.com/max/1186/0*Wsf4o0CCGLFGY27L.png" width="500" height="350" ></center>
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

### 2022-02-25 DAY 10: CONDITIONAL PROBABILITIES 

### 2022-02-26 DAY 11: BAYES' THEOROM
- P(A|B) = [P(B|A) * P(A)] / P(B)
  where:
  - A and B are certain events.
  - P(A) is the probability of event A occurring.
  - Likewise P(B) is the probability of event B occurring.
  - P(A|B) is the conditional probability of event A occurring given that B has happened.
  - Similarly P(B|A) is the conditional probability of event B occurring given that A has happened.

### 2022-02-27 DAY 12: R-SQUARED
-R2 is the perentage of varition explained by the relationship between 2 variables.

<img src="https://user-images.githubusercontent.com/25703485/155865670-32f97d05-622d-4dcd-a6e2-04f590b75520.png" width="400" height="350" >
<img src="https://user-images.githubusercontent.com/25703485/155865690-2f5e5cf9-94ff-498f-a776-402b705837f8.png" width="400" height="350" >

- If statistically significant R2 was 0.9 - we can think that 'the relationship between 2 variables explains 90% of the variation in the data'.
- Is statistically significant R2 was 0.01 - we can think that 'who cares if the relationship is significant, it only accounts for 1% of the variation in the data. How about the remainining 99%?
- R2 is just the square of R. 
- For example, 0.9 times 0.9 = 0.81 i.e. the relationship between 2 variables explain 81% of the variation in the data. 
- If the statistically significant R was 0.5, i.e. 0.5 * 0.5 = 0.25. Thre relationship accounts for 25% of the variation in the data. 
- R2 can be easier to interpret than R.
- R2 does not indicate the direction the correlation because squared numbers are never negative.

### 2022-02-28 DAY 13: THE CENTRAL LIMIT THEOREM, STANDARD DEVIATION VS STANDARD ERROR
- The standard deviation quantifies the variation within a set of measurements.
- The standard error quantifies the variation in the means from multiple sets of measurements.
- The standard deviation of the means is called The Standard Error.
- <img src="https://user-images.githubusercontent.com/25703485/155971251-111d70af-2c56-403e-a3a5-247b420f132a.png" width="400" height="350" >
- We can use **bootstrapping** to calculate the standard errors 
- <img src="https://user-images.githubusercontent.com/25703485/155971457-51f33e1d-a894-44db-be7b-07f6cb4523bd.png" width="400" height="350" >

### 2022-03-01 DAY 14: CONFIDENCE INTERVALS
- There are a lof of ways to calculate confidence intervals, bootstrapping is one of them. 
- A 95% CI means an interval that covers 95% of the means (from multiple bootstrapping)
- ![image](https://user-images.githubusercontent.com/25703485/156166160-35dda818-490b-42d4-950d-37c153ec534b.png)
- Because the interval covers 95% of the means, we know that anything outside of it occurs < 5% of the time. 
- ![image](https://user-images.githubusercontent.com/25703485/156166313-a4df8a34-2eec-4e75-9a51-5455a3d8cc52.png)
- If the 95% CI do not overlap, we know there is a statistically significant difference in the weights of female and male mice. 
- If the CI overlap, there is still a chance that the means are significantly different from each other, so you might have to do t-test.

### 2022-03-02 DAY 15: BOOTSTRAPPING MAIN IDEAS, USING BOOSTRAPPING TO CALCULATE P-VALUES, SAMPLE SIZE AND EFFECTIVE SAMPLE SIZE, BOX PLOT, LOGS
- Main basic steps in bootstrapping:
  i. Make a bootstrapped dataset
  ii. Calculate something (like mean)
  iii. Keep track of that calculation
  iv. Repeat step 1 to 3 a bunch of times. 
![image](https://user-images.githubusercontent.com/25703485/156372611-7c552def-d2d3-4552-954b-aade2f4718b3.png)
- Log:
  - Logs isolate exponents
  - Use a log scale/axis when talking about fold change. This puts positive and negative fold changes on a symmetric scale. 

### 2022-03-03 DAY 16: THRESHOLDS FOR SIGNIFICANCE, ONE OR TWO TAILED P-VALUES
- p-value of 0.05 - always the best to use?
- If your data are barely correlated/ low r-squared, then the results might not be interesting regardless of the p-value

### 2022-03-04 DAY 17: BINOMIAL DISTRIBUTION AND TEST, QUANTILES AND PERCENTILES, Q-Q PLOT, QUANTILE NORMALIZATION
 ![image](https://user-images.githubusercontent.com/25703485/156783668-8fdbccfc-9417-4345-a124-3203a0d0bfd6.png)
- Quantile-quantile (QQ) plots are used to determine if the data can be approximated by a statistical distributed. For e.g., if you are wondering if your data is normally distributed/ uniform ditributed, you can use QQ plot to check.  
- ![image](https://user-images.githubusercontent.com/25703485/156785436-34d148e5-9e09-4df5-98f2-de72d0cf9dd5.png)
- Quantile Normalization: To help us to compare data that has al kinds of noise in it. E.g., quantile normalization is performed when we do microarray experiment. The genes in different samples have different level of expression could be due to biological difference, or technical difference like if you have better lightbulb for one experiment, you would likely to have higher light intensity for certain sample/experiment. 
- ![image](https://user-images.githubusercontent.com/25703485/156786957-eedcf948-8a27-46d4-ba20-27dc23808f8c.png)

### 2022-03-05 DAY 18: PROBABILITY IS NOT LIKELIHOOD, MAXIMUM LIKELIHOOD
![image](https://user-images.githubusercontent.com/25703485/156874945-4286a1cd-9980-4b3b-ba4c-9f896d27ae67.png)
![image](https://user-images.githubusercontent.com/25703485/156875445-d2108756-e017-4cd4-95b7-923f87d279ba.png)
 
### 2022-03-06 DAY 19: WHY DIVIDING BY N UNDERESTIMATES THE VARIANCE
- The differences between the data and the sample mean tend to be smaller than the differences between data and population mean. 
![image](https://user-images.githubusercontent.com/25703485/156905911-ea9d9993-8788-461e-b293-9233141b9d67.png)

### 2022-03-08 DAY 20: MAXIMUM LIKELIHOOD FOR BINOMIAL DISTRIBUTION, MAXIMUM LIKELIHOOD FOR NORMAL DISTRIBUTION

### 2022-03-12 DAY 21: PYTHON PANDAS
- Missed a few days of #66daysofdata due to many projects at work :( Taking a break from statistic video. Refreshing all the syntaxs in Python for my use case at work. 
- Python Equivalent to SQL Rank from Stackoverflow:
  - df['date'] = pd.to_datetime(df['date'])
  - df['rank'] = df.groupby('id')['date'].rank(method='dense').astype(int)

### 2022-03-13 DAY 22: PROBABILITY CONCEPTS EXPLAINED: INTRODUCTION
- **MARGINAL PROBABILITY**: If A is an event, then the marginal probability is the probability of that event occurring, P(A)
- **JOINT PROBABILITY**: The probability of the intersection of two or more events.If A and B are two events then the joint probability of the two events is written as P(A ∩ B)
- 'and' rule: When the events are independent from each other, the joint proababilityis the product of the individual marginal probabilities of the event.  P(A ∩ B) = P(A) ✕ P(B).
- 'or rule': We have to add the individual probabilities and substract the intersection.P(A ∪ B) = P(A) + P(B) - P(A ∩ B). Check the venn diagram of the reference. 
- **CONDITIONAL PROBABILITY**: The probability that some event(s) occur given that we know other events have already occurred. If A and B are two events then the conditional probability of A occurring given that B has occurred is written as P(A|B). 
- Reference: https://towardsdatascience.com/probability-concepts-explained-introduction-a7c0316de465

### 2022-03-15 DAY 23: PROBABILITY CONCEPTS EXPLAINED: RULES OF PROBABILITY
- Rules of Probability (Axioms)
-  i. Axiom 1: The probability of an event is bigger than or equal to 0. The probability of an event is between 0 and 1 (inclusive)
-  ii. Axiom 2 : The probability of at least one of the possible outcomes happening is 1. 
-  iii. Axiom 3: The axiom says if 2 events are mutually exclusive (i.e. the 2 events can’t occur at the same time), then the probability of either of them happening is equal to the sum of the individual probabilities of them happening.
- Reference: https://medium.com/towards-data-science/probability-concepts-explained-rules-of-probability-introduction-part-2-2a9d5a1a9df4

### 2022-03-16 & 17 DAY 24 & 25: PROBABILITY CONCEPTS EXPLAINED: PROBABILITY DISTRIBUTIONS
- Probability distribution - a list of all of the possible outcomes of a random variable along with their corresponding probability values. 
- Probability mass functions is a probability function to describe a **discrete probability distribution**
- Example of discrete probability distribution is The Bernoulli distribution, which describes the probability distribution of a process that has 2 possible outcomes. E.g. coin toss - head/tail. Another example of discrete probability distribution is rolling a fair six-sided dice
- Probabillity density functions is used to describe a **continuous probability distribution**
- Example of continuous probability distribution: Normal distribution 
- The output of a probability mass function is a probability
- The area under curve produced by a probability density function represents a probability. 
- Parameter is important - wrong parameters can give results that differ wildly!
- Reference: https://towardsdatascience.com/probability-concepts-explained-probability-distributions-introduction-part-3-4a5db81858dc

### 2022-03-19 DAY 26: PROBABILITY CONCEPTS EXPLAINED: MAXIMUM LIKELIHOOD ESTIMATION
- Maximum likelihood estimation - a method that detemines values for the parameters of a model. 
- The parameter values are found such that they maximise the likelihood that the process described by the model produced the data that were actually observed.
- Reference: https://medium.com/towards-data-science/probability-concepts-explained-maximum-likelihood-estimation-c7b4342fdbb1

### 2022-03-20 & 21 DAY 27 & 28: PROBABILITY CONCEPTS EXPLAINED: BAYESIAN INFERENCE FOR PARAMETER ESTIMATION
- Reference: https://medium.com/towards-data-science/probability-concepts-explained-bayesian-inference-for-parameter-estimation-90e8930e5348

### 2022-03-22 & 23 DAY 29 & 30: CANNIBALIZATION STUDY 
- Working on my cannibalization study and refreshed my knowledge on some syntax:
- For example, venn diagram - matplotlib's venn2 and venn3 - can draw up to 3 sets only 
- Reference: https://stackoverflow.com/questions/19841535/python-matplotlib-venn-diagram

### 2022-03-24 - 2022-04-02 DAY 31 - 38: GRADIENT BOOST 
- Gradient boosting is one of the boosting algorithms to minimize bias error. 
- Gradient bossting can be used for both regression and classification. When it is the regressor, the cost function is mean square error while when it is classifier, the cost function is Log loss. 
- When we use Gradient Boost for Regression
  - We start with a leaf that is the average value of the variable that we want to predict (e.g. weight as target variable)
  - Then we add a tree based on the **Residuals** (not weight), which is the difference between Observed and Predicted values 
  - Then we scale the tree's contribution to the final Prediction with a **learning rate**
  - Then add another tree based on new residuals and keep adding trees based on errors made by previous tree.
  - In practice, people often set the max number of leaves to be 8 - 32.
  - Steps:
    - Input: data & a differentiable Loss Function (1/2 * (observed - predicted)^2 is one te most commonly used loss function for regression with Gradient Boost). When we remove 1/2, it's similar to linear regression. 
    - Step 1: Initialize the model with a constant value  
    - Step 2: For m = 1 to M (m means nb of tree, and M means max nb of tree)
      -  a. Calculate new residuals for the new predictions
      -  b. Create a new tree
      -  c. Calculate output values 
      -  d. Make new predictions
  - References: 
    - StatQuest
    - https://www.analyticsvidhya.com/blog/2021/04/how-the-gradient-boosting-algorithm-works/


### 2022-04-03 DAY 39: BASIC EMSEMBLE LEARNING
  - 2 most popular ensemble methods are **bagging** and **boosting**. 
      i. Bagging: Train a bunch of individual models in *parallel*. Each model is trained by a random subset of data
        - Example: Random Forest- select random subsets from training data, train _n_ decision trees, each individual tree predicts the records in test data indepedently. Then make final prediction. RF uses the class with the majority vote as final prediction. 
      ii. Boosting: Train a bunch of individual models in *sequential*. Each  model learns from mistakes made by the previous model. 
        - Example: AdaBoost (adaptive boosting). 
          - Step 0 Initialize the weights of data points. 
          - Step 1: Train the decision tree 
          - Step 2: Caluclate the weighted error rate.
          - Step 3: Calculate the decision tree's weight in the ensemble 
          - Step 4: Update weights of wrongly classified points 
          - Step 5: Repeat Step 1 (until nb trees we set to train)
          - Step 6: Make final prediction 
        - Example: Gradient boosting
          - Gradient boosting learns from the mistake - residual error directly, rather than update the weights of data points. 
      
  - Reference:
    - https://medium.com/towards-data-science/basic-ensemble-learning-random-forest-adaboost-gradient-boosting-step-by-step-explained-95d49d1e2725
 
 
### 2022-04-04 - 2022-04-05 DAY 40 - 41: REGRESSION METRIC
- MSPE, MSAE, R square, adjusted R square
- Root mean square error: sample standard deviation of the difference between predicted and observed values (called residues)
- MAE: Average of the absolute difference between predicted and observed values  
- MAE takes the average of the offsets directly, RMSE penalizes the higher difference between more than MAE
- Adjusted R2 vs R:
  - Adjusted R² will consider the marginal improvement added by an additional term in the model. It will increase if you add the useful terms and it will decrease if you add less useful predictors. However, R² increases with increasing terms even though the model is not actually improving.
- References:
  - https://medium.com/usf-msds/choosing-the-right-metric-for-machine-learning-models-part-1-a99d7d7414e4
  - https://medium.com/towards-data-science/regression-an-explanation-of-regression-metrics-and-what-can-go-wrong-a39a9793d914

### 2022-04-08 DAY 42: RFM
- I am doing member analysis for my day job. Read about RFM.
- Reference: https://medium.com/marketingdatascience/%E5%B8%B8%E8%B2%B4%E5%AE%A2-%E6%96%B0%E5%AE%A2-%E8%AE%93rfm%E6%A8%A1%E5%9E%8B%E7%B0%A1%E7%B0%A1%E5%96%AE%E5%96%AE%E8%A7%A3%E9%87%8B%E4%B8%80%E5%88%87-%E9%99%84%E5%AF%A6%E7%8F%BE%E7%A8%8B%E5%BC%8F%E7%A2%BC-cd7f45fb3e30
 
### 2022-04-09 DAY 43: COVARIANCE, CORRELATION, R-SQUARE

### 2022-04-10 DAY 44: R-SQUARED VS ADJUSTED R-SQUARE
- R SQUARED, A.K.A coefficient determination, define the degree to which the variance in the dependence variable (target) can be explained by the independent variable (features).
- R squared is calculated by dividing the sum of squares of residuals from the regression models by the total sum of squares of errors from the average model and then subtract it from 1. 
- Adjusted R squared - penalize for adding features which are not useful for predicting the target
- If R2 increases sinificantly, then the adjusted r-squared increases.
- Id there is no significant change in R2, then the adjusted R2 would decrease. 
- Reference: https://medium.com/analytics-vidhya/r-squared-vs-adjusted-r-squared-a3ebc565677b

### 2022-04-11 DAY 45: ML & DATA STORYTELLING
1. https://towardsdatascience.com/5-data-storytelling-tips-for-creating-more-persuasive-charts-and-graphs-150f3544b4e8
2. https://towardsdatascience.com/data-storytelling-improve-insight-to-action-conversion-for-a-greater-real-world-impact-b94e1827fa01
3. https://medium.com/towards-data-science/all-machine-learning-algorithms-you-should-know-in-2022-db5b4ccdf32f

### 2022-04-19 & 20 DAY 46-47: FITTING A LINE TO DATA, MUTIPLE LINEAR REGRESSION

### 2022-04-21 DAY 48: POLYNOMIAL REGRESSION
- Reference: https://www.analyticsvidhya.com/blog/2021/07/all-you-need-to-know-about-polynomial-regression/#:~:text=Polynomial%20Regression%20is%20a%20form%20of%20Linear%20regression%20known%20as,also%20badly%20affect%20the%20performance.

### 2022-04-23 DAY 49: WHAT IS THE ASSUMPTION OF LINEARITY IN LINEAR REGRESSION 
- We can check for linearity by evaluating a Residuals vs Fitted plot. X values are the fitted values from our linear model, and y values are the residuals for the fitted values. 
- Reference: https://medium.com/the-data-base/what-is-the-assumption-of-linearity-in-linear-regression-3ed67ad8ef93

### 2022-04-26 DAY 50: DISTRIBUTION
https://towardsdatascience.com/econometrics-is-the-original-data-science-6725d3f0d843

### 2022-04-27 & 28 DAY 51 & 52: VISUALIZE THE BUSINESS VALUE OF PREDICTIVE MODELS  
- 4 plots - cumulative gains, cumulative lift, response and cumulative response
- Gains plot 
https://medium.com/broadhorizon-cmotions/visualise-the-business-value-of-predictive-models-21c6bc8132c

### 2022-05-03 DAY 53: DATA INSPIRED/DATA DRIVEN?
- Recommendation from the article: setting your decision criteria in advanced
- Reference: https://hackernoon.com/data-inspired-5c78db3999b2

### 2022-05-04 DAY 54: GA4 VS UNIVERSAL ANALYTICS
- Universal Analytics (GA3) will be discontinued from 1st July 2023
- GA3 is based on sessions & pageviews while GA4 is based one events & parameters.
- A session is a combination of page views, events, transactions or more by 1 user within a given timeframe. It's like a container of actions taken by a user. While GA4 is not limited by time. It doesn't create new sessions for source changes mid-session - the session count might be lower
- GA4 does not have bounce rate - New metric: engagement rate
- IP anonymisation - GA4, IPs are automatically anonymised. 
- Landing page reports - we can find out how many times the 'session start event' is triggered on a particular page. 
- App & site monitoring - cross platform 
- GA4 is natively connected to BigQuery 
- GA4 data expires after 14 months
- Reference: https://www.ruleranalytics.com/blog/insight/google-analytics-4/

### 2022-05-05 DAY 55: A/B TESTING
- Before the launch of experiment:
  1. Think about the product & talk with PM: Evaluate the feasibility and IMPACT. Ask questions like what are the hypothesis, can we find calculable metrics to test, what's the risk
  3. Design the experiment: (i) what are the evaluation metrices - better to have lower variance and sensitive to changes. (ii) Unit of Diversion - randomized based on session or user? (iii) Min required sample (iv) experiment duration & traffic portion (v) experiment layer & type 
  4. A/A variation: A/A variation is the difference in key metrics between control group and another control group. There should be no statistically significantly differences between the two.

- During the experiment:
  5. Check the invariant metrics & experiment set-up
  6. Monitor key evaluation metrices

- After the end of the experiment:
  7. Check p-values, magnitudes of difference, minimum detectable effects & dive deeper when surprise
  8. Formulate product recommendations
  9. Write report
- Reference: https://medium.com/towards-data-science/typical-9-step-a-b-test-workflow-for-data-scientists-in-2022-d672c9a0d658

### 2022-05-07-09 DAY 57-59: REGULARIZATION 
- Lasso (L1) REGRESSION & Ridge Regression - quite similar
![image](https://user-images.githubusercontent.com/25703485/167258650-66ece07f-38ae-4a4a-b7b7-ee6cb3eeaf7f.png)
- Lasso regression can exclude useful variables - a little better than Ridge at reducing the variance in models that contains many useless variables. Ridge regression tends to do a little better when most variables are useful
- Reference: Statquest

### 2022-05-19 - 21 DAY 60 - 62: WEB ANALYTICS
- Learned new tool for work - Contentsquare 

### 2022-07-15 FORECAST
- Back testing 
- Data drift 
- Reference: Hands-on time series analysis, open source, R, MLOps - The Data Scientist Show 
