#10001st prime
Problem 7
By listing the first six prime numbers: 2, 3, 5, 7, 11, and 13, we can see that the 6th prime is 13.

What is the 10 001st prime number?

#Solution
```c++
#include <string> 
#include <iostream> 

using namespace std;

int main()
{
	int a;
	int b;
	a = 2;
	b = 2;
	int c;
	int counter=0;
	c = 1;
	while (c <= 10001)
	{
		while (a%b != 0)
		{
			b++;

		}
		if (a == b)
		{
			counter=a;
			c++;
		}
		a++;
		b = 2;
    

	}
cout<<counter<<endl;	
}
```
Answer: 104743
