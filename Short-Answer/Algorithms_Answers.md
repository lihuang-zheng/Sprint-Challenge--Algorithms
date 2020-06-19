#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n)
```python
a = 0                      // log(1)
    while (a < n * n * n): // log(n)
        a = a + n * n      // log(n)
```


b) O(n log n)
```
sum = 0                // log(1)
    for i in range(n): // log(n)
        j = 1          // log(1)     
        
        while j < n:   // log(n)
            j *= 2     // log(log n) 
            sum += 1   // log(n)
```


c) O(n)
```
def bunnyEars(bunnies):
    if bunnies == 0:
        return 0 
    
    return 2 + bunnyEars(bunnies-1) // log (n)
```

## Exercise II
By using O(log n), we begin in the middle of the floors (range of n) while drop an egg & if egg breaks,
we go down a floor.
By skipping the floors that above and below that breaking the egg.

```
for f in range(0, len(n) // 2):
    if egg_breaks(f):
        return f
```



