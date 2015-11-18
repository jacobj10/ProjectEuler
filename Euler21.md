#Amicable numbers
Problem 21
Let d(n) be defined as the sum of proper divisors of n (numbers less than n which divide evenly into n).
If d(a) = b and d(b) = a, where a ≠ b, then a and b are an amicable pair and each of a and b are called amicable numbers.

For example, the proper divisors of 220 are 1, 2, 4, 5, 10, 11, 20, 22, 44, 55 and 110; therefore d(220) = 284. The proper divisors of 284 are 1, 2, 4, 71 and 142; so d(284) = 220.

Evaluate the sum of all the amicable numbers under 10000.

#Solution
```python
from math import*
a=1
b=0
div=1
list1=list()
list2=list()
total=0
if (1==1):
   while(a<10000):
        while(div<a):
            if a%div==0:
                total=div+total     
            div+=1
        list1.append(a)
        list2.append(total)
        a+=1
        total=0
        div=1
a=0
b=0
total=0
print len(list1)
print len(list2)
while(a<len(list1)):
    while(b<len(list2)):
        if list1[a]==list2[b] and list1[b]==list2[a] and a!=b:
            total=list1[a]+total
        b+=1
    b=0
    a+=1    
print total
```
Answer:31626
