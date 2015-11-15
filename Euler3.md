#Largest prime factor
Problem 3
The prime factors of 13195 are 5, 7, 13 and 29.

What is the largest prime factor of the number 600851475143 ?

#Solution
```c++
#include<iostream>
#include<string>

using namespace std;

int main()
{
	int a;
	a = 3;
	int num;
	num = 2;
	while (a < 600851475143/2)
	{
		if (600851475143 % a == 0)
		{
			while (a%num != 0)
			{
				num++;
				
			}
			if (a == num)
			{
				cout << a << endl;
			}
			
		}
		a++;
		num = 2;
	}
	
}
```
Answer: 6857
*Disclaimer: I did this problem a while ago so this is definately not the OPTIMAL solution*
