My JSC370 Final Project Website

This is my JSC370 Final Project website home. The website is online at https://sean-1005.github.io/jsc370-final-project/.

# Introduction 

This is the final project for JSC370. For this final project, I would like to do a research on 

**What are the main factors related to the salary of datascientist?**

We are interested in this specific research question since answering this question can give us a preliminary understanding of our possible future development working in a company. Besides, we are also interested in whether there is gender discrimination when it comes to the salaries of male data scientists and female data scientists. Our goal for this research is to build a statistical model which is best for explaining the relationship between salary, and other possible predictors. And we may use our model to predict the salary that we may receive in out future career.

Our dataset was scraped off levels.fyi and then cleaned by the author. The license[1] of this data set is including in the *Reference* section. According to the terms and conditions of the website, people may use the data for personal, non-commercial purposes (mentioned in the last sentence in the "License" section).

# Method

We are using linear regression, regression tree, random forest, bagging, boosting models to analyze the data. 

# Conclusion

The most significant factors that would affect salary are years working at company, years of experience, Gender, if obtaining Bachelor’s degree, Master’s Degree, Doctor’s degree.

The relationships between response and each predictors are as follow:

-   years working at company: negative

-   years of experience: positive

-   gender: positive

- if obtaining Bachelor’s degree: negative
- if obtaining Master’s degree: negative
- if obtaining Doctor’s degree: positive



According to the above relationships, we are not surprising to see that if you are more experienced, you will earn more.

However, there are some interesting facts that people work longer in a company, they will earn less. This could be caused by some extreme outliers in the dataset. Usually, employees will at least stay at the same salary level throughout the duration of working at the companies. Another one is that people having a bachelor’s or master’s degree earn less than those does not have. All the information on the degree is recorded by 0 and 1 without NA. Thus, 0 may be the default value for the column, which may represent not having that degree or unknown. This may influence the result and cause interesting facts.

Another funny fact is that female earns more than males. Because of many facts of gender inequality, in reality, females earn less than males in the same positions, to some degree. I think this may show an improvement in gender equality nowadays. Another reason may be the percentage of females in this dataset is much smaller than males, thus, the data of females in this dataset is less representative. However, I would like to believe that we have a more open, less discriminatory working environment for females than in the past.

For the machine learning model, I have tried all kinds of models that we learned, only the regression tree models give us the least mse, which is 3797.952. However, the mse is still significantly large.

Overall, only according to the result, experience is the most important factor to earn more. And generally, females earn more than males when working as data scientists.
