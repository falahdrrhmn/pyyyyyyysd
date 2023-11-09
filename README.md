# python 


## Recursion

```py
# Recursion 
# example 
# 5! = 5 * 4 * 3 * 2 * 1

def recursion(nilai):
    if nilai == 0 or nilai == 1:
        return 1
    else:
        return nilai * recursion(nilai - 1)
   
print(recursion(5))
```
