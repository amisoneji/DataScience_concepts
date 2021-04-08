**Logistic Regression**:

Logistic regression is one of the most common machine learning algorithms used for binary classification. 
It predicts the probability of occurrence of a binary outcome using a logit function. 
Logistic regression usually applied to  problem statements where two classification problems can linearly separable(separated  by linear line). 

**Linear vs Logistic:**

- Linear Regression is used when our dependent variable is continuous in nature for example weight, height, numbers, etc. and in contrast, Logistic Regression is used when the dependent variable is binary or limited for example: yes and no, true and false, 1 or 2, etc.

- Linear regression uses the ordinary least square method to minimize the error and arrives at the best possible solution, and the Logistic regression achieves the best outcomes by using the maximum likelihood method.
______________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________
- Logistic regression solves task by learning, from a training set, a vector of weights and a bias term. 

- Each weight wi is a real number, and is associated with one of the input features xi . 

- The weight wi represents how important that input feature is to the classification decision, and can be positive (providing evidence that the instance being classified belongs in the positive class) or negative (providing evidence that the instance being classified belongs in the negative class). 

- The bias term, also called the intercept, is intercept another real number that’s added to the weighted inputs. To make a decision on a test instance— after we’ve learned the weights in training— the classifier first multiplies each xi by its weight wi , sums up the weighted features, and adds the bias term b. The resulting single number z expresses the weighted sum of the evidence for the class. 

                                      Z=( ∑_(i=1)^n wixi) +b

- As we find  the distance between positive points in positive direction,and negative point in negative direction our term become  positive so we can say that the points are properly claasified whereas if positive point in negative direction or negative point in positive direction and vice versa we got term negative so we can say that those points are not properly classified.

- As we know the cost function(optimizer) value should be maximum for best line & if the outlier present in our data max doesn't occure and it hard to cover outlier so for prevent this we introduce the sigmoid function.
- It is a mathematical function having a characteristic that can take any real value and map it to between 0 to 1 shaped like the letter "s". The sigmoid function also called a logistic function.

                                       Y = 1 / 1+e –z

- So, if the value of z goes to positive infinity then the predicted value of y will become 1 and if it goes to negative infinity then the predicted value of y will become 0. 
- And if the outcome of the sigmoid function is more than 0.5 then we classify that label as class 1 or positive class and if it is less than 0.5 then we can classify it to negative class or label as class 0.
 
- The logistic regression model is not only a classification model, but also gives you probabilities. This is a big advantage over models that can only provide the final classification. Knowing that an instance has a 99% probability for a class compared to 51% makes a big difference.




