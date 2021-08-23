**CodeBlog**

Day : 3

Problem solved : 3/4

Problem 3 : **# Simple Statistics**

[Problem Statement](https://www.codechef.com/problems/SIMPSTAT)

Approach :

Topics:Sorting

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
>     int n,k;
>
>     cin>>n>>k;
>
>     double arr[n];
>
>     double sum=0;
>
>     for (int i =0 ; i<n ; i++)
>
>     {
>
>     cin>>arr[i];
>
>     sum = sum + arr[i];
>
>     }
>
>     sort(arr , arr+n);
>
>     for(int i=0;i<k ; i++)
>
>     {
>
>     sum = sum - arr[i];
>
>     sum = sum - arr[n-1 - i];
>
>     }
>
>     double mean=(sum)/(n-(2*k));
>
>     cout<<fixed<<setprecision(6)<<mean<<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 15 min
