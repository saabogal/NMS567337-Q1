# Clear graphics and data
graphics.off()
rm(list = ls())

# Name of QuantLet : NMS567337-Q9A

# Published in : Null

# Description : transformation of a random variable with a given mean
# and variance to an Asymptotic normal distribution with mean zero and
# variance 1.

# Keywords : 'Asymptotic Normal Distribution, Graphical Representation,
# Random Variables, pdf'

# Author : Luis Alejandro Sarmiento Abogado

# Submitted : Tue, December 02 2015 by Luis Alejandro Sarmiento Abogado

# Datafile : Null

# Generate a set of random variables.
random <- rnorm(n = 1e+05, mean = 2, sd = 0.5)

# determine their correspondent mean and variance
mu = mean(random)
sd = sd(random)

# Set the transformation function.
Y = function(mu, sd, random) {
  (random - mu)/sd
}
X = (random - mu)/sd

# Determine the mean and variance of our transformation
mean(X)
var(X)

# Plot the results graphically to prove that X is asymptotically normal
# distributed

plot(density(random), col = "red", xlim = c(-3, 4), ylim = c(0, .8), lwd = 2, 
     main = "Densities comparison")
lines(density(X), col = "blue", lwd = 2)
legend("topleft", legend = c("Transformation", "r.v"), lty = 1, col = c("blue", 
                                                                        "red"), cex = 0.9)
