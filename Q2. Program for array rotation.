#include<iostream>
using namespace std;

int main()
{
	int n, d; 
	cin>>n>>d;
	if(d > n)
	{
		d = d%n;
	}
	int a[n], ans[n];
	for(int i = 0; i < n; i++)
	{
		cin>>a[i];
		ans[(i-d+n)%n] = a[i];
	}
	
	for(int i = 0; i < n; i++)
	{
		cout<<ans[i]<<" ";
	}
	
}
