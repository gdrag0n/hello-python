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

## Ways to sort

1. sort by keys
```sorted_dic = sorted(dic.items())```

2. sort by values
```
sorted_dic = sorted(dic.items(), key=lambda x:x[1])
#here, x[1] refers to the values
```

Note:
- For key-based sort, why not simply use ```sorted(dic)```?:
    it does not return the entire dictionary, but only a list of sorted keys
    
- lambda reduces speed of execution
