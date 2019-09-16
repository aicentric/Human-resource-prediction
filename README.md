# Human-resource-prediction
Predicting attrition in an organization using machine learning on employee data

Implemented a Logistic regression model which would be able to predict whether an employee would leave the company or not. This model would be useful in identifying discontent employees so that the HR department could take action before the employee left the company.
Logistic regression can be used whenever an individual is to be classified into one of two populations. Logistic regression analysis requires knowledge of both the dependent (or outcome) variable and the independent (or predictor) variables in the sample being analyzed (Afifi, Abdelmonem_ Clark, Virginia A._ May, Susanne Practical Multivariate Analysis)
For a given training set with N labeled training examples (xi,yi)} with i = 1, 2,… , N with input data xi є Rn and corresponding binary target labels yi є {0, 1}, the logistic regression tries to estimate the probability P(y = 1|x) given by
P(y = 1|x) = 1/[1 + exp(-(w0 + wx))]
with x є Rn being equal to an n-dimensional input vector, w to the parameter vector and w0 to the intercept. The parameters w0 and w are
usually estimated using a maximum likelihood procedure (Hosmer &Lemeshow, 2000)
We have data of 15000 employees that worked in the organization. We have used this data to create a model that can predict whether a current or future employee will leave the organization or not. The dataset was split into two parts in the ratio of 4:1
Training dataset of about 12000 employees
Testing dataset of about 3000 employees
We used the training dataset and created a prediction model using logistic regression using R. From analyzing the results of this model, we could see that satisfaction level, number of projects, average monthly hours, time spent at the company, work accident were important variables in this prediction model. As department was not an important variable in the model we also created a logistic regression model after removing variable department to see if the Null deviance and AIC decreased. But both of these values increased on removing the department variable from the model. Therefore, we decided to continue with the first logistic regression model which had lower AIC value as the model with the least AIC emerges as the most adequate and is chosen. 

