# Symmetric Difference

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/symmetric-difference/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
M = int(input())
Ms = set(map(int,input().split()))

N = int(input())
Ns = set(map(int,input().split()))

list_of_differences = []

for i in Ms:
    if i not in Ns:
        list_of_differences.append(i)

for i in Ns:
    if i not in Ms:
        list_of_differences.append(i)

for i in sorted(list_of_differences):
    print(i)
```