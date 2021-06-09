---
layout: single
date: 2021-04-02
title: "두번째 포스팅"
---

# 두번째 포스팅입니다

```python
n = int(input())
num = int(input())
```

    3
    9



```python
def is_in_arr(arr, w):
    for i in arr:
        if i[2] == w:
            return True
    return False
```

2 1 4 3 5 6 2 7 2


```python
arr = []
who = input().split()
```

    2 1 4 3 5 6 2 7 2



```python
arr = []
```


```python
for idx, w in enumerate(who):
    if is_in_arr(arr,w):
        for index, var in enumerate(arr):
            if var[2] == w:
                arr[index][0]+=1
                print(arr)
                break
    else:
        if len(arr) < n:
            arr.append([1, idx, w])
        else:
            arr[0] = [1, idx, w]
    print(arr)
    arr.sort(key=lambda x: (x[0], x[1]))
    print(arr, '\n')
arr.sort(key=lambda x:int(x[2]))
for i in range(n):
    if i == n-1:
        print(arr[i][2])
    else:
        print(arr[i][2], end=' ')
```

    [[1, 0, '2']]
    [[1, 0, '2']] 
    
    [[1, 0, '2'], [1, 1, '1']]
    [[1, 0, '2'], [1, 1, '1']] 
    
    [[1, 0, '2'], [1, 1, '1'], [1, 2, '4']]
    [[1, 0, '2'], [1, 1, '1'], [1, 2, '4']] 
    
    [[1, 3, '3'], [1, 1, '1'], [1, 2, '4']]
    [[1, 1, '1'], [1, 2, '4'], [1, 3, '3']] 
    
    [[1, 4, '5'], [1, 2, '4'], [1, 3, '3']]
    [[1, 2, '4'], [1, 3, '3'], [1, 4, '5']] 
    
    [[1, 5, '6'], [1, 3, '3'], [1, 4, '5']]
    [[1, 3, '3'], [1, 4, '5'], [1, 5, '6']] 
    
    [[1, 6, '2'], [1, 4, '5'], [1, 5, '6']]
    [[1, 4, '5'], [1, 5, '6'], [1, 6, '2']] 
    
    [[1, 7, '7'], [1, 5, '6'], [1, 6, '2']]
    [[1, 5, '6'], [1, 6, '2'], [1, 7, '7']] 
    
    [[1, 5, '6'], [2, 6, '2'], [1, 7, '7']]
    [[1, 5, '6'], [2, 6, '2'], [1, 7, '7']]
    [[1, 5, '6'], [1, 7, '7'], [2, 6, '2']] 
    
    2 6 7



```python
arr
```




    [[2, 6, '2'], [1, 5, '6'], [1, 7, '7']]




```python
pp = []
```


```python
pp[0][0]+=1
```


```python
arr
```




    [[2, 6, '2'], [1, 5, '6'], [1, 7, '7']]




```python

```
