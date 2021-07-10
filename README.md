# A/B-Testing-for-Data-Science-using-Python 

A/B Testing for Data Science using Python

A/B testing is a popular way to test your products and is gaining steam in the data science field

 Scenario – One compnay has  made certain changes to their website recently. Unfortunately, they have no way of knowing with full accuracy how the next 100,000 people who visit their website will behave. That is the information we cannot know today, and if we were to wait until those 100,000 people visited our site, it would be too late to optimize their experience.
 
 This is where a A/B test can be useful. A data scientist collects and studies the data available to help optimize the website for a better consumer experience. And for this, it is imperative to know how to use various statistical tools, especially the concept of A/B Testing.

What is A/B testing?

A/B testing is a basic randomized control experiment. It is a way to compare the two versions of a variable to find out which performs better in a controlled environment.

For instance, let’s say you own a company and want to increase the sales of your product. Here, either you can use random experiments, or you can apply scientific and statistical methods. A/B testing is one of the most prominent and widely used statistical tools.

In the above scenario, you may divide the products into two parts – A and B. Here A will remain unchanged while you make significant changes in B’s packaging. Now, on the basis of the response from customer groups who used A and B respectively, you try to decide which is performing better.

It is a hypothetical testing methodology for making decisions that estimate population parameters based on sample statistics. The population refers to all the customers buying your product, while the sample refers to the number of customers that participated in the test.


#### How does A/B Testing Work?

Let’s say there is an e-commerce company XYZ. It wants to make some changes in its newsletter format to increase the traffic on its website. It takes the original newsletter and marks it A and makes some changes in the language of A and calls it B. Both newsletters are otherwise the same in color, headlines, and format.

##### Objective
Our objective here is to check which newsletter brings higher traffic on the website i.e the conversion rate. We will use A/B testing and collect data to analyze which newsletter performs better.

###### 1.  Make a Hypothesis

In hypothesis testing, we have to make two hypotheses i.e Null hypothesis and alternative hypothesis. Let’s have a look at both.

 ###### Null hypothesis or H0:
 
The null hypothesis is the one that states that sample observations result purely from chance. From an A/B test perspective, the null hypothesis states that there is no difference between the control and variant groups. It states the default position to be tested or the situation as it is now, i.e. the status quo. Here our H0 is ” there is no difference in the conversion rate in customers receiving newsletter A and B”.

Alternative Hypothesis or H0:
The alternative hypothesis challenges the null hypothesis and is basically a hypothesis that the researcher believes to be true. The alternative hypothesis is what you might hope that your A/B test will prove to be true.

In our example, the Ha is- “the conversion rate of newsletter B is higher than those who receive newsletter A“.

Now, we have to collect enough evidence through our tests to reject the null hypothesis.

 

###### 2. Create Control Group and Test Group
Once we are ready with our null and alternative hypothesis, the next step is to decide the group of customers that will participate in the test. Here we have two groups – The Control group, and the Test (variant) group.

The Control Group is the one that will receive newsletter A and the Test Group is the one that will receive newsletter B.

For this experiment, we randomly select 1000 customers – 500 each for our Control group and Test group.

Randomly selecting the sample from the population is called random sampling. It is a technique where each sample in a population has an equal chance of being chosen. Random sampling is important in hypothesis testing because it eliminates sampling bias, and it’s important to eliminate bias because you want the results of your A/B test to be representative of the entire population rather than the sample itself.

Another important aspect we must take care of is the Sample size. It is required that we determine the minimum sample size for our A/B test before conducting it so that we can eliminate under coverage bias. It is the bias from sampling too few observations.

 

###### 3. Conduct the A/B Test and Collect the Data
One way to perform the test is to calculate daily conversion rates for both the treatment and the control groups. Since the conversion rate in a group on a certain day represents a single data point, the sample size is actually the number of days. Thus, we will be testing the difference between the mean of daily conversion rates in each group across the testing period.

When we run our experiment for one month, we noticed that the mean conversion rate for the Control group is 16% whereas that for the test Group is 19%.

### Statistical significance of the Test
Now, the main question is – Can we conclude from here that the Test group is working better than the control group?

The answer to this is a simple No! For rejecting our null hypothesis we have to prove the Statistical significance of our test.

There are two types of errors that may occur in our hypothesis testing:

##### Type I error:
We reject the null hypothesis when it is true. That is we accept the variant B when it is not performing better than A

##### Type II error: 
We failed to reject the null hypothesis when it is false. It means we conclude variant B is not good when it performs better than A
To avoid these errors we must calculate the statistical significance of our test.

That means the difference between your control version and the test version is not due to some error or random chance. To prove the statistical significance of our experiment we can use a two-sample T-test.

The two–sample t–test is one of the most commonly used hypothesis tests. It is applied to compare whether the average difference between the two groups.

To understand this, we must be familiar with a few terms:



![test_sta](https://user-images.githubusercontent.com/50706192/124101634-dbd74a80-da5f-11eb-8d3c-a5fe131ef3d7.png)




( courtesy: https://www.analyticsvidhya.com/blog/2020/10/ab-testing-data-science/)



 


