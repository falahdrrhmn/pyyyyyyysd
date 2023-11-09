# python 

```py
# Recursion 
# example 
# 5! = 5 * 4 * 3 * 2 * 1

def faktorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * faktorial(n - 1)
   
print(faktorial(5))
```
