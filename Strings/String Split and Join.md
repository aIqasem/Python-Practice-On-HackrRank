# String Split and Join

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/python-string-split-and-join/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def split_and_join(line):
    return "-".join(line.split())

if __name__ == '__main__':
    line = input()
    result = split_and_join(line)
    print(result)
```