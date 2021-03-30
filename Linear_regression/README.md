**Linear Regression:**

- From linear regression will try to create best fit line such that Best line indicate prediction from the features.
- In linear Regression if one feature(unit change in x)changes  for that change what prediction parameter(feature or target ) will change(change in y) and that changes what slop occur(m)(liner equation for one feature :y=mx+c).
- We try to draw multiple fit lines for data & minimize the distance between fit line and actual data.
- The distance from fit line & point is simply called as error and if we sum all the errors for our scattered data points  the error must be minimal error, and in such case that fit line is our best fit line for model.
- That best fit line give us some value of m (slope) & intercept ( c ).
The error equation:

MSE =1/n∑_(i=1)^n(ŷi –yi)2


The primary set-up for learning neural networks is to define a cost function (also known as a loss function) that measures how well the network predicts outputs on the test set.
The goal is to then find a set of weights and biases that minimizes the cost. One common function that is often used is the mean squared error, which measures the difference between the actual value of y and the estimated value of y (the prediction).

ŷ =1/2m∑_(i=1)^m(ŷ –y)2
ŷ = The point of best fit line that we predict
y = Real scattered point

Our goal is to reach global minima (when slop will become zero)
In order to get the lowest error value, we need to adjust the weights and to reach the smallest possible error. This is because the result of a lower error between the actual and the predicted values means the algorithm has done a good job in learning. Gradient descent is an efficient optimization algorithm that attempts to find a local or global minimum of a function.

**Convergence Theorem**:
To solve for the gradient, we iterate through our data points using our new weight and bias values and compute the partial derivatives. This new gradient tells us the slope of our cost function at our current position (current parameter values) and the direction we should move to update our parameters.(the m value should subtract with derivative of m with respect to m multiple by  α)

m=m -  ∂m/dm α

**learning rate (α)**

-The size of these steps is called the learning rate (α) that gives us some additional control over how large of steps we make. 
-With a large learning rate, we can cover more ground each step, but we risk overshooting the lowest point since the slope of the hill is constantly changing.
-With a very low learning rate, we can confidently move in the direction of the negative gradient since we are recalculating it so frequently. A low learning rate is more precise, but calculating the gradient is time-consuming, so it will take us a very long time to get to the bottom. The most commonly used rates are: 0.001, 0.003, 0.01, 0.03, 0.1, 0.3.


