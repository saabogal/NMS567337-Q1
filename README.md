![Q_banner](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/banner.png)

## ![qlogo](https://github.com/QuantLet/Styleguide-and-Validation-procedure/blob/master/pictures/qloqo.png) **Quiz Two**

```yaml

Name of QuantLet : NMMS2

Published in : Null

Description : 'Plot if Right and leftskewed asymetric normal distributions' 

Keywords : 'Asymetric Normal Distribution, Skeweness, pdf, histogram'

Author : Luis Alejandro Sarmiento Abogado

Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

Datafile : Null
```
![Q_image](https://cloud.githubusercontent.com/assets/15620386/11501538/45696f1e-9835-11e5-80cf-e912fd50923f.png)
![Q_image](https://cloud.githubusercontent.com/assets/15620386/11501538/45696f1e-9835-11e5-80cf-e912fd50923f.png)

```r
# Clear graphics and data
graphics.off()
rm(list = ls())

# Load Packages
library(fGarch)

# Left Skewed
r = rsnorm(n = 1e+05, xi = 2)

# Plot the distribution
hist(r, n = 100, probability = TRUE, border = "white", col = "red", main = "Left Skewed Dist.")
box()

# Compute the density
d = density(r)
lines(d, lwd = 2, col = "blue")

# Right Skewed distribution 
rr = rsnorm(n = 1e+05, xi = -2)

# Plot the given distribution and correspondent Histogram
hist(rr, n = 100, probability = TRUE, border = "white", col = "green", 
     main = "Right Skewed Dist.")
box()

# Compute the density
dr = density(rr)
lines(dr, lwd = 2)

```




`


