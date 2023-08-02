# Nested Lists

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/nested-list/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
if __name__ == '__main__':
    l = []
    for i in range(int(input())):
        name = input()
        score = float(input())
        l.append([name,score])
    
    def l_2nd_lowest(l):
        ***# creating a list of the scores***
        scores = []
        for i in l:
            scores.append(i[1])
        
        ***# getting the 2nd lowest score***
        scores = sorted(scores)
        for i in range(1,len(scores)):
            if scores[i] != scores[i-1]:
                seoned_lowest_score = scores[i]
                break
        
        ***# getting names that got the 2nd lowest score***
        l_2nd_lowest = []
        for i in range(len(l)):
            if l[i][1] == seoned_lowest_score:
                l_2nd_lowest.append(l[i][0])
        return sorted(l_2nd_lowest)
    
    for i in l_2nd_lowest(l):
        print(i)
```