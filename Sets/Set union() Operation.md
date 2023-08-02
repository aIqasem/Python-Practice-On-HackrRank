# Set .union() Operation

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-set-union/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
n_eng = int(input())
n_roll_numbers = set(list(map(str,input().split())))

n_fren = int(input())
fren_roll_numbers = set(list(map(str,input().split())))

all = n_roll_numbers.union(fren_roll_numbers)
print(len((all)))
```