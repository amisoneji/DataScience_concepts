**R square and Adjusted R square**:

In regression model the way of checking accuracy, the techniques used are called as r square and Adjusted R square (Used for checking goodness of best fit line).

r2  =1-(ssres)/(ssmean)

ssres = sum of residual(error)

ssmean=sum of average 
- if R2 is nearer to 1 the line is best fitted line.
- if R2<0  this value only occurs when best fitline worser then average best fit line.

When we added more number of features, model added new and new coefficients such that the ssres  will decreases and the ratio of ssres/ssmean also decreases so that R2 increases.
If features not correlated the R2 value definitely increases so that we can say that R2 value does not do anything with the features that are not correlated or related.it is not penalizing new added feature.
So, overcome this we use adjusted R2

_________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________________

**Adjusted R square**

R2 adj=1-[(1-R2)(N-1)/N-P-1]

R2=sample R square
P=no. of predictors
N=total sample size

- If independent features are not correlated:
R2 adj= p>>>increases
        >(N-P-1) smaller
        >(1-R2)(N-1)/N-P-1 increases
        >R2 adj decreases
- If independent features are correlated:
R2 adj= >R2 higher
        >(1-R2) smaller
        >R2 adj increases

- Every time add an independent variables to model, the R2 increases, even if the independent variable is insignificant.it never declines. Whereas Adj R2 increases only when independent variable is significant and affects dependent variable.
- Adj R2 value always be less than or equal to R2 value.







