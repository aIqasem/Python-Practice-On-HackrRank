# Capitalize!

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/capitalize/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def solve(s):
    l = s.split(" ")
    print(l)
    for i in range(len(l)):
        if len(l[i]) >= 1:
            l[i] = str.upper(l[i][0]) + l[i][1:]
        else:
            continue
    return " ".join(l)
```