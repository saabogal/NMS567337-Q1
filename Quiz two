graphics.off()
rm(list = ls())

# Quiz two : Plot the above figure with asymmetric normal distribution

# Load fGarch package
library(fGarch)

# 1.0 Left Skewed
r = rsnorm(n = 1e+05, xi = 2)

# Plot the distribution
hist(r, n = 100, probability = TRUE, border = "white", col = "red", main = "Left Skewed Dist.")
box()

# Compute the density
d = density(r)
lines(d, lwd = 2, col = "blue")

# 2.0 Right Skewed distribution 
rr = rsnorm(n = 1e+05, xi = -2)

# Plot the given distribution and correspondent Histogram
hist(rr, n = 100, probability = TRUE, border = "white", col = "green", 
     main = "Right Skewed Dist.")
box()

# Compute the density
dr = density(rr)
lines(dr, lwd = 2)
