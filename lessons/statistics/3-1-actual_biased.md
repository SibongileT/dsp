[Think Stats Chapter 3 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2004.html#toc31) (actual vs. biased)

```python
import nsfg
resp = nsfg.ReadFemResp()
no_of_children = resp['numkdhh']
```
**Compute the PMF**
```python
pmf = thinkstats2.Pmf(no_of_children,label='actual')
```
**Compute the biased distribution.**
```python
biased_pmf = BiasPmf(pmf,label='observed')
```
**Plot the actual and biased distribution**
```python
thinkplot.PrePlot(2)
thinkplot.Pmfs([pmf, biased_pmf])
thinkplot.Show(xlabel='Number of children', ylabel='PMF')
```
**PMF Mean**
```python
pmf.Mean()
```
1.024205155043831

**Biased Mean**
```python
biased_pmf.Mean()
```
2.403679100664282
