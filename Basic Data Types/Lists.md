# Lists

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/python-lists/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
if __name__ == '__main__':
    N = int(input())
    operations = []
    l = []
    
    for i in range(N):
        x = input().split()
        operations.append(x)
    
    for i in range(len(operations)):
        if operations[i][0] == 'insert':
            x = int(operations[i][1])
            y = int(operations[i][2])
            l.insert(x,y)
        elif operations[i][0] == 'print':
            print(l)
        elif operations[i][0] == 'remove':
            l.remove(int(operations[i][1]))
        elif operations[i][0] == 'append':
            l.append(int(operations[i][1]))
        elif operations[i][0] == 'sort':
            l.sort()
        elif operations[i][0] == 'pop':
            l.pop()
        elif operations[i][0] == 'reverse':
            l.reverse()
```

- This problem is so dumb and boring .. the wording of the problem is so dumb .. take a quick look and feel free to skip if you know the basic operations of python lists.