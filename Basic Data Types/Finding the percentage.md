# Finding the percentage

<br>

- Python level: Python (Basic)
- Level: Easy
- [link on HackerRank](https://www.hackerrank.com/challenges/finding-the-percentage/problem?isFullScreen=true&h_r=next-challenge&h_v=zen)

<br>
<br>

> ***Solution***
> 

```python
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    
    print(f"{sum(student_marks.get(query_name)) / len(student_marks.get(query_name)):.2f}")
```

- The weird format of the print statement .. is just to print the float number with 2 decimal points .. as the test got a wrong result when displaying just one 0 after the decimal point .. my answer for some test case was 56.0 .. and the Expected Output was 56.00 .. so the test considered my answer is wrong .. that’s why i using formatted string in the print statement.