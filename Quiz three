graphics.off()
rm(list = ls())

# Quiz 3 : Plot Multivariate normal distributions

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


