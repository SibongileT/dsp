[Think Stats Chapter 4 Exercise 2](http://greenteapress.com/thinkstats2/html/thinkstats2005.html#toc41) (a random distribution)

**Generate the randoms from numpy**
```python
import numpy as np
randoms = np.random.random(1000)
```
---
**Plot the PMF:** When you try and plot the random variable nothing shows up on the plot because all the probabilities are the same.  
```python
pmf = thinkstats2.Pmf(randoms)
thinkplot.hist(pmf)
```
---
**Plot the CDF**
```python
cdf = thinkstats2.Cdf(randoms)
thinkplot.Cdf(cdf)
thinkplot.Show(xlabel='weeks', ylabel='CDF')
```
The distribution is uniform because when it is plotted it appears as almost a straight line  
