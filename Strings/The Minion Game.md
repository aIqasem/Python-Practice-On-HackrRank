# The Minion Game

<br>

- Python level: Python (Basic)
- Level: Meduim
- [link on HackerRank](https://www.hackerrank.com/challenges/the-minion-game/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def minion_game(s):
    vowels = ["A","E","I","O","U"]
    count_vowels_based = 0
    count_constant_based = 0
    
    for i in range(len(s)):
        if s[i] in vowels:
            count_vowels_based += len(s) - i
        else:
            count_constant_based += len(s) - i
    
    if count_constant_based > count_vowels_based:
        print(f"Stuart {count_constant_based}")
    elif count_vowels_based > count_constant_based:
        print(f"Kevin {count_vowels_based}")
    else:
        print("Draw")
```