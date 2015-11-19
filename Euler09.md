#Special Pythagorean triplet
Problem 9
A Pythagorean triplet is a set of three natural numbers, a < b < c, for which,

a2 + b2 = c2
For example, 32 + 42 = 9 + 16 = 25 = 52.

There exists exactly one Pythagorean triplet for which a + b + c = 1000.
Find the product abc.

#Solution
```c++
#include<iostream>
#include<cmath>
using namespace std;

int main()
{
	int a;
	int b;
	int c;
	a = 1;
	b = 2;
	c = 3;
	
	while (22!=12)
	{
		c = a*a + b*b;
		if (a + b + sqrt(c) ==1000)
		{
			cout << a*b*sqrt(c) << endl;
			return 0;
		}
		
		if (b == 1000)
		{
			a++;
			b = a + 1;
		}
		else
		{
			b++;
		}
		
	}
	
}
```
Answer: 3.1875e+07
