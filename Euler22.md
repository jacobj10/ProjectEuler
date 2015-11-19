#Names scores
Problem 22
Using names.txt (right click and 'Save Link/Target As...'), a 46K text file containing over five-thousand first names, begin by sorting it into alphabetical order. Then working out the alphabetical value for each name, multiply this value by its alphabetical position in the list to obtain a name score.

For example, when the list is sorted into alphabetical order, COLIN, which is worth 3 + 15 + 12 + 9 + 14 = 53, is the 938th name in the list. So, COLIN would obtain a score of 938 × 53 = 49714.

What is the total of all the name scores in the file?

#Solution
```python
from string import ascii_uppercase as v
file=open("names.txt","r") 
with open("names.txt","r") as f:
    x=f.readline()
a=0
b=1
counter=1
z=list()
while(a<len(x)):
    if x[a]==",":
        z.append(x[b:a-1])
        b=a+2
    elif a==len(x)-1:
        z.append(x[b:len(x)-1])
    a+=1
a=0
b=0
z.sort()
total=0
total2=0
while(a<len(z)):
    while(b<len(z[a])):
       total=v.index(z[a][b])+1+total
       b+=1
    total2=total*counter+total2
    counter+=1
    total=0
    b=0
    a+=1
print total2

```
Answer:871198282
