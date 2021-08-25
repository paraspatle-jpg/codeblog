**CodeBlog**

Day : 5

Problem solved : 2/4

Problem : **# Chef and Steps**

[Problem Statement](https://www.codechef.com/problems/CHEFSTEP)

Approach :

Topics: Basic C++ , String

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
>     int n,step;
>
>     cin>>n>>step;
>
>     string res;
>
>     int arr[n];
>
>     for (int i=0 ; i<n ; i++){
>
>     cin>>arr[i];
>
>     if(arr[i]%step == 0)res.append(1,'1');
>
>     else res.append(1,'0');
>
>     }
>
>     cout<<res<<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 10 min
