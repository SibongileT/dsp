[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

**Find percentage of people between 5'10 and 6'1'**
```python
five_ten_cdf = dist.cdf(177.8)
six_one_cdf = dist.cdf(185.4)
percent = six_one_cdf - five_ten_cdf
```
Around 34% of men are in this height range.
