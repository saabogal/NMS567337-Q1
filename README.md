![Q_banner](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/banner.png)

## ![qlogo](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/qloqo.png) **Quiz Extra**

```yaml

# Name of QuantLet : NMMSQextra

# Published in : Null

# Description : Plot of different mutivariate normal distributions, through
# Kernel estimates

# Keywords : 'Multivariate Normal Distribution, Graphical Representation,
# Random Variables, pdf, Kernel estimates'

# Author : Luis Alejandro Sarmiento Abogado

# Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

# Datafile : Null

```
![Q_image](https://cloud.githubusercontent.com/assets/15620386/11501173/797bc19c-9832-11e5-80a7-3e8aa06225ed.png)

```r

# Clear graphics and data
graphics.off()
rm(list = ls())

# Load Packages
library(MASS)

# Lets first simulate some bivariate normal samples
bivn  = mvrnorm(1000,  mu = c(0, 0), Sigma = matrix(c(8, 2, 2, 5), 2, 2))
bivn2 = mvrnorm(10000, mu = c(0, 0), Sigma = matrix(c(1.5, 0, 0, 1.5), 2, 2))
bivn3 = mvrnorm(100000,mu = c(0, 0), Sigma = matrix(c(1, 0, 0, 1), 2, 2))

# Now, we do a kernel density estimate
bivn.kde  = kde2d (bivn[, 1],  bivn[, 2], n = 50)
bivn.kde2 = kde2d(bivn2[, 1], bivn2[, 2], n = 50)
bivn.kde3 = kde2d(bivn3[, 1], bivn3[, 2], n = 50)

# We now proceed to plot our stimates.
old.par = par(mfrow = c(1, 3))

persp(bivn.kde,  phi = 30, theta = 30, shade = 1, border = NA, col = "beige", scale = TRUE, expand = .6)
persp(bivn.kde2, phi = 30, theta = 30, shade = 2, border = NA, col = "lightblue", expand = 0.6)
persp(bivn.kde3, phi = 30, theta = 30, shade = 2, border = NA, col = "yellow", expand = 0.6)

```
