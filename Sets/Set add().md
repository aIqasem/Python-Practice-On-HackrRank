# Set .add()

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-set-add/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
N = int(input())
list_counties = []

for i in range(N):
    list_counties.append(input())

print(len(set(list_counties)))
```