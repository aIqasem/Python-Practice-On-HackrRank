# Alphabet Rangoli

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/alphabet-rangoli/problem?isFullScreen=true)

<br>
<br>

> ***Solution***
> 

```python
def print_rangoli(size):
    def add_to_str(s, add):
        return f"{add}-{s}-{add}"
    
    l = "a b c d e f g h i j k l m n o p q r s t u v w x y z"
    l_alpha = l.split()
    
    def middle_rangoli(size,index):
        p = l_alpha[index]
        for i in range(size-1):
            p = add_to_str(p, l_alpha[index+i+1])
        return p
    
    s = middle_rangoli(size,0)
    width = ((size-1)*4+1)
    for i in range(1, size):
        s = middle_rangoli(size-i,i).center(width,"-") + "\n" + s + "\n" + middle_rangoli(size-i,i).center(width,"-")
    print(s)
    
if __name__ == '__main__':
    n = int(input())
    print_rangoli(n)
```

- This one took me about 2 hours to solve. So dumb.