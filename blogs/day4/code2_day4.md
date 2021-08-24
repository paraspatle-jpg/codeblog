**CodeBlog**

Day : 4

Problem solved : 2/4

Problem : **# Train Partner**

[Problem Statement](https://www.codechef.com/problems/ANKTRAIN)

Approach :

Topics:

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int t;
>     	cin>>t;
>     	while(t--){
>     	    int n;
>     	    cin>>n;
>     	    int res=(n%8);
>     	    if(res == 1)cout<<n+3<<"LB"<<endl;
>     	    if(res == 4)cout<<n-3<<"LB"<<endl;
>     	    if(res == 2)cout<<n+3<<"MB"<<endl;
>     	    if(res == 5)cout<<n-3<<"MB"<<endl;
>     	    if(res == 3)cout<<n+3<<"UB"<<endl;
>     	    if(res == 6)cout<<n-3<<"UB"<<endl;
>     	    if(res == 0)cout<<n-1<<"SL"<<endl;
>     	    if(res == 7)cout<<n+1<<"SU"<<endl;
>     	}
>     	return 0;
>     }

Time taken : 15 min
