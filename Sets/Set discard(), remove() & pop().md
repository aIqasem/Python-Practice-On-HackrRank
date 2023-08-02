# Set .discard(), .remove() & .pop()

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-set-discard-remove-pop/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
n = int(input())
ns = set(list(map(int,input().split())))

N = int(input())
l_commands = []
for i in range(N):
    l_commands.append(input().split())

for i in l_commands:
    if i[0] == "pop":
        ns.pop()
    elif i[0] == "remove":
        ns.remove(int(i[1]))
    elif i[0] == "discard":
        ns.discard(int(i[1]))

print(sum(ns))
```