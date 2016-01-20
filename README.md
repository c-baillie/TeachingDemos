# TeachingDemos
## Synthetic Data
### Friedman Dataset
Synthetic data set suggested by Friedman as a benchmark dataset. The cases are generated using the following method: 
- Generate the values of 5 attributes, X1, ..., X5 independently each of which uniformly distributed over [0.0, 1.0]. Obtain the value of the target variable Y using the equation: 
- y=10(sin(PI)x1x2)+20(x3-0.5)2+10x4+5x5+e  
![equation](http://www.sciweavers.org/tex2img.php?eq=f%28x%29%20%3D%200.1e%20%5E%7B4x_%7B1%7D%7D%20%2B%20%20%5Cfrac%7B4%7D%7B1%2Be%5E%7B-20%28%20x_%7B2%7D%3D0.5%7D%7D%20%2B%203%20x_%7B3%7D%2B2%20x_%7B4%7D%20%2B%20x_%7B5%7D%20%20%20&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=0)                   
![equation](http://www.sciweavers.org/tex2img.php?eq=f%28x%29%20%3D%200.1e%20%5E%7B4x_%7B1%7D%7D%20%2B%20%20%5Cfrac%7B4%7D%7B1%2Be%5E%7B-20%28%20x_%7B2%7D%3D0.5%7D%7D%20%2B%203%20x_%7B3%7D%2B2%20x_%7B4%7D%20%2B%20x_%7B5%7D%20%20%20&bc=White&fc=Black&im=png&fs=12&ff=arev&edit=0)
- Where e is a Gaussian random noise N(0,1)

```r
model = lm(y~x, data=data, family="binomial")
plot(model)
```
![](OPLS_example_files/figure-html/unnamed-chunk-9-1.png)

**REFERENCES**               
Jerome H. Friedman, Multivariate adaptive regression splines, The Annals of Statistics, 19(1):1-141, 1991. 
Leo Breiman, Jerome H. Friedman, Charles J. Stone and R. A. Olson, Classification and Regression Trees, Chapman and Hall, 1984

**Equations**         
Editing done with (http://www.sciweavers.org/free-online-latex-equation-editor) + google docs insert with (). 
