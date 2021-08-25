**CodeBlog**

Day : 5

Problem solved : 1/4

Problem : **#Average Number**

[Problem Statement](https://www.codechef.com/problems/AVG)

Approach :

Topics: Basic C++

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
>     while(t--){
>
>     int n,k,v;
>
>     cin>>n>>k>>v;
>
>     int arr[n];
>
>     int sum1=0;
>
>     int sum = v*(n+k);
>
>     for(int i = 0 ; i<n  ;  i++){
>
>     cin>>arr[i];
>
>     sum1+=arr[i];
>
>     }
>
>     int rem = (sum - sum1)%k;
>
>     if(rem != 0|| sum - sum1<=0) cout<<"-1"<<endl;
>
>     else  cout<<  (sum  -  sum1)/k  <<endl;
>
>     }
>
>     return 0;
>
>     }

Time taken : 10 min
