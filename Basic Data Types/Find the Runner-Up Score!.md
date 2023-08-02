# Find the Runner-Up Score!

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/find-second-maximum-number-in-a-list/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
arr = list(map(int,input("enter values: ").split()))

def runner_up(l):
		# sorting it descending from max to min
    sl = list(reversed(sorted(l)))
		
		# returning the second max element
    for i in range(len(sl)):
        if i == len(sl):
            return -1
        else:
            if sl[i+1] != sl[i]:
                return sl[i+1]
 

print(runner_up(arr))
```

- got the list
- sorted it descending from max to min
- the else clause deals with the duplicated max elements and returns the second max .. for instance .. returns 4 from a list of 1 2 3 5 5 5 4.
    
    ---