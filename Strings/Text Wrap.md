# Text Wrap

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/text-wrap/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
import textwrap

def wrap(string, max_width):
    s = ""
    for i in range(len(string)):
        if i == 0:
            s += string[i]
        else:
            if (i) % (max_width) == 0:
                s += "\n" + string[i]
            else:
                s += string[i]
    return s

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)
```