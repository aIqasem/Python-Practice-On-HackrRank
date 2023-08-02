# Find a string

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/find-a-string/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def count_substring(string, sub_string):
    count = 0
    for i in range(len(string)):
        if string[i] == sub_string[0]:
            if string[i:i+len(sub_string)] == sub_string:
                count += 1
    return count

if __name__ == '__main__':
    string = input().strip()
    sub_string = input().strip()
    
    count = count_substring(string, sub_string)
    print(count)
```