# Designer Door Mat

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/designer-door-mat/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
pattern1 = "-"
pattern2 = ".|."
welcome = "WELCOME"

n, m = map(int,input().split())
for i in range(0,n*2,2):
    if i < n-1:
        print((pattern2*(i+1)).center(m,pattern1))
    elif i == n-1:
        print(welcome.center(m,pattern1))
    else:
        print((pattern2*(n*2-(i+1))).center(m,pattern1))
```