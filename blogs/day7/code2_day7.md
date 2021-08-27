**CodeBlog**

Day : 7

Problem solved : 2/4

Problem : **# Chef and SnackDown**

[Problem Statement](https://www.codechef.com/problems/SNCKYEAR)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>         int t;
>         cin>>t;
>     	while(t--){
>     	    int n;
>     	    cin>>n;
>     	    if(n == 2010 || n == 2015 || n == 2016 || n == 2017 || n == 2019){
>     	        cout<<"HOSTED"<<endl;
>     	    }
>     	    else
>     	    {
>     	        cout<<"NOT HOSTED"<<endl;
>     	    }
>     	}
>     	return 0;
>
> Time taken : 4 min
