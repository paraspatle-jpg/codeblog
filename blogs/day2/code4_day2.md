**CodeBlog**

Day : 2

Problem solved : 4/4

Problem 4 : **# Greedy puppy**

[Problem Statement](https://www.codechef.com/problems/GDOG)

Approach :

Topics: Vector,sorting

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>         int t;
>         cin>>t;
>         while(t--){
>             int n , k;
>             cin>>n>>k;
>             int max=0;
>             for(int i = 2; i<=k ; i++){
>                 if(n%i > max)
>                 {
>                     max = n%i;
>                 }
>             }
>             cout<<max<<endl;
>
>         }
>     	return 0;
>     }

Time taken : 7 min
