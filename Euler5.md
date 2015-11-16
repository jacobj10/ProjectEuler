#Smallest multiple
Problem 5
Published on Friday, 30th November 2001, 06:00 pm; Solved by 285475; Difficulty rating: 5%
2520 is the smallest number that can be divided by each of the numbers from 1 to 10 without any remainder.

What is the smallest positive number that is evenly divisible by all of the numbers from 1 to 20?

#Solution
```c++
#include<iostream>
#include<string>
using namespace std;

int main()
{
	int a;
	a = 2521;
	int b;
	b = 1;
	while (b<=20)
	{
		if (a%b == 0)
		{
			b++;
		}
		else
		{
			a++;
			b = 1;
		}
	}
		
	cout << a << endl;
	return 0;
}
```
Answer: 232792560
