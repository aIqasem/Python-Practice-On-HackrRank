# String Formatting

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/python-string-formatting/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def print_formatted(number):
    length = len(f"{number:b}")
    s = ""
    for i in range(1,number+1):
        if i == number:
            s += f"{i:d}".rjust(length," ") +" "+ f"{i:o}".rjust(length," ") +" "+ f"{i:X}".rjust(length," ") +" "+ f"{i:b}".rjust(length," ")
        else:
            s += f"{i:d}".rjust(length," ") +" "+ f"{i:o}".rjust(length," ") +" "+ f"{i:X}".rjust(length," ") +" "+ f"{i:b}".rjust(length," ") + "\n"
    print(s)
if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
```

- note
    
    `*f”number:x”*` returns a small alphabetical character representing the hexadecimal number ( A : F ).
    
    `*f”number:X”*` returns a capital alphabetical character.