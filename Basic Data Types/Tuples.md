# Tuples

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/python-tuples/problem?isFullScreen=true)

<br>
<br>

> ***Solution ( not really )***
> 

```python
import builtins

n = int(input())
t = tuple(map(int,input().split()))
print(hash(t))
```

- This should work properly .. but it gets an error .. idk why.

> ***Important note***
> 
- seems like the output of `hash()` function in correct when using **Pypy 3** .. not **python 3** .. idk why .. but use **Pypy 3** and have a nice looking Congratulations! popup

```python
n = int(input())
print(hash(tuple(map(int,input().split()))))
```