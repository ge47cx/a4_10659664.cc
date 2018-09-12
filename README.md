#include <iostream>
#include <math.h>
using namespace std;

int GCD(int a, int b)
{
	int rem= a%b;
	while(rem!=0)
{
	a=b;
	b=rem;
	rem=a%b;	
	}
	return b;
}
int main()
{
	int a,b;
	cout<<"Enter the first the number"<<endl;
	cin>>a;
	cout<<"Enter the second the number"<<endl;
	cin>>b;
	cout<< "The GCD of the numbers is" << GCD(a,b);
	
	return 0;
	
	
	
	
	
}
