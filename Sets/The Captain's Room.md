# The Captain's Room

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/py-the-captains-room/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
k = int(input())
unordered_rooms = list(map(int, input().split()))

l = sorted(unordered_rooms)

for i in range(1,len(l)):
    if i == len(l)-1:
        captain_room_number = l[i]
        break
    if l[i] != l[i-1] and l[i] != l[i+1]:
        captain_room_number = l[i]
        break

print(captain_room_number)
```