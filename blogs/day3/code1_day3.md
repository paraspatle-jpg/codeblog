**CodeBlog**

Day : 3

Problem solved : 1/4

Problem 1 : **# That Is My Score!**

[Problem Statement](https://www.codechef.com/problems/WATSCORE)

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
>     int n;
>
>     cin>>n;
>
>     int p , s , arr[8]={0};
>
>     for (int i =0 ; i<n  ;  i++)
>
>     {
>
>     cin>>p>>s;
>
>     if(p>8)
>
>     {
>
>     continue;
>
>     }
>
>     if(arr[p-1]<s)
>
>     {
>
>     arr[p-1]=s;
>
>     }
>
>     }
>
>     int sum=0;
>
>     for (int i =0 ; i<8 ; i++)
>
>     {
>
>     sum += arr[i];
>
>     }
>
>     cout<<sum<<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 20 min
