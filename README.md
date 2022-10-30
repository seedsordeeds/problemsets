# Problem sets!

# [Easy] Problem 1: Find the distance!

The challenge is to write a function that computes the distance between two points A and B with coordinates (x1, y1) and (x2, y2) respectively.

To test, use the following values:

```
* x1 = 4 ; y1 = 0
* x2 = 6 ; y2 = 6
```

The program should return ```6.324555320336759```.

# [Intermediate/Hard] Problem 2: N-Divisible Digits

The task is to write a program that takes two integers, N and M, and then to find the largest integer composed of N-digits that is evenly divisible by M. 

The following statements are always true:

* N will always be 1 or greater and ranges from 1 to 9.
* M will always be 2 or greater and ranges from 2 to 999,999,999.

Please note that some combinations of N and M will not have a solution.

To test, use the following values:

```
* N = 3 ; M = 2
* N = 5 ; M = 12372
```
The program should return ```998``` and ```98976```.

# Solution 1: 

```
def dist(x1, x2, y1, y2):
	distance = (((x1-x2)**2)+((y1-y2)**2))**(1/2)
	return distance
```

OR

```
import math

def distance(x1, x2, y1, y2):
	distance = math.sqrt(((x1-x2)**2)+((y1-y2)**2))
	return distance
```

# Solution 2: 

```
def ndiv(n,m):
    x=(10**n-1)
    return x - x % m
```

OR 

```
N = int(input("Enter number of digits of numerator: "))
M = int(input("Enter denominator: "))
X = 10**N-1
print(X-X%M)
```


