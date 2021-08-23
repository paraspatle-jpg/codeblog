**CodeBlog**

Day : 3

Problem solved : 2/4

Problem 2 : **#Lazy Jem**

[Problem Statement](https://www.codechef.com/problems/TALAZY)

Approach :

Topics:

> Code:
>
>     #include <bits/stdc++.h>
>
>     using namespace std;
>
>
>
>     int main() {
>
>     int t;
>
>     cin>>t;
>
>     while(t--)
>
>     {
>
>     long long int n,b,m;
>
>     cin>>n>>b>>m;
>
>     long long int sum=0;
>
>     while(n!=1)
>
>     {
>
>     if(n%2 == 0)
>
>     {
>
>     sum = sum + ((n*m)/2) + b;
>
>     n= n-(n/2);
>
>     m=m*2;
>
>     }
>
>     else
>
>     {
>
>     sum = sum + ((n+1)*m/2) + b;
>
>     n= n-((n+1)/2);
>
>     m=m*2;
>
>     }
>
>     }
>
>     sum = sum + m;
>
>     cout<<sum<<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 10 min
