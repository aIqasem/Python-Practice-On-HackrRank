# Set Mutations

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-set-mutations/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
len_a = int(input())
set_a = set(list(map(int,input().split())))

number_of_other_sets = int(input())

l_ops = []
l_sets = []

for i in range(number_of_other_sets):

    op,len_set = input().split()
    set_ = set(list(map(int,input().split())))

    l_ops.append(op)
    l_sets.append(set_)

for i in range(len(l_ops)):

    if l_ops[i] == "intersection_update":
        set_a.intersection_update(l_sets[i])

    elif l_ops[i] == "update":
        set_a.update(l_sets[i])

    elif l_ops[i] == "symmetric_difference_update":
        set_a.symmetric_difference_update(l_sets[i])

    elif l_ops[i] == "difference_update":
        set_a.difference_update(l_sets[i])

print(sum(set_a))
```