![Q_banner](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/banner.png)

## ![qlogo](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/qloqo.png) **Quiz Ten**

Name of QuantLet : NMMSQ10

Published in : Null

Description : 'An example of random variables nor following asymptotic normality, for this specific example a Cauchy set of random variables was selected and its asymptotic behavior compared with both Binomial and normal distributions'.

Keywords : 'Asymptotic Normal Distribution, Graphical Representation, Random Variables, Cauchy, Binomial, pdf'

Author : Luis Alejandro Sarmiento Abogado

Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

Datafile : Null

R

# Load Packages
library(MASS)
library(KernSmooth)

# Random generation of a bynomial distribution
p = 0.5
n = 1000

# Random generation of the binomial distribution with parameters 1000*n
# and 0.5

bsample  = rbinom(n * 1000, 1, 0.5)

# Create a matrix of binomial random variables

bsamplem = matrix(bsample, n, 1000)

# Compute kernel density estimate

bden = bkde((colMeans(bsamplem) - p)/sqrt(p * (1 - p)/n))

# Proceed to plot the three distributions

pdf(file = "distributions.pdf", width = 15, height = 10)
plot(bden, col = "blue3", type = "l", lty = 1, lwd = 1, xlab = "1000 Random Samples", 
     ylab = "Estimated and Normal Density", cex.lab = 1, cex.axis = 1, ylim = c(0, 
                                                                                0.45))

plot(dnorm,   -4, 4, n = 1000, col = "Green", add = TRUE)

plot(dcauchy, -4, 4, n = 1000, col = "red", add = TRUE)
