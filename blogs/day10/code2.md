**CodeBlog**

Day : 10

Problem solved : 2/4

Problem : **# Airline Restrictions**

[Problem Statement](https://www.codechef.com/SEPT21C/problems/AIRLINE)

Approach :

Topics: Basic C++

> Code:
>
>     #include <bits/stdc++.h>
>     using namespace std;
>
>     int main() {
>     	int t;
>     	cin>>t;
>     	while(t--){
>     	    int a,b,c,d,e;
>     	    cin>>a>>b>>c>>d>>e;
>     	    if(a+b<=d && c<=e){
>     	        cout<<"YES"<<endl;
>     	    }
>     	    else if(c+b<=d && a<=e){
>     	        cout<<"YES"<<endl;
>     	    }
>     	    else if(c+a<=d && b<=e){
>     	        cout<<"YES"<<endl;
>     	    }
>     	    else
>     	    {
>     	        cout<<"NO"<<endl;
>     	    }
>     	}
>     	return 0;
>     }

Time Taken : 8min
