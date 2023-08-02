# No Idea!

<br>

- Python level: Python (Basic)
- Level: Meduim
- [link on HackerRank](https://www.hackerrank.com/challenges/no-idea/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
n, m = map(int,input().split())
l_n = map(int,input().split())
l_m_a = map(int,input().split())
l_m_b = map(int,input().split())

set_m_a = set(l_m_a)
set_m_b = set(l_m_b)

h = 0

for i in l_n:
    if i in set_m_a:
        h += 1
    elif i in set_m_b:
        h -= 1
    else:
        continue
print(h)
```