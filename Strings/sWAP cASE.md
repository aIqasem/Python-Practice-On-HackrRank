# sWAP cASE

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/swap-case/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def swap_case(s):
    swapped_s = ""
    for i in s:
        if i.islower():
            swapped_s += str.upper(i)
        else:
            swapped_s += str.lower(i)
    return swapped_s

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```