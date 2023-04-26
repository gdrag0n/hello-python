## Ways to create

1. with given arrays for keys and values:

```
n=len(A)
dic={}
for i in range(n):
    dic[ A[i] ] = B[i]
```
But we'd like a simpler approach to it than using for loop

```
n=len(A) #=len(b)
dictionary = {A[i]:B[i] for i in range(n)}
```

*The fastest approach:*
```
dictionary = dict(zip(A, B))
```
