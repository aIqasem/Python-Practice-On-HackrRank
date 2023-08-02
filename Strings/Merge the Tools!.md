# Merge the Tools!

<br>

- Python level: Python (Basic)
- Level: Meduim
- [link on HackerRank](https://www.hackerrank.com/challenges/merge-the-tools/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def merge_the_tools(string, k):
    # Creating substrings
    l_substrings = []
    i = 0
    while i<len(string):
        l_substrings.append(string[i:i+k])
        i = i + k

    # storing each substring chars in a dic
    final_l_subtrings = []
    for i in range(len(l_substrings)):
        d ={}
        for ii in range(len(l_substrings[i])):
            d[l_substrings[i][ii]] = 0
        final_l_subtrings.append("".join(list(d.keys())))

    for i in final_l_subtrings:
        print(i)
```