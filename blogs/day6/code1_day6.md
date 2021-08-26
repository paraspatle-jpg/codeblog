**CodeBlog**

Day : 6

Problem solved : 1/4

Problem : **# Magician versus Chef**

[Problem Statement](https://www.codechef.com/problems/MAGICHF)

Approach :

Topics: Basic C++

> Code:
>
>      #include <bits/stdc++.h>
>     using namespace std;
>     int main() {
>     	int t;
>     	cin>>t;
>     	while(t--)
>     	{
>     	    int n,x,s;
>     	    cin>>n>>x>>s;
>     	    int a,b;
>     	    for(int i = 0; i<s ; i++)
>     	    {
>     	        cin>>a>>b;
>     	        if(a==x)
>     	        {
>     	            x = b;
>     	        }
>     	        else if(b==x)
>     	        {
>     	            x = a;
>     	        }
>     	    }
>     	    cout<<x<<endl;
>     	}
>     	return 0;
>     }

Time taken : 9 min
