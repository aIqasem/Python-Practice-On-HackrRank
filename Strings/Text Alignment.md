# Text Alignment

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/text-alignment/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
thickness = int(input())
char = "H"

# Top
l = []
index = 0
for i in range(1,(thickness)*2,2):
    l.append((char*i).center(1+(thickness-1)*2," "))
    print(l[index])
    index += 1

# Middle
line = " "*(thickness//2) + char*thickness + " "*(thickness*3) + char*thickness + " "*((thickness*3)-(thickness//2))
for i in range(thickness+1):
    print(line)

for i in range( thickness//2 + 1 ):
    print(" "*(thickness//2) + char*(thickness*5))

for i in range(thickness+1):
    print(line)

# Bottom
for i in range(thickness):
    print(" "*(thickness * 4) + l[thickness-1 - i])
```

- I could have explained that code .. just used a pen and a paper to figure out a formula for each part of the logo .. this code can be more clean .. but not today