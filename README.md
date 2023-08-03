# README.md

## Erfinv Project `erfinv`

Implementation by [lakshayg](https://github.com/lakshayg) of the inverse error 
function 'erfinv' based on the rational approximation of percentage points of 
normal distribution available from https://www.jstor.org/stable/2347330.

```
                1           /  x + 1  \
erfinv(x) = --------- ppnd |  -------  |
             sqrt(2)        \    2    /
```

The code has been tested on an x86_64 machine with Intel Core i7, the
tests provided in this repository might not pass for different hardware
configuration due to difference in floating point operations.

Note: golang's math library uses the same implementation for erfinv
[here](https://github.com/golang/go/blob/master/src/math/erfinv.go)
