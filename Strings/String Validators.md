# String Validators

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/string-validators/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
if __name__ == '__main__':
    s = input()

contains_alphanumeric = False
contains_alphabetical = False
contains_digits = False
contains_lowercase = False
contains_uppercase = False

for i in s:
    if i.isalnum():
        contains_alphanumeric = True
    if i.isalpha():
        contains_alphabetical = True
    if i.isdigit():
        contains_digits = True
    if i.islower():
        contains_lowercase = True
    if i.isupper():
        contains_uppercase = True

print(contains_alphanumeric)
print(contains_alphabetical)
print(contains_digits)
print(contains_lowercase)
print(contains_uppercase)
```