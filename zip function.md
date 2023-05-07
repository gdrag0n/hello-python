# 

# 2d Array
each element of zipped entity corresponds to each column of the 2d array
```
        for g in zip(*grid):  # g is a list/tuple of column elements
            m+=max(g)         # maximum element in g, i.e. maximum value in that column
        return m
```
