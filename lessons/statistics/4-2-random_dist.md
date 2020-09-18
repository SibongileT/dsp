[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

**Generate the randoms from numpy**
```python
import numpy as np
randoms = np.random.random(1000)
```
---
**Plot the PMF:**  
```python
pmf = thinkstats2.Pmf(randoms)
thinkplot.Pmf(pmf, linewidth=0.1)
thinkplot.Show(xlabel='Random', ylabel='CDF')
```
The lines plotted on the PMF here are all of the same height since they all have the same probability of occurring.
___
**Plot the CDF**
```python
cdf = thinkstats2.Cdf(randoms)
thinkplot.Cdf(cdf)
thinkplot.Show(xlabel='Random', ylabel='CDF')
```
The distribution is uniform because when it is plotted it appears as almost a straight line.
