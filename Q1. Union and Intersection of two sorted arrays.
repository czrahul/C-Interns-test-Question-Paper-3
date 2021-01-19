#include<iostream>
#include<unordered_set>
#include<vector>
using namespace std;

void union_intersection(int a[], int b[], int n, int m)
{
	vector<int> intrs_arr;
	unordered_set<int> s;
	for(int i = 0; i < n; i++)
	{
		s.insert(a[i]);
	}
	for(int i = 0; i < m; i++)
	{
		if(s.find(b[i]) != s.end())
		{
			intrs_arr.push_back(b[i]);
		}
		else
			s.insert(b[i]);
	}
	cout<<"Union : {";
	for(auto i = s.begin(); i != s.end(); i++)
	{
		cout<<*i<<", ";
	}
	cout<<"}"<<"\n";
	cout<<"Intersection : {";
	for(int i = 0; i < intrs_arr.size(); i++)
	{
		cout<<intrs_arr[i]<<", ";
	}
	cout<<"}"<<"\n";
}
int main()
{
	int n, m;
	cin>>n>>m;
	int a[n], b[m];
	for(int i = 0; i < n; i++)
	{
		cin>>a[i];
	}
	
	for(int i = 0; i < m; i++)
	{
		cin>>b[i];
	}
	if(n>=m)
		union_intersection(a, b, n, m);
	else
		union_intersection(b, a, m, n);
	return 0;
	
} 
