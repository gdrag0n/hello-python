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

## Ways to create from given lists
```
#make sure that
dic = dict(zip(list1, list2))
```

## Ways to sort

1. sort by keys
```
#reverse to be included if sorting in descending order, with reverse=True
sorted_dic = sorted(dic.items(), reverse=True/False)
dic=dict(sorted_dic)
```

2. sort by values
```
sorted_dic = sorted(dic.items(), key=lambda x:x[1])
#here, x[1] refers to the values
```

Note:
- For key-based sort, why not simply use ```sorted(dic)```?:
    it does not return the entire dictionary, but only a list of sorted keys
    
- lambda reduces speed of execution


## Returning keys/values
```
return list(dic.values())
```

## Dictionaries to remove duplicates
```
nums=list(dict.fromkeys(nums))
```
