# Analysing The Impact of a New E-commerce Web Page on Conversion Rate (A/B Testing)
 In this project we will run an A/B testing analysis by leveraging the Chi-Square test for independence and assess the impact of a new ecommerce web page on the users conversion rate compared to an old web page.

# Project Summary

## Context

An e-commerce company has developed a new web page in order to try and increase the number of users who "convert," meaning the number of users who decide to pay for the company's product.  

The users were randomly divided into two groups: the treatment group have access to only the new web page and the control group have access to only the old web page.  

The company want understand if they should implement this new page, keep the old page, or perhaps run the experiment longer to make their decision.

## Actions
To perform our analysis, we first explored the data and made some cleanup. We observed there are 3,895 duplicated user_id, some of these users where exposed to both the new and old web pages and some users where in both treatment group and control group. This mismatch entries were about 1.32% of the entire dataset. For the purpose of our analysis we excluded the mismatched data to resolve the disparity.


To compare the conversion rate of the two groups, we used the Chi-Square test for independence. To run the test, we set the following hypothesis and alpha level:

* Null Hypothesis = There is no relationship between landing page type and conversion rate.
* Alternate Hypothesis = There is a relationship between landing page type and conversion rate.
* Alpha = 0.05

## Results & Conclusion
We performed the analysis and obtained the following results:

* users from the ***control*** group had a conversion rate of ***12.03%*** 
* users from the ***treatment*** group had a conversion rate of ***11.88%***  

We noticed the users of the old web page have a bit higher conversion rate than the users of the new web page.  We then performed the Chi-Squared test.

The results obtained from the Chi-Square test gave us a p-value of ***0.19*** which is greater than our alpha value of ***0.05*** and a chi-square statistic of ***1.71*** which is less than our critical value of ***3.84***.  
Hence we failed to reject the Null Hypothesis and concluded that there was no significant difference between the conversion rates of the old landing page and the new landing page.  

In conclusion, our analysis showed that it will not be a good idea for the company to change their old web page for the new one at the moment.  
We recommended that the company runs the experiment again to collect more data and make sure users from each group only access the web page their supposed to access. Doing that may help us obtain more insight.
