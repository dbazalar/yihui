---
title: sim.qqnorm()
subtitle: Simulation of QQ plots for the Normal distribution
date: '2017-04-04'
slug: sim-qqnorm
from_Rmd: yes
---

This demo shows the possible QQ plots created by random numbers generated
from a Normal distribution so that users can get a rough idea about how QQ
plots really look like.

When the sample size is small, it is hard to get a correct inference about
the distribution of data from a QQ plot. Even if the sample size is large,
usually there are outliers far away from the straight line. Therefore, don't
overinterpret the QQ plots.
 

```r
library(animation)
ani.options(interval = 0.1, nmax = 100)
par(mar = c(3, 3, 2, 0.5), mgp = c(1.5, 0.5, 0), tcl = -0.3)

sim.qqnorm(n = 20, last.plot = expression(abline(0, 1)))
```

<video controls loop autoplay><source src="https://assets.yihui.org/figures/animation/example/sim-qqnorm/demo-a.mp4?dl=1" /><p>plot of chunk demo-a</p></video>
