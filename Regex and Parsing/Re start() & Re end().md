# Re.start() & Re.end()

<br>

- Python level: Python (Intermediate)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/re-start-re-end/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
if __name__ == '__main__':
    s = input()
    sub_s = input()

    def substring_starts_ends(string, sub_string):
        their_is_matcing = False
        l = []
        for i in range(len(string)):
            if string[i] == sub_string[0]:
                if string[i:i+len(sub_string)] == sub_string:
                    their_is_matcing = True
                    l.append((i,i+len(sub_string)-1))
        if their_is_matcing:
            return l
        else:
            return [(-1,-1)]

    for i in substring_starts_ends(s,sub_s):
        print(i)
```