# TeachingDemos
## Synthetic Data
### Friedman Dataset
Synthetic data set suggested by Friedman as a benchmark dataset. The cases are generated using the following method: 
- Generate the values of 5 attributes, X1, ..., X5 independently each of which uniformly distributed over [0.0, 1.0]. Obtain the value of the target variable Y using the equation: 
- y=10(sin(PI)x1x2)+20(x3-0.5)2+10x4+5x5+e           
- Where e is a Gaussian random noise N(0,1)

```r
model = lm(y~x, data=data, family="binomial")
plot(model)
```

**REFERENCES**
Jerome H. Friedman, Multivariate adaptive regression splines, The Annals of Statistics, 19(1):1-141, 1991. 
Leo Breiman, Jerome H. Friedman, Charles J. Stone and R. A. Olson, Classification and Regression Trees, Chapman and Hall, 1984
