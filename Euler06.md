#Sum square difference
Problem 6
The sum of the squares of the first ten natural numbers is,

12 + 22 + ... + 102 = 385
The square of the sum of the first ten natural numbers is,

(1 + 2 + ... + 10)2 = 552 = 3025
Hence the difference between the sum of the squares of the first ten natural numbers and the square of the sum is 3025 − 385 = 2640.

Find the difference between the sum of the squares of the first one hundred natural numbers and the square of the sum.

#Solution
```c++
#include<iostream>
#include<string>
using namespace std;

int main()
{
	int a;
	int b;
	a = 1;
	b = 2;
	int c;
	c = 1;
	int limit;
	limit = 100;
	while (b <= limit)
	{
		a = b * b;
		c = a + c;
		
		
		b++;
	}
	int d;
	int e;
	d = 2;
	e = 1;
	while (d <= limit)
	{
		e = d + e;
		d++;
	}
	cout <<(e*e-c) << endl;
	return 0;
}
```
Answer: 25164150
