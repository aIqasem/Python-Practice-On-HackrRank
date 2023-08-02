# Check Strict Superset

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-check-strict-superset/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
set_a = set(input().split())
number_of_other_sets = int(input())
print(all(set_a > set(input().split()) for i in range(number_of_other_sets)))
```