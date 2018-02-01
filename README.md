
ggplot2 <img src="man/figures/logo.png" align="right" />
========================================================
![ggplot](http://hexb.in/hexagons/ggplot2.png)
Overview
--------

ggplot2 is a system for declaratively creating graphics, based on . You provide the data, tell ggplot2 how to map variables to aesthetics, what graphical primitives to use, and it takes care of the details.

Installation
------------

``` r

# can easily be installed by
install.packages("ggplot2")

# Or the the development version from GitHub:
# install.packages("devtools")
devtools::install_github("tidyverse/ggplot2")
```

Usage
-----
the grammer of graphics can be quit intimidating by its looks but is worth it

even the advanced graph can be done by just adding few layer of  grammer
```{r}
p <- ggplot(df[df$carat < 3, ], aes(x = carat, y = price, colour = clarity))
# loading data and adding the layers over it
print(p + geom_point(alpha = 0.1) + geom_smooth() + )
```
![](https://raw.githubusercontent.com/Rupii/ggplot2/master/Rplot.png)
