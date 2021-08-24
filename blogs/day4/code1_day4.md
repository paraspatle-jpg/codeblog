**CodeBlog**

Day : 4

Problem solved : 1/4

Problem : ** # IPL and RCB**

[Problem Statement](https://www.codechef.com/problems/CLIPLX)

Approach : I approached the problem thinking that if i want to find minimum number of match wins then i have to find maximum number of matches which can be tied and losing was out of the option.

Topics: Basic C++ , Apitude

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int t;
>     	cin>>t;
>     	while(t--)
>     	{
>     	    int x,y;
>     	    cin>>x>>y;
>     	    int count=0;
>     	    int res=0;
>     	    while(x-count > y)
>     	    {
>     	        count = count +2;
>     	        res++;
>     	        y--;
>     	    }
>     	    cout<<res<<endl;
>     	}
>     	return 0;
>     }

Time taken : 12 min
