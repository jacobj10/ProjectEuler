##Multiples of 3 and 5
Problem 1
If we list all the natural numbers below 10 that are multiples of 3 or 5, we get 3, 5, 6 and 9. The sum of these multiples is 23.
Find the sum of all the multiples of 3 or 5 below 1000.

#Solution
```c++
#include <iostream>

using namespace std;

int main()
{
   int x=3;
   int sum=0;
   while(x<1000)
   {
     sum=sum+x;
     x=x+3;
   }
   x=5;
   while(x<1000)
   {
        if (x%3!=0)
        {
            sum=sum+x;     
        }
       x=x+5;
       
   }
   cout<< sum<<endl;
}
```
Answer: 	233168
