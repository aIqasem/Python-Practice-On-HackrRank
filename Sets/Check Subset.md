# Check Subset

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-check-subset/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
T = int(input())

list_of_sets = []

for i in range(T):
    len_a = int(input())
    set_a = set(list(map(int,input().split())))
    len_b = int(input())
    set_b = set(list(map(int,input().split())))
    list_of_sets.append((set_a,set_b))

for i in list_of_sets:
    if i[0].intersection(i[1]) == i[0]:
        print("True")
    else:
        print("False")
```