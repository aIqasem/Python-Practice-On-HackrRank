# Write a function

<br>

- Python level: Python (Basic)
- Level: Meduim
- [link on HackerRank](https://www.hackerrank.com/challenges/write-a-function/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def is_leap(year):
    leap = False
    if year % 4 == 0:
        leap = True
        if year % 100 == 0:
            leap = False
            if year % 400 == 0:
                leap = True
            
    
    return leap

year = int(input())
print(is_leap(year))
```