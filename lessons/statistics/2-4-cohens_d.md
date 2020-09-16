[Think Stats Chapter 2 Exercise 4](http://greenteapress.com/thinkstats2/html/thinkstats2003.html#toc24) (Cohen's d)

**Mean of the weight of firsts and others**  
```python
[firsts['totalwgt_lb'].mean(),others['totalwgt_lb'].mean()]
```
```python
[7.201094430437772, 7.325855614973262]
```

___
**Cohen's d**
```python
import math
diff = firsts['totalwgt_lb'].mean() - others['totalwgt_lb'].mean()

var1 =firsts['totalwgt_lb'].var()
var2 = others['totalwgt_lb'].var()
n1, n2 = len(firsts), len(others)
pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
d = diff / math.sqrt(pooled_var)
```
```python
-0.08867292707260174
```
___
**On average it seems as though while the first pregancy is slightly longer than the others the first baby is slightly lighter than others.**
