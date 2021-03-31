**Ridge Regression & Lasso Regression:**

Ridge and lasso regression lead to less variance.
They work by penalizing the magnitude of coefficients of features along with minimizing the error between predicted and actual observations. These are called regularization techniques. The key difference is in how they assign penalty to the coefficients.

When training data set model give us low bias or less error result & for test data set it give us huge residuals error then model is called **overfitting** model whenever we got huge error for both training data and test data model is called **underfitting** model.

When we change one unit in independent parameter and if dependent parameter change is so huge the model goes on high stripper. For good accuracy model want the down the stripper. Stripper basically indicates the slopes of features. High strip slope causes overfitting.
For ridge the equation becomes:     
 ∑_(i=1)^m(ŷ –y)2 + λ * slope    

If we have many features the slop equation become λ  +(m1+m2+………..mn)

As the value of λ increases, the model complexity reduces. Though higher values of λ reduce overfitting, significantly high values can cause underfitting as well. Thus λ   should be chosen wisely. A widely accept technique is cross-validation, i.e. the value of alpha is iterated over a range of values and the one giving higher cross-validation score is chosen.

**Lasso Regression:**

Lasso stands for least absolute shrinkage and selection  operator.As name suggest it is use for overcome the overfitting as well as also used for feature selection. When we have more number of features generally we have to drop strongly correlated features.
 ∑_(i=1)^m(ŷ –y)2 + λ * |slope|

Feature slop will move towards zero whenever slop will be very less. Those feature will remove.

- For the same values of  λ  , the coefficients of lasso regression are much smaller as compared to that of ridge regression .
- For the same λ  , lasso has higher RSS (poorer fit) as compared to ridge regression.
- Many of the coefficients are zero even for very small values of λ  

                                                                                                                                                                                                    
                                  

